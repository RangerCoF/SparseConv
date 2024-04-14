# Sparsity Invariant CNNs
This repository contains the code for reproducibility project of paper [Sparsity Invariant CNNs](https://ieeexplore.ieee.org/abstract/document/8374553).

### TUD 2023-2024 CS4240 Group75
Members:
* Zhixuan Ge (5927633)
* Jiarui Zhou (6017002)
* Junchi Liu (5983533)

## Setup
To check and run the code, please first clone or download this repository.

The directories are structured as follow:
```
SparseConv/
│
├── Caltech 101/
│   ├── Conv.ipynb  # Normal ConvNet for Caltech 101
│   └── SparseConv.ipynb # Sparse ConvNet for Caltech 101
│
├── MNIST/
│   ├── ACC.ipynb #  Plot how accuracy changes as sparsity increases
│   ├── Conv.ipynb  # Normal ConvNet for MNIST
│   └── SparseConv.ipynb # Sparse ConvNet for MNIST
│
└── Resnet18/
│   ├── Resnet18.ipynb # Normal Resnet for MNIST
│   └── SparseResnet18.ipynb # Sparse Resnet for MNIST
│
├── Blog.pdf # Blog for reproducibility project
└── README.md
```

Each Jupyter Notebook file contais complete code for the corresponding network. You can run the code step by step to get the result in our blog.

Note: All the experiments are run on Google Colab. To accelerate training, all images are stored in RAM during training. You are expected to have about 20 GB to continue the training.

## Quick Look Up
The results of our reproducibility project are as follow.

#### Accuracy on MNIST

|Sparsity|5%|10%|20%|30%|40%|50%|60%|70%|80%|90%|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|ConvNet|98.88%|98.70%|98.26%|98.26%|98.01%|97.47%|96.80%|95.11%|91.81%|78.58%|
|SparseConvNet|98.72%|98.77%|98.52%|98.02%|97.94%|97.23%|96.61%|95.65%|91.20%|75.77%|

#### Accuracy on Caltech 101
|Sparsity|5%|10%|20%|30%|40%|50%|60%|70%|80%|90%|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|ConvNet|63.94%|65.09%|63.13%|63.42%|59.50%|59.27%|58.81%|57.26%|54.84%|51.15%|
|SparseConvNet|63.42%|65.09%|63.59%|62.85%|60.02%|55.01%|58.47%|56.28%|54.15%|51.67%|

