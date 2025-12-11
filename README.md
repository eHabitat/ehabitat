<p align="center">
        <a>
	    <img src='https://img.shields.io/badge/python-3.7%7C3.8%7C3.9%2B-blueviolet' alt='Python' />
	</a>
	<a href='https://xgen-timeseries.readthedocs.io/en/latest/?badge=latest'>
    	    <img src='https://readthedocs.org/projects/xgen-timeseries/badge/?version=latest' alt='Documentation Status' />
	</a>
	<a href='https://creativecommons.org/licenses/by/4.0/'>
	    <img alt="CC 4.0 - License" src="https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg">
	</a><br>
</p>
</p>

# **eHabitat — Open-Source Time Series Dataset & Tools**

**eHabitat** is an open-source project providing data, tools, and utilities for building and evaluating models related to energy monitoring, appliance-level analysis, and carbon-footprint estimation.
It offers a unified framework that simplifies working with electricity consumption data, running experiments, and developing data-driven energy applications.

## 🚀 Features

* **Unified data loading interface**
* **Preprocessing & cleaning pipelines**
* **Baseline NILM and signal decomposition methods**
* **Evaluation metrics for energy monitoring tasks**
* **Visualization utilities**
* **Support for dataset extensions**
* **Lightweight and easy to integrate into existing workflows**

---

## 📦 Repository Structure

```
eHabitat/
│
├── data/                # dataset interface + loaders
├── models/              # baseline models
├── preprocessing/       # cleaning, normalization, filtering
├── evaluation/          # metrics and evaluation scripts
├── examples/            # tutorials and usage examples
└── docs/                # documentation for GitHub Pages
```

---

## 📖 Documentation

Documentation is available through GitHub Pages and includes:

* Getting started
* Installation
* Basic usage
* API reference

```bash
git clone https://github.com/<your-org>/eHabitat.git
cd eHabitat
pip install -r requirements.txt
```

---

## 🧪 How to use 

```python
from ehabitat import load_dataset

data = load_dataset("example")
aggregate, appliances = data["aggregate"], data["appliances"]
```

---

## 📄 License

This project is released under an **open-source license**.
See `LICENSE` for details.

---
