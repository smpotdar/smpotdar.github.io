---
layout: page
title: 3D Dense Reconstruction Using ICP and Point-based Fusion
description: In this project we implemented a 3D dense mapping system that reconstructs a 3D dense model with the given RGB-D image sequences.
img: /assets/img/icp_thumbnail.png
---

In this project we implemented a 3D dense mapping system that reconstructs a 3D dense model of a static indoor environment with given RGB-D image sequences.
The system follows the tracking and mapping framework proposed in [1], which is commonly used in many state-of-the-art
visual tracking and mapping systems. In this framework, mapping relies on the pose estimation from tracking to
update the global model, and tracking uses the refined global model from mapping as reference.

The visual tracking part of the system, which is also known as localization or visual odometry (VO), is solved using point-to-plane
iterative closest point (ICP) [2]. The mapping part is done using point-based fusion [1]. However, unlike in
[1], we did not consider the estimation of dynamic objects in this project since the input data are from a static
environment. 

The output of the system for a squence of RGBD is shown below:

<div class="container">
  <div class="row row-cols-1">
    <div class="col">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/icp_top.png' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/icp_front.png' | relative_url }}" alt="" title="example image"/>
    </div>
  </div>
</div>
<div class="caption">
    The top and front view of the fused point cloud along with the trajectory of the camera in red.
</div>


[1]: http://ieeexplore.ieee.org/document/6599048/

[2]: http://ieeexplore.ieee.org/document/6162880/