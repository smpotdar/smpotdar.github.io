---
layout: page
title: 3D Reconstruction using RGB images
description: In this project, our task was to reconstruct an object in 3D using 3D rgb images.
img: assets/img/3dr_rgb_thumbnail.gif
importance: 1
category: work
---

In this project we implemented two different methods i.e. the 8-point algorithm and the 7-point algorithm to estimate
the fundamental matrix from corresponding points in two images. Given the fun-
damental matrix and calibrated intrinsics we computed the essential matrix and used it to compute a 3D metric reconstruction from 2D correspondences using triangulation.

The performance was evaluated on the Middlebury multi-view dataset.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/3dr_im1.png' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/3dr_im2.png' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    The view from two different camera poses.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/3dr_rgb.gif' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    Scatter plot of 3D points extracted from the above images.
</div>

