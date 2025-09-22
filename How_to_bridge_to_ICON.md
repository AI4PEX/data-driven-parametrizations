**How to implement the data-driven cloud cover equation in ICON-A (2.6.4.)**

Take https://github.com/EyringMLClimateGroup/grundner25_iconaml_automatic_tuning/blob/main/data_driven_cloud_cover_scheme.txt

Here: ptm1 = air temperature [K], pxlm1 = cloud water [kg/kg], pxim1 = cloud ice [kg/kg], papm1 = air pressure [p], pqm1 = specific humidity [kg/kg], zf = Height at full levels [m].

In the mo_cover.f90 script, this cloud cover equation must be added as an additional option. Appearing variables must be declared in the header of the script.
The new tunable parameters must be permitted in the ICON code. After those changes, the ICON-code needs to be reconfigured.

A complete implementation can be found [here](https://gitlab.dkrz.de/icon-ml/icon_developments/icon-a-ml/-/blob/icon-2-6-4-ml_cloud_cover/src/atm_phy_echam/mo_cover.f90?ref_type=heads) (might require special access).

The tunable parameters of the equation are then set in the runscript as follows:
https://github.com/EyringMLClimateGroup/grundner25_iconaml_automatic_tuning/blob/main/simulation_scripts_and_evaluation/auto_tuned_iconaml_full/exp.ag_atm_amip_r2b5_cvtfall_entrmid_05_cov15_based_on_12962670_20yrs_240927.run

**Differences when implementing the scheme in ICON-NWP**

In the default cloud cover scheme of [ICON-NWP](https://gitlab.dkrz.de/icon/icon-model), two specific measures of cloud cover (convective and turbulent) are estimated in each grid cell. 
Each of those is used to modify cloud ice/water. Eventually the two cloud cover measures are combined to get a single cloud cover measure.
See case 1 in this [code](https://gitlab.dkrz.de/icon/icon-model/-/blob/release-2025.04-public/src/atm_phy_schemes/mo_cover_koe.f90?ref_type=heads).
There are two options for how to implement the data-driven cloud cover equation (that does not differentiate between convective and turbulent cloud cover).
The first one is to treat the cloud cover estimate of the data-driven scheme as the authoritative turbulent cloud cover within the native scheme (case 1).
The second option treats the cloud cover estimate of the data-driven scheme as the authoritative `total' cloud cover within the native scheme (case 1).  
It combines the estimates of turbulent and convective cloud cover with that of the data-driven equation to derive the amount of overlap that necessarily needs to be there s.t. the given turbulent and convective portions can yield the given total cloud cover.
We can use this overlap to derive better informed estimates of total cloud ice/water. 

Remark: To implement neural networks in ICON, we used the Fortran-Keras-Bridge (https://github.com/scientific-computing/FKB/tree/master) for ICON-A 2.6.4 and FTorch (https://github.com/Cambridge-ICCS/FTorch) for ICON-NWP (only a remark as the NNs were not the main focus of the publications).