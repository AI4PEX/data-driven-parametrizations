# 🌍 Data-Driven Parameterizations for Climate Models

This repository collects machine learning–based parameterizations and emulators of climate processes developed in the **AI4PEX project**, providing reusable modules for Earth system modeling.  
Each parameterization is maintained as a submodule, or as a linked archive, with its own documentation and license.  Note: The equation discovery module (Grundner 2024) is provided as Background IP necessary for the ICON-A-MLe integration developed under AI4PEX. 

---

## 🚀 Getting Started

- Browse the available parameterizations by methodology class, with domain indicated by badges.  
- Follow the links to each submodule’s **README** for setup and usage.  
- Quickstart guides, where available, provide examples for applying a method to your own data and challenges.  
- To clone the repository including all submodules:
```bash
git clone --recurse-submodules https://github.com/AI4PEX/data-driven-parametrizations
```

---

## 📂 Available Parameterizations

### 📐 Analytic and equation-based closure methods

- [Equation Discovery of Cloud Cover Parameterization: Hierarchical modeling framework to discover new ML-based equations for cloud cover, including symbolic regression](https://github.com/EyringMLClimateGroup/grundner23james_EquationDiscovery_CloudCover)  
  ![atmosphere](https://img.shields.io/badge/atmosphere-lightblue) ![python](https://img.shields.io/badge/python-yellow) [![License: Apache](https://img.shields.io/badge/License-Apache-yellow.svg)](https://opensource.org/licenses/Apache-2-0) [![paper](https://img.shields.io/badge/paper-gray)](https://doi.org/10.1029/2023MS003763) 

  - **Quickstarts** on a data-driven cloud cover equation discovery:
    - [from synthetic data](https://github.com/EyringMLClimateGroup/grundner23james_EquationDiscovery_CloudCover/blob/main/quickstart_synth_data.ipynb) 
    - [from real data](https://github.com/EyringMLClimateGroup/grundner23james_EquationDiscovery_CloudCover/blob/main/quickstart_real_data.ipynb) 

- [Leith subgrid closures for parameterising mesoscale eddies in idealised and global (NEMO) ocean models](https://zenodo.org/records/15703784)  
  ![ocean](https://img.shields.io/badge/ocean-blue) ![python](https://img.shields.io/badge/python-yellow) [![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-yellow.svg)](https://creativecommons.org/licenses/by/4.0/) [![paper](https://img.shields.io/badge/paper-gray)](https://doi.org/10.1029/2025MS004950)  

---

### 🔗 Hybrid and semiparametric modeling strategies

- [Enhancement of Physical Models with Rashomon-Set-Controlled Deep Learning for Robust Inference and Extrapolation](https://github.com/KaiHCohrs/rashomon-hybrid-modeling)  
  ![generic](https://img.shields.io/badge/generic-gray) ![land](https://img.shields.io/badge/land-darkgreen) ![python](https://img.shields.io/badge/python-yellow) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 

- [Hybrid JSBACH: Hybrid Model of Land-Atmosphere Fluxes for ICON-ESM](https://github.com/relghawi/Hybrid_JSBACH_Example)  
  ![land](https://img.shields.io/badge/land-darkgreen) ![atmosphere](https://img.shields.io/badge/atmosphere-lightblue) ![python](https://img.shields.io/badge/python-yellow) [![License: GPL-3.0](https://img.shields.io/badge/License-GPL-yellow.svg)](https://opensource.org/licenses/GPL-3-0) [![paper](https://img.shields.io/badge/paper-gray)](https://doi.org/10.1029/2025MS005102) 

- [Hybrid Variational Inference for Soil Organic Matter dynamics](https://github.com/EarthyScience/HybridVariationalInference.jl)  
  ![land](https://img.shields.io/badge/land-darkgreen) ![julia](https://img.shields.io/badge/julia-purple) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)  

- [Convection parameterizations for ICON-A: Confidence-Guided Mixing of Parameterizations in a Hybrid AI-Climate Model](https://github.com/EyringMLClimateGroup/heuer25james_ml_convection_climsim)  
  ![atmosphere](https://img.shields.io/badge/atmosphere-lightblue) ![python](https://img.shields.io/badge/python-yellow) [![License: Apache](https://img.shields.io/badge/License-Apache-yellow.svg)](https://opensource.org/licenses/Apache-2-0) [![paper](https://img.shields.io/badge/paper-gray)](https://doi.org/10.1029/2025MS005544) 

---

### 🧠 Standalone supervised learning and emulation methods

- [Stochastic Recurrent Neural Network for modeling Atmospheric Regimes](https://github.com/andrei-ml/stochastic-rnn)  
  ![generic](https://img.shields.io/badge/generic-gray) ![atmosphere](https://img.shields.io/badge/atmosphere-lightblue) ![python](https://img.shields.io/badge/python-yellow) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)  
    - [Quickstart](https://github.com/andrei-ml/stochastic-rnn/blob/main/quickstart_with_synthetic_example/quickstart.ipynb) using synthetic data

- [Engression-LSTM: a Deep Generative Time-Series Approach for Streamflow Regression](https://github.com/bask0/mach-flow-engression)  
  ![generic](https://img.shields.io/badge/generic-gray) ![land](https://img.shields.io/badge/land-darkgreen) ![python](https://img.shields.io/badge/python-yellow) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![paper](https://img.shields.io/badge/paper-gray)](https://doi.org/10.1029/2025GL120122)

- [Vertical superresolution: Improving Vertical Detail in Simulated Temperature and Humidity Data Using Machine Learning](https://github.com/jdsrodrigues/superresolution)  
  ![atmosphere](https://img.shields.io/badge/atmosphere-lightblue) ![python](https://img.shields.io/badge/python-yellow) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![paper](https://img.shields.io/badge/paper-gray)](https://doi.org/10.1002/asl.1288)

- [CNN and U-Net models for a Machine Learning eddy parameterisation for NEMO](https://github.com/thomaswilder/ml_model_ai4pex)  
  ![ocean](https://img.shields.io/badge/ocean-blue) ![python](https://img.shields.io/badge/python-yellow) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 

- [PISCES-AI: a U-Net based emulator of the PISCES biogeochemical model](https://github.com/edwardgowsmith/PISCES-AI)  
  ![ocean](https://img.shields.io/badge/ocean-blue) ![python](https://img.shields.io/badge/python-yellow) [![License: GPL-3.0](https://img.shields.io/badge/License-GPL-yellow.svg)](https://opensource.org/licenses/GPL-3-0)

- [MortNetSE parameterization pipeline](https://github.com/AdrianGustafson/MortNetSE-parameterisation-pipeline)  
  ![land](https://img.shields.io/badge/land-darkgreen) ![python](https://img.shields.io/badge/python-yellow) [![License: GPL-3.0](https://img.shields.io/badge/License-GPL-yellow.svg)](https://opensource.org/licenses/GPL-3-0) 
    - Includes a **quickstart notebook** with example data

---

### ⚙️ Calibration and online evaluation strategies

- [ClimSim Kaggle Edition: Online Testing of Machine Learning Emulators of Cloud and Convection Processes](https://github.com/leap-stc/climsim-kaggle-edition)  
  ![atmosphere](https://img.shields.io/badge/atmosphere-lightblue) ![python](https://img.shields.io/badge/python-yellow) [![License: Apache](https://img.shields.io/badge/License-Apache-yellow.svg)](https://opensource.org/licenses/Apache-2-0) [![paper](https://img.shields.io/badge/paper-gray)](https://doi.org/10.1029/2025MS005643) 

  - [Demo notebooks](https://github.com/leap-stc/climsim-kaggle-edition/tree/main/demo_notebooks) 

- [Euler Gradient Approximation: Online Calibration of Deep Learning Sub-Models for Hybrid Numerical Modeling Systems](https://github.com/saidOUALA/EGA)  
  ![generic](https://img.shields.io/badge/generic-gray) ![ocean](https://img.shields.io/badge/ocean-blue) ![python](https://img.shields.io/badge/python-yellow) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![paper](https://img.shields.io/badge/paper-gray)](https://www.nature.com/articles/s42005-024-01880-7)

- [ICON-A Automatic Tuning: First ICON-A-MLe model: Data-driven cloud cover equation in ICON-A 2.6.4 with subsequent automatic tuning](https://github.com/EyringMLClimateGroup/grundner25_iconaml_automatic_tuning)  
  ![atmosphere](https://img.shields.io/badge/atmosphere-lightblue) ![python](https://img.shields.io/badge/python-yellow) [![License: Apache](https://img.shields.io/badge/License-Apache-yellow.svg)](https://opensource.org/licenses/Apache-2-0) [![paper](https://img.shields.io/badge/paper-gray)](https://doi.org/10.1038/s41598-025-29155-3) 

  - **Guide:** [How to implement the data-driven cloud cover equation in ICON-A (2.6.4.)](https://github.com/AI4PEX/data-driven-parametrizations/blob/main/How_to_bridge_to_ICON.md) 

---


## License

This repository is released under the MIT License, which covers its own content: this welcome page, the documentation and the links between entries. It does not extend to the parameterizations themselves. Each entry is governed by its own license, indicated by the badge beside it, and users should observe the license of the specific entry they intend to use.

---

## 📬 Contact

For questions and contributions, please reach out to the [ISP at UVEG](https://isp.uv.es/):  
- Andrei Gavrilov <andrei.gavrilov@uv.es>  
- Gherardo Varando <gherardo.varando@uv.es>  
- Kai-Hendrik Cohrs <kai.cohrs@uv.es>  

---