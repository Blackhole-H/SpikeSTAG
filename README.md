# SpikeSTAG
```markdown
# Installation

To install SeqSNN in a new conda environment:

```bash
conda create -n SeqSNN python=[3.8, 3.9, 3.10]  
conda activate SeqSNN  
git clone https://github.com/microsoft/SeqSNN/  
cd SeqSNN  
pip install .  
```

If you would like to make changes and run your experiments, use:

```bash
pip install -e .
```

# Training

Take the `ispikformer` model as an example:

```bash
python -m SeqSNN.entry.tsforecast exp/forecast/ispikformer/ispikformer_electricity.yml  
```

You can change the `yml` configuration files as you want.

You can add, remove, or modify your model architecture in `SeqSNN/network/XXX.py`.

---

# Datasets

Mett-la and Pems-bay are available at Google Drive or Baidu Yun. Solar and Electricity can be downloaded from  
[this link](https://github.com/laiguokun/multivariate-time-series-data).

The folder structure of this project is as follows:

```
SeqSNN
├── README.md
├── data
│   ├── metr-la.h5
│   ├── pems-bay.h5
│   ├── solar-energy
│   │   └── solar_AL.txt
│   ├── electricity
│   │   └── electricity.txt
│   ├── traffic
│   │   └── traffic.txt
│   ├── forecaster
│   └── outputs
├── exp
└── ...
```

You can change the path of the data file in `exp/forecast/dataset/XXX.yml` configuration files.

---

# Acknowledgement

This repo is built upon [forecaster](https://github.com/Arthur-Null/SRD), which is a general time-series forecasting library. We greatly thank @rk2900 and @Arthur-Null for their initial contribution.
```
