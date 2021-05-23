---
title: Deep Feature Interpolation
summary: Implementation of the Deep Feature Interpolation for Image Content Changes in TensorFlow
tags:
- TensorFlow
- Computer Vision
date: "2017-02-01T00:00:00Z"

image:
  caption: 
  focal_point: Smart

links:
 - name: Code
   url: https://github.com/steven-lang/dfi-tensorflow
url_slides: "pdf/deep-feature-interpolation.pdf"

math: true
---

### Description

Implementation of the Deep Feature Interpolation for Image Content Changes [paper](https://arxiv.org/abs/1611.05507) in tensorflow.

The goal is to add a specific target feature to the face of a person. This may be a Mustache or a smiling mouth. The procedure starts with taking `k` images of people with the feature and `k` images of people without the feature. These sets (positive/negative) are the input to an - on IMAGENET pretrained - VGG19 network. The output of each image is then fetched at the Relu layers of the third, fourth and fifth convolutional block. This builds a deep feature representation of an image. The deep feature vector of the target feature is then calculated by taking the difference of the mean of the positive and the negative set. To add the target feature to a new image, the target feature vector in the deep feature space will be added to the deep feature representation of this image. The image will then be restored by reverse mapping the deep feature values into the original pixel space, using an optimizer of your choice and the following loss function: 

$$
z = argmin_z \frac{1}{2}||\left(\phi\left(x\right) + \alpha w\right) - \phi \left( z \right)||_2^2 + \lambda\_{V^\beta} R\_{V^\beta}\left(z\right)
$$
$$
R\_{V^\beta}\left(z\right) = \sum\_{i,j}\left( \left(z\_{i,j+1} - z\_{i,j}\right)^2   + \left(z\_{i+1,j} - z\_{i,j}\right)^2 \right)
$$


Where $z$ is the new image, $x$ is the input image, $\phi$ is the mapping into deep feature space, $\alpha$ is a scalar and $w$ is the deep feature vector of the target feature.
