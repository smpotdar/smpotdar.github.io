---
layout: page
title: Image stitching using homographies
description: In this assignment, I performed stiched of two images by first finding correspondencies between the two images and estimating the planar homography transformation matrix between the two images.
img: assets/img/incline_mini.jpg
importance: 1
category: work
---

In this assignment, I implemented an interest point (keypoint) detector, a feature
descriptor and an image stitching tool based on feature matching and homography.

Interest point (keypoint) detectors find particularly salient points in an image. I
then extracted a feature descriptor that helped describe the region around each of the
interest points. I implemented the BRIEF feature descriptor in this homework. BRIEF has a compact
representation, is quick to compute, has a discriminative yet easily computed distance
metric, and is relatively simple to implement. This allows for real-time computation and it is also just as powerful as
more complex descriptors like SIFT for many cases.

After matching the features that were extracted, I estimated the relationship between the captured images 
using a 3 × 3 transformation matrix, called a planar homography.
A planar homography allows us to compute how a planar scene would look from a
second camera location, given only the first camera image. This allowed me to warp the second image
to perspective of the first image. This was followed by stiching of the images to get a beautiful panorama
of Pittsburgh

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/incline_L-min.png' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/incline_R-min.png' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    The view from two different camera poses.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/incline_pano.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    The final panorama after stitching.
</div>

