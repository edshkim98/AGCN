# AGCN
**Adversarial Graph Convolutional Network for 3D point cloud segmentation**<br />

**Key Contributions:**<br />
1. We propose a novel neural network approach for 3D point cloud segmentation by using an adversarial learning scheme, where unlike previousworks, we present an embedding L2 loss as an adversarial loss to provide more informative feedback to segmentation network.
2. We introduce GeoEdgeConv as local feature aggregation method, which helps our network to efficiently and effectively learn complex local geometric structures.
3. We propose a smaller AGCN, AGCN-S, that achieves the smallest time complexity andsecond lowest space complexity compared to the SOTA, but still outperforming them.<br />

# Results<br />
**Instance Average IoU** <br />

PointNet++ | DGCNN | PointCNN | KPConv | Proposed witout Adv | Proposed with Adv
------------ | ------------- | ------------ | ------------- | ------------- | -------------
85.1 | 85.2 | 86.1 | 86.4 | 86.7 | **86.9** 

**Class Average IoU** <br />

PointNet++ | DGCNN | PointCNN | KPConv | Proposed witout Adv | Proposed with Adv
------------ | ------------- | ------------ | ------------- | ------------- | -------------
80.4 | 82.3 | 84.6 | 85.1 | 84.3 | **85.7** 

# Package Installation<br />
This code has been tested on: <br />
ubuntu <br />
torch == 1.7.1 <br />
torch-geometric == 1.7.0 <br />
torch-cluster == 1.5.9 <br />
torch-scatter == 2.0.6 <br />
torch-sparse == 0.6.9 <br />
torch-spline-conv == 1.2.1 <br />
open3d == 0.9.0 <br />
