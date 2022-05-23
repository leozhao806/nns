# NN-Steiner

Introduction
------
Code and Datasets for NN-Steiner: A Mixed Neural-algorithmic Approach for the Rectilinear Steiner Minimum Tree Problem


Dependencies
------

Python 3.7+

Pytorch 1.10.0+

DGL-CUDA

Geosteiner 5.1

CPLEX 12+

lp_solve 2.3+


Dataset
------
small: size 480 - 520

medium: size 1450 - 1550

large: size 2450 - 2550

They are generated randomly by utils.pointGeneration.py. Input parameters for small, medium, and large are (480, 520, 3000, 5), (1450, 1550, 3000, 5) and (2450, 2550, 3000, 5)

Usage
------
utils.geo_utils.py provides an interface for calling Geosteiner. 

eval = Evaluator(); rsmt = eval.gst_rsmt() # rectilinear steiner minimum tree; rmst = eval.gst_rmst() # rectilinear minimum spanning tree

/saved/nnsteiner500.pt provides a trained model

Call evaluate.py to load it.
