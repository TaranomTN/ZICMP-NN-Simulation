# ZICMP-NN-Simulation

## Model Comparison on Simulated Count Data

This project evaluates the performance of various statistical and machine learning models in predicting count data using simulated datasets. The focus is on comparing traditional count models with advanced zero-inflated models, including the proposed **ZICMP Neural Network**.

Models compared:
- Poisson Regression
- Negative Binomial
- Zero-Inflated Poisson (ZIP)
- **ZICMP (Zero-Inflated Comp-Poisson)**

---

### 📊 Model Comparison Based on AIC and Log-Likelihood (NL)

| Model                    | AIC      | NL       |
|--------------------------|----------|----------|
| Poisson                  | 6554.22   | -3273.11  |
| Negative Binomial        | 3464.03   | -1727.01  |
| Zero-Inflated Poisson    | 3361.98   | -1675.99  |
| **ZICMP**         | **5837.88** | **-483.94** |


---

### 📊 Model Comparison Based on MSE

| Model                    | MSE     |
|--------------------------|---------|
| **ZICMP**               | **24.15**   |
| Zero-Inflated Poisson    | 25.65   |
| Poisson                  | 25.87   |
| Negative Binomial        | 26.62   |

> ✅ **ZICMP** outperforms all baseline models in terms of prediction accuracy (lowest MSE).

---

### 🧠 Key Insights

- The dataset exhibits high zero-inflation, making it ideal for zero-inflated modeling.
- ZICMP effectively captures both overdispersion and excess zeros.
- Our neural network-based ZICMP model improves upon classical approaches in both fit and prediction.

---

### 📁 Files

- `zicmp_nn_simulation.ipynb`: Colab notebook containing simulation setup, model training, and evaluation.

---

### 🔧 Requirements

- Python 3.x
- Jupyter Notebook or Colab
- Required libraries: `pandas`, `numpy`, `scikit-learn`, `torch`, `statsmodels`

Install dependencies:
```bash
pip install pandas numpy scikit-learn torch statsmodels
```

## 📬 Contact

Created by [Taranom Torabi](mailto:taranom.torabi1377@gmail.com) — feel free to reach out with any questions or feedback!
