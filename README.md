# HumanBodyOcclusionMaskEstimation

This project presents a method to estimate a mask for the occluded parts of human 
bodies depicted in an image, i.e. the occlusion mask. The estimation of the occlusion
mask plays an important role in many methods that address relevant problems of
machine vision and image synthesis such as, e.g. human pose estimation or human
de-occlusion. 

An accurate occlusion mask is also a requirement of synthesis methods
that replace human figures by 3D meshes in photos or videos such as in 3D-based
automatic image cartoonization. The method consists of three main steps: modal mask
extraction, 3D human body reconstruction and background inpainting. Modal mask
extraction is done with the [Binary People Segmentation](https://github.com/ternaus/people_segmentation) algorithm, the 3D
reconstruction is obtained using the [SMPLify-X](https://github.com/vchoutas/smplify-x) algorithm with [Openpose](https://github.com/CMU-Perceptual-Computing-Lab/openpose) for keypoints
detection and the inpainting is done with [Stable Diffusion](https://huggingface.co/stabilityai). As far as we know, this is the
first work focusing exclusively on this problem. The results obtained show that the
method is capable of obtaining accurate estimations of the occlusion masks, and it can
be successfully applied in automatic image cartoonization methods, such as [Pictonaut](https://github.com/rtous/pictonaut).

![alt text](https://github.com/snicolau/HumanBodyOcclusionMaskEstimation/blob/main/Diagram.jpg?raw=true)
