# README: GNN Project Setup

This repository contains code for practicing graph neural networks (GNNs).

The code is based on [Officail PyTorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/get_started/colabs.html).

## Reference
- [A Gentle Introduction to Graph Neural Networks](https://distill.pub/2021/gnn-intro/)
- [PyTorch Official Colab and Tutorials](https://pytorch-geometric.readthedocs.io/en/latest/get_started/colabs.html)
- [Karen Medium](https://karenkaods.medium.com/邁向圖神經網絡gnn-part1-圖數據的基本元素與應用-c3856a7f729d)

## Environment Setup

This project is designed to work with **Python 3.11**, **PyTorch 2.4.0**, **PyTorch Geometric (PyG) 2.4.x**. The setup is compatible with both **V100** and **A100** GPUs.

### 1. Create a Conda Virtual Environment

```bash
conda create -n gnn python=3.11 -y
conda activate gnn
```

### 2. Install PyTorch(2.4.0) with CUDA 12.1

```bash
pip install torch==2.4.0 --index-url https://download.pytorch.org/whl/cu121
```

### 3. Install PyTorch Geometric (PyG) and Dependencies

```bash
pip install torch-geometric
pip install pyg_lib torch_scatter torch_sparse torch_cluster torch_spline_conv -f https://data.pyg.org/whl/torch-2.4.0+cu121.html
```

### 4. Install Additional Dependencies

```bash
pip install -r requirements.txt
```

## Verification
After installation, you can verify that PyTorch is using the GPU:

```python
python torch_version.py
```

## Notes
- Ensure that your NVIDIA driver is updated to **version 525+** to support CUDA 12.1.
- If you are running on a CPU-only system, replace `cu121` with `cpu` in the PyTorch installation command.

This setup ensures **full compatibility** with both **V100** and **A100**, maximizing stability and performance.

