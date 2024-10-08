# GNN Practice

This repository contains code for practicing graph neural networks (GNNs).

The code is based on [Officail PyTorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/get_started/colabs.html).

## References
- [A Gentle Introduction to Graph Neural Networks](https://distill.pub/2021/gnn-intro/)
- [PyTorch Official Colab and Tutorials](https://pytorch-geometric.readthedocs.io/en/latest/get_started/colabs.html)
- [Karen Medium](https://karenkaods.medium.com/邁向圖神經網絡gnn-part1-圖數據的基本元素與應用-c3856a7f729d)


## Installation

1. Install PyTorch (with CUDA 12.1) [(Official Doc)](https://pytorch.org/get-started/locally/)

```bash
conda install pytorch torchvision torchaudio pytorch-cuda=12.1 -c pytorch -c nvidia
```

2. Install PyTorch Geometric [(Official Doc)](https://pytorch-geometric.readthedocs.io/en/latest/install/installation.html)

```bash
pip install torch-geometric
```

3. Install Additional Libraries for GNN (Based on your environment)

```bash
pip install pyg_lib torch_scatter torch_sparse torch_cluster torch_spline_conv -f https://data.pyg.org/whl/torch-2.4.0+cu121.html
```

4. Install Other Packages

```bash
pip install -r requirements.txt
```

