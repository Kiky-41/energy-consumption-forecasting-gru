# 📈 Energy Consumption Forecasting in Indonesia
[![DOI](https://zenodo.org/badge/1206693098.svg)](https://doi.org/10.5281/zenodo.19492753)

Time series forecasting implementation for energy consumption analysis in Indonesia, combining deep learning and statistical approaches.

This project is part of ongoing research on data-driven energy modeling and future demand projection using CNN, GRU, and ARIMA methods.

---

## 📄 Related Publication

Yustika, L.M., Ikhsan, R.R.N., Raharjo, J., Callista, A.A., Abdiary, M.A. (2025)
*Future Trends of Energy Consumption in Indonesia Through CNN-based Modeling*
2025 IEEE International Conference on Industry 4.0, Artificial Intelligence, and Communications Technology (IAICT)
https://doi.org/10.1109/IAICT65714.2025.11101693

---

## 🚀 Features

- 📊 Time series forecasting of **national energy consumption**
- 🧠 Deep learning model: **GRU (Gated Recurrent Unit)**
- 📉 Statistical baseline: **ARIMA**, **CNN**
- ⚙️ Full pipeline including:
  - Data preprocessing
  - Sequence generation for time series modeling
  - Model training and evaluation
- 📈 Visualization of actual vs predicted values
- 🔁 Suitable for **energy planning and demand projection**

---

## 🧠 Method Overview

The forecasting problem aims to minimize prediction error over the time horizon:

$$\hat{y}_{t+h} = f(y_t, y_{t-1}, \ldots, y_{t-p})$$

Models implemented and compared:

- **CNN** (paper) → convolutional feature extraction from temporal sequences
- **GRU** (this repo) → gated recurrent unit for sequential dependency modeling
- **ARIMA** → classical statistical baseline for comparison

Performance is evaluated using MAPE and R² across all model variants.

---

## 📊 Evaluation Metrics

| Metric | Description |
|--------|-------------|
| MAPE   | Mean Absolute Percentage Error |
| R²     | Coefficient of determination |

Results include visual comparison between actual and predicted energy consumption values.

---

## 📂 Project Structure

```text
energy-forecasting-indonesia/
├── GRU.ipynb       # Main notebook: model implementation & experiments
├── README.md
└── .gitignore
```

---

## ⚙️ Requirements

- Python 3.x
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- TensorFlow
- OpenPyXL
- Jupyter Notebook

Install all dependencies:

```bash
pip install numpy pandas matplotlib scikit-learn tensorflow openpyxl jupyter
```

---

## ▶️ Usage

Clone and run the notebook:

```bash
git clone https://github.com/Kiky-41/energy-forecasting-indonesia.git
cd energy-forecasting-indonesia
jupyter notebook
```

Open `GRU.ipynb` and run all cells.

---

## 📊 Dataset

> ⚠️ The dataset used in the original research is not included in this repository.

To run the notebook, you need to:
- Provide your own dataset with a similar structure, or
- Adapt the preprocessing code to match your data format

Make sure to update the file path in the notebook accordingly.

**Expected dataset format:**

| Column | Description |
|--------|-------------|
| Date   | Time index (yearly or monthly) |
| Energy_Consumption | Total energy consumption value |

**Example (CSV):**

```csv
Date,Energy_Consumption
2000,1234.5
2001,1289.3
2002,1345.7
```

> 💡 A note is included at the top of the notebook to guide you on providing your own data.

---

## 📌 Reproducibility

This repository focuses on the model implementation and experimental pipeline.
Exact reproduction of published results requires the original dataset used in the paper.

---

## 📖 Citation

If you use this work, please cite:

```bibtex
@inproceedings{yustika2025energy,
  title={Future Trends of Energy Consumption in Indonesia Through CNN-based Modeling},
  author={Yustika, Lindiasari Martha and Ikhsan, Rifki Rahman Nur and Raharjo, Jangkung and Callista, Areta Adelia and Abdiary, Muhammad Albaihaq},
  booktitle={2025 IEEE International Conference on Industry 4.0, Artificial Intelligence, and Communications Technology (IAICT)},
  pages={311--317},
  year={2025},
  doi={10.1109/IAICT65714.2025.11101693}
}
```

---

## 🔗 DOI (Zenodo)

After creating a GitHub release, Zenodo will automatically generate a DOI for this repository.

---

## 📜 License

MIT License

---

## 🙌 Acknowledgements

This work is based on research in energy demand forecasting, deep learning for time series, and Indonesia's national energy planning.

---

## ⭐ Support

If you find this repository useful:
- ⭐ Star this repo
- 🍴 Fork and contribute
- 📢 Share with the research community
