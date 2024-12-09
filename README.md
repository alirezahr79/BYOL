# 📈 BYOL (Bootstrap Your Own Latent) – From Scratch Implementation in PyTorch

<p align="center">
  <img src="https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white" alt="PyTorch">
  <img src="https://img.shields.io/badge/Python-3670A0?style=for-the-badge&logo=Python&logoColor=ffdd54" alt="Python">
  <img src="https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=white" alt="Jupyter Notebook">
  <img src="https://img.shields.io/badge/license-MIT-blue.svg?style=for-the-badge" alt="License">
  <img src="https://img.shields.io/github/stars/deepmancer/byol-pytorch?style=for-the-badge" alt="GitHub Stars">
</p>

Welcome to the **BYOL (Bootstrap Your Own Latent)** repository! This project provides a comprehensive, from-scratch implementation of BYOL, a revolutionary self-supervised learning algorithm. Whether you're a researcher, developer, or enthusiast, this repository offers valuable insights into state-of-the-art unsupervised feature learning.

---

## 🚀 Key Highlights

- **From-Scratch Implementation**: Dive deep into the mechanics of BYOL with clean, understandable PyTorch code.
- **Self-Supervised Learning**: Explore a negative-sample-free approach to feature learning.
- **Documentation**: Clear explanations, visualizations, and results to aid your understanding.
- **Interactive Notebooks**: Experiment hands-on with our Jupyter notebooks.

---

## 🧠 What is BYOL?

**Bootstrap Your Own Latent (BYOL)** is a self-supervised learning algorithm that breaks new ground by learning from positive pairs (different augmentations of the same image) without relying on negative samples. This simplicity leads to faster training and competitive results across a range of benchmarks.

### ✨ Key Features:
- **No Negative Samples**: Reduces complexity while maintaining high performance.
- **State-of-the-Art Results**: Competes effectively with contrastive methods on various image classification tasks.
- **Minimal Computational Overhead**: Optimized for efficiency during training.

<h3 align="center">BYOL Model Overview</h3>
<p align="center">
  <img src="https://raw.githubusercontent.com/deepmancer/byol-pytorch/main/images/Byol.jpg" width="600" alt="BYOL Model Architecture">
</p>

---

## 📊 Experimental Results

We evaluated our implementation using the **STL10 Dataset**, showcasing the impact of BYOL pretraining:

| **Training Method**      | **Accuracy** |
|---------------------------|--------------|
| Without Pretraining       | 84.58%       |
| With BYOL Pretraining     | **87.61%**   |

This demonstrates how BYOL can effectively enhance feature learning, even with relatively few epochs.

---

## 📁 Dataset: STL10

The **STL10 Dataset** is designed for unsupervised and self-supervised learning models, making it a perfect fit for BYOL.

- **Classes**: 10 categories, including animals and vehicles.
- **Train/Test Split**: 500 training images and 800 test images per class.
- **Source**: [STL10 Dataset](https://cs.stanford.edu/~acoates/stl10/)

<h3 align="center">STL10 Dataset Sample</h3>
<p align="center">
  <img src="https://cs.stanford.edu/~acoates/stl10/images.png" width="600" alt="STL10 Dataset Example">
</p>

---

## 🔧 Getting Started

### Prerequisites
- **Python 3.6+**
- **PyTorch**
- **Torchvision**
- **Jupyter Notebook** (for interactive experiments)

### Installation

Clone the repository and install the required dependencies

---

## 🧾 License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

---

## 📚 Citations

```bibtex
@inproceedings{NEURIPS2020_f3ada80d,
  author = {Grill, Jean-Bastien and Strub, Florian and Altch\'{e}, Florent and Tallec, Corentin and Richemond, Pierre and Buchatskaya, Elena and Doersch, Carl and Avila Pires, Bernardo and Guo, Zhaohan and Gheshlaghi Azar, Mohammad and Piot, Bilal and kavukcuoglu, koray and Munos, Remi and Valko, Michal},
  booktitle = {Advances in Neural Information Processing Systems},
  editor = {H. Larochelle and M. Ranzato and R. Hadsell and M.F. Balcan and H. Lin},
  pages = {21271--21284},
  publisher = {Curran Associates, Inc.},
  title = {Bootstrap Your Own Latent - A New Approach to Self-Supervised Learning},
  url = {https://proceedings.neurips.cc/paper_files/paper/2020/file/f3ada80d5c4ee70142b17b8192b2958e-Paper.pdf},
  volume = {33},
  year = {2020}
}
```
