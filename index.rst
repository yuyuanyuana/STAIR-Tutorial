Welcome to STAIR's documentation!
=========================================

:Introduction: 

STAIR is a deep learning-based algorithm for Spatial Transcriptomic Alignment, Integration, and de novo 3D Reconstruction. STAIR utilizes heterogeneous graph attention network with spot-level and slice-level attention mechanisms to learn and integrate spatial features and obtain consistent spatial region divisions across slices. These results are then used to completes the 2D alignment. Unlike previous methods relying on known slice distance or known 3D coordinates, STAIR requires only ST data as input and infers the relative positioning of slices along z-axis in a completely unsupervised manner. In addition, STAIR seamlessly integrates new slices into the existing 3D atlas, effectively expanding the reference 3D atlas.

:Usage: 
.. toctree::
   :maxdepth: 1
   
   Installation
   1. Spatial feature integration of mouse olfactory bulb datasets
   2. 3D reconstruction of MERFISH mouse hypothalamic preoptic region
   3. 3D reconstruction of ST mouse brain
   4. Align new slices to the ABA brain atlas


:Citation: 
Yuanyuan Yu, Zhi Xie. Spatial Transcriptomic Alignment, Integration, and de novo 3D Reconstruction by STAIR, 08 February 2024, PREPRINT (Version 1) available at Research Square [https://doi.org/10.21203/rs.3.rs-3939678/v1]


