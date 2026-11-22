# Multiclass Classification from Scratch: One-vs-All and All-Pairs

DATA 2060 final project.

## Overview

Logistic regression can only separate two classes. This project builds two multiclass classifiers on top of it: **one-vs-all**, which trains one binary model per class and predicts the most confident one, and **all-pairs**, which trains one binary model per pair of classes and predicts the class with the most votes. Both use regularized binary logistic regression trained with mini-batch stochastic gradient descent, implemented from scratch in NumPy. We apply them to the handwritten Digits dataset (10 classes), show that our predictions exactly reproduce scikit-learn's `OneVsRestClassifier` and `OneVsOneClassifier`, and compare the two methods.

## Repository structure

```
├── data/          # dataset (digits.csv)
├── src/           # Jupyter notebook with the report and code
├── .gitignore
├── LICENSE
├── README.md
├── environment.yml
├── presentation.pdf
└── report.pdf
```

## Requirements

The code was developed with:

| Package | Version |
|---|---|
| Python | 3.14.7 |
| NumPy | 2.5.2 |
| pandas | 3.0.5 |
| matplotlib | 3.11.1 |
| scikit-learn | 1.9.0 |
| pytest | 9.1.1 |
| Jupyter | 1.1.1 |

## How to run

1. Clone the repository:
   ```bash
   git clone https://github.com/SimaRaha/multiclass-classification-from-scratch.git
   cd multiclass-classification-from-scratch
   ```
2. Create and activate the environment:
   ```bash
   conda env create -f environment.yml
   conda activate data2060-multiclass
   ```
3. Open `src/multiclass_classification.ipynb` in Jupyter and run all cells.

## Authors

- George Chudley: <george_chudley@brown.edu>
- Sima Raha: <sima_raha@brown.edu>
- Yuan Ying: <yuan_ying@brown.edu>
- Kunhao Yue: <kunhao_yue@brown.edu>

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
