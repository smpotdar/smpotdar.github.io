---
layout: page
title: ORB-SLAM using Multiple Cameras
description: In this project we made a Visual Simultaneous Localization and Mapping (VSLAM) system which integrates measurements from multiple cameras to achieve robust pose tracking and mapping.
img: assets/img/mc_orb_thumbnail.gif  
importance: 1
category: work
---

**_Abstract_** : Most of the autonomous systems such as self-
driving vehicles, autonomous aerial systems have multiple
cameras but typically use a single camera for SLAM. In this
project, we propose a different approach, where we present
a Visual Simultaneous Localization and Mapping (VSLAM)
system which integrates measurements from multiple cameras
to achieve robust pose tracking and mapping for these autonomous systems in unknown complex environments. The well-
known feature based ORB SLAM system has been extended
to work with three cameras in the final implementation. The
theory behind this system can easily be extended to multiple
camera configurations. We have implemented this and shown
experimental results on custom, KITTI, and the Argoverse
datasets.

A demo video of the project can be found by clicking on the image below

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        <a href="https://youtu.be/W9X_5pSzR-o"  target="_blank">
            <img class="img-fluid rounded z-depth-1" src="assets/img/slam_mc_orb.gif" alt="" title="example image"/>
        </a>
    </div>
</div>


For detailed information, please refer the paper.