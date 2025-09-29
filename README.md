# 🌍 Data-Driven Parameterizations for Climate Models

This repository collects machine learning–based parameterizations developed in the **AI4PEX project**, providing reusable modules for Earth system modeling.  
Each parameterization is maintained as a submodule with its own documentation and license.  

---

## 🚀 Getting Started

- Browse the available parameterizations by domain (Land, Atmosphere, Ocean).  
- Follow the links to each submodule’s **README** for setup and usage.  
- Quickstart guides (coming soon) will provide examples for applying each method to your own data and challenges.  

---

## 📂 Available Parameterizations

### 🌲 Land + ☁️ Atmosphere
- [Hybrid Model of Land-Atmosphere Fluxes for ICON-ESM](https://github.com/relghawi/Hybrid_JSBACH_Example)  
  ![python](https://img.shields.io/badge/python-yellow) ![land](https://img.shields.io/badge/land-darkgreen) ![atmosphere](https://img.shields.io/badge/atmosphere-lightblue) [![License: GPL-3.0](https://img.shields.io/badge/License-GPL-yellow.svg)](https://opensource.org/licenses/GPL-3-0) [![paper](https://img.shields.io/badge/paper-gray)](https://doi.org/10.22541/essoar.174439495.50028878/v1) 

---

### 🌲 Land
- [Hybrid Q10 Model with Double Machine Learning](https://github.com/KaiHCohrs/hybrid-q10-model-chm)  
  ![python](https://img.shields.io/badge/python-yellow) ![land](https://img.shields.io/badge/land-darkgreen) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![paper](https://img.shields.io/badge/paper-gray)](https://doi.org/10.1088/2632-2153/ad5a60)

- [NN-based Respiration and GPP from Flux Partitioning](https://github.com/KaiHCohrs/nn-flux-part)  
  ![python](https://img.shields.io/badge/python-yellow) ![land](https://img.shields.io/badge/land-darkgreen) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![paper](https://img.shields.io/badge/paper-gray)](https://doi.org/10.1088/2632-2153/ad5a60)
  
- [Hybrid Variational Inference for Soil Organic Matter dynamics](https://github.com/EarthyScience/HybridVariationalInference.jl)  
  ![julia](https://img.shields.io/badge/julia-purple) ![land](https://img.shields.io/badge/land-darkgreen) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)  

**Coming soon:**  
- Parameterizations of tree mortality directly from satellite and climate data  
- Tree mortality likelihood parameterization  

---

### ☁️ Atmosphere
- [First ICON-A-MLe model: Data-driven cloud cover equation in ICON-A 2.6.4 with subsequent automatic tuning](https://github.com/EyringMLClimateGroup/grundner25_iconaml_automatic_tuning)  
  ![python](https://img.shields.io/badge/python-yellow) ![atmosphere](https://img.shields.io/badge/atmosphere-lightblue) [![License: MIT](https://img.shields.io/badge/License-Apache-yellow.svg)](https://opensource.org/licenses/Apache-2-0) [![paper](https://img.shields.io/badge/paper-gray)](https://doi.org/10.48550/arXiv.2505.04358) 

  - **Guide:** [How to implement the data-driven cloud cover equation in ICON-A (2.6.4.)](https://github.com/AI4PEX/data-driven-parametrizations/blob/main/How_to_bridge_to_ICON.md) 

- [Hierarchical modeling framework to discover new ML-based equations for cloud cover, including symbolic regression](https://github.com/EyringMLClimateGroup/grundner23james_EquationDiscovery_CloudCover)  
  ![python](https://img.shields.io/badge/python-yellow) ![atmosphere](https://img.shields.io/badge/atmosphere-lightblue) [![License: MIT](https://img.shields.io/badge/License-Apache-yellow.svg)](https://opensource.org/licenses/Apache-2-0) [![paper](https://img.shields.io/badge/paper-gray)](https://doi.org/10.1029/2023MS003763) 

  - **Quickstarts** on a data-driven cloud cover equation discovery:
    - [from synthetic data](https://github.com/EyringMLClimateGroup/grundner23james_EquationDiscovery_CloudCover/blob/main/quickstart_synth_data.ipynb) 
    - [from real data](https://github.com/EyringMLClimateGroup/grundner23james_EquationDiscovery_CloudCover/blob/main/quickstart_real_data.ipynb) 

- [Stochastic Recurrent Neural Network for modeling Atmospheric Regimes](https://github.com/andrei-ml/stochastic-rnn)  
  ![python](https://img.shields.io/badge/python-yellow) ![atmosphere](https://img.shields.io/badge/atmosphere-lightblue) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)  
    - [Quickstart](https://github.com/andrei-ml/stochastic-rnn/blob/main/quickstart_with_synthetic_example/quickstart.ipynb) using synthetic data
  

**Coming soon:**  
- Convection parameterization trained on ClimSim data for the ICON model  
- Improving vertical detail in simulated temperature and humidity  

---

### 🌊 Ocean
**Coming soon:**  
- Emulation of PISCES biogeochemical model  
- Predicting eddy energy using a CNN for use in the scale-aware GEOMETRIC eddy parameterization  

---

## 📋 Roadmap

- [ ] Add quickstart guides for each method  
- [ ] Expand documentation and folder organization  
- [ ] Review contribution guidelines   

---

## 📬 Contact

For questions and contributions, please reach out to the [ISP at UVEG](https://isp.uv.es/):  
- Gherardo Varando <gherardo.varando@uv.es>  
- Andrei Gavrilov <andrei.gavrilov@uv.es>  
- Kai-Hendrik Cohrs <kai.cohrs@uv.es>  

---
