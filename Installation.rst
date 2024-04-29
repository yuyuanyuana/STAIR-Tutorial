Installation 
============

First, create and activate a virtual environment named STAIR-test:

```
conda create -n STAIR-test python=3.9.13
conda activate STAIR-test
```
Then, install the appropriate versions of PyTorch and PyG for your device. We will follow the [PyG tutorial](https://pytorch-geometric.readthedocs.io/en/latest/install/installation.html) and use CUDA 11.3 as an example:

```
pip install torch==1.12.1+cu113 torchvision==0.13.1+cu113 torchaudio==0.12.1 --extra-index-url https://download.pytorch.org/whl/cu113
```
Confirm that the installed PyTorch version is correct:
```
(STAIR-test)[yuyuanyuan@mu03 ~]$ python -c "import torch; print(torch.version)"
1.12.1+cu113
(STAIR-test)[yuyuanyuan@mu03 ~]$ python -c "import torch; print(torch.version.cuda)"
11.3
```
Next, install the corresponding PyG and its related packages:
```bash
pip install pyg_lib torch_scatter torch_sparse torch_cluster torch_spline_conv -f https://data.pyg.org/whl/torch-1.12.1+cu113.html
```

Finally, install the latest version of STAIR-tools via pip:

```
pip install STAIR-tools
```
To perform a complete STAIR analysis, in addition to the installation steps, you need to install the following software packages:
```
pip install anndata
pip install scanpy
pip install --user scikit-misc
conda install rpy2
conda install r-base=4.1.3
conda install conda-forge::r-mclust
pip install plotly
conda install bioconda::r-lisi
```

Then STAIR can be used in python:

.. code-block:: python

   import STAIR

Downloading STAIR code from https://github.com/yuyuanyuana/STAIR
