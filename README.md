# Pytorch CPA

Principal Component Anlaysis (PCA) in PyTorch. The intention is to provide a
simple and easy to use implementation of PCA in PyTorch, the most similar to
the `sklearn`'s PCA as possible (in terms of API and, of course, output).

![PythonVersion](https://img.shields.io/badge/python-3.8%20%7E%203.11-informational)
![PytorchVersion](https://img.shields.io/badge/pytorch-1.8%20%7E%201.13%20%7C%202.0+-informational)

[![GitHub User followers](https://img.shields.io/github/followers/valentingol?label=User%20followers&style=social)](https://github.com/valentingol)
[![GitHub User's User stars](https://img.shields.io/github/stars/valentingol?label=User%20Stars&style=social)](https://github.com/valentingol)

[![Ruff_logo](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
[![Black_logo](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

[![Ruff](https://github.com/valentingol/torch_pca/actions/workflows/ruff.yaml/badge.svg)](https://github.com/valentingol/Dinosor/actions/workflows/ruff.yaml)
[![Flake8](https://github.com/valentingol/torch_pca/actions/workflows/flake.yaml/badge.svg)](https://github.com/valentingol/Dinosor/actions/workflows/flake.yaml)
[![Pydocstyle](https://github.com/valentingol/torch_pca/actions/workflows/pydocstyle.yaml/badge.svg)](https://github.com/valentingol/Dinosor/actions/workflows/pydocstyle.yaml)
[![MyPy](https://github.com/valentingol/torch_pca/actions/workflows/mypy.yaml/badge.svg)](https://github.com/valentingol/Dinosor/actions/workflows/mypy.yaml)

## Installation

```bash
pip install torch-cpa
```

## How to use

```python
from torch_cpa import PCA

# Create like sklearn.decomposition.PCA
pca_model = PCA(n_components=None, whiten=False)

# Use like sklearn.decomposition.PCA
>>> new_X1 = pca_model.fit_transform(X1)
>>> new_X2 = pca_model.transform(X2)
>>> print(pca.explained_variance_ratio_)
[0.756, 0.142, 0.062, ...]
```
