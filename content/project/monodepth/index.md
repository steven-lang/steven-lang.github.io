---
title: Unsupervised Monocular Depth Estimation using Atrous Convolutions
summary: Practical Course for Deep Learning in Computer Vision at TU Darmstadt
tags:
- Computer Vision
- Deep Learning
- Depth Estimation
date: "2019-03-01T00:00:00Z"


image:
  caption: 
  focal_point: Smart

links:
  - name: Code
    url: https://github.com/steven-lang/atrous-monodepth
url_pdf: "pdf/dlcv/report.pdf"
url_slides: "pdf/dlcv/presentation.pdf"
---

### Abstract

Monocular depth estimation is concerned with computing a dense depth map from a single image, but faces difficulties especially at object boundaries. Atrous convolutions have been successfully employed to this end in the task of semantic segmentation. In this paper we investigate, whether it is also possible to apply atrous convolutions in unsupervised monocular depth estimation. Specifically, we place an Atrous Spatial Pyramid Pooling block in a convolutional neural network between the encoder and decoder. This block allows for computing feature maps at different spatial scales on top of the encoder output. Our experiments show that atrous convolutions in the proposed setup do not improve depth estimation performance. Furthermore, the necessity of a lower output stride after the encoder, such that an increased receptive field size is even applicable, harms runtime and increases memory consumption. Finally, we show that it is possible to reduce the number of channels after the encoder, which reduces the parameter count without impairing predictions.

Project on *Unsupervised Monocular Depth Estimation Using Atrous Convolutions* in the Practical Course for Deep Learning in Computer Vision at TU Darmstadt.
