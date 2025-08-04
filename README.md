# SpikeSTAG
```markdown
To install SpikeSTAG in a new conda environment:

```bash
conda create -n SeqSNN python=3.9  
conda activate SpikeSTAG  
git clone https://github.com/microsoft/SeqSNN/
cd SpikeSTAG 
pip install .  
```

# Training

```bash
python -m SeqSNN.entry.tsforecast exp/forecast/spikegnn/spikegnn_metr-la.yml  
```

You can change the `yml` configuration files as you want.
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

```
