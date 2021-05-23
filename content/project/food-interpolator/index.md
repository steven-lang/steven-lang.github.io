---
title: GAN based Food Interpolation
summary: Project for the Deep Generative Models Course at the TU Darmstadt
tags:
- Deep Generative Models
- Generative Adverserial Models
date: "2020-01-14T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: 
  focal_point: Smart

url_slides: "pdf/deep-generative-models-food-interpolator.pdf"
url_code: "https://github.com/steven-lang/food-interpolator"
---

Deep Generative Models Course Project at TU Darmstadt.

## Goal
The main goal of this project is to learn a conditional GAN that can interpolate between different types of food. 
We want to achieve fluid transitions between e.g.:
- Burger <-> Pizza

## Data
- Scraped from google with [google-images-download](https://github.com/hardikvasa/google-images-download)
- Partly from [PizzaGAN](http://pizzagan.csail.mit.edu/)

## Results
Video results can be found [here](https://www.youtube.com/watch?v=LndGGbR4uxY&list=PLVCWvLHvDaenJrE2N-Akwo7-1kGN5vd5W).

### Progressive Growing (Video)
[<img src="https://img.youtube.com/vi/V7n1M14jKPM/hqdefault.jpg" width="50%">](https://youtu.be/V7n1M14jKPM)

### Pizza to Pizza (Video)
[<img src="https://img.youtube.com/vi/MSPZ56zy-OU/hqdefault.jpg" width="50%">](https://youtu.be/MSPZ56zy-OU)

### Burger to Burger (Video)
[<img src="https://img.youtube.com/vi/LndGGbR4uxY/hqdefault.jpg" width="50%">](https://youtu.be/LndGGbR4uxY)

### Random Latent Space (Video)
[<img src="https://img.youtube.com/vi/n0ucsR-ko60/hqdefault.jpg" width="50%">](https://youtu.be/n0ucsR-ko60)

## Code Base
The code is based on a [PyTorch implementation](https://github.com/jalola/improved-wgan-pytorch) of [Improved Training of Wasserstein GAN](https://arxiv.org/abs/1704.00028) and a [PyTorch implementation of Progressive Growing of GANs](https://github.com/jeromerony/Progressive_Growing_of_GANs-PyTorch)
