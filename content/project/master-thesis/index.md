---
title: Oriented Object Detection using a One-Stage Anchor-Free Deep Model
summary: Master Thesis at the AIML Lab TU Darmstadt
tags:
- Deep Learning
- Computer Vision
- Oriented Object Detection
- Object Detection
date: "2021-05-13T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: 
  focal_point: Smart

url_pdf: "pdf/master-thesis/thesis.pdf" 
# url_code: TODO
url_slides: "pdf/master-thesis/pres.pdf"
---

Master Thesis at the TU Darmstadt in the AIML Lab supervised by [Prof. Kristian Kersting](https://ml-research.github.io/people/kkersting/index.html) and [Fabrizio Ventola](https://www.ml.informatik.tu-darmstadt.de/people/fventola/).

### Abstract

Object detection is a fundamental task in computer vision. While substantial
progress in the field of axis-aligned bounding-box detection has been made, it
suffers from poor performance on oriented objects, resulting in large parts of
the bounding box covering non-object related area. Therefore, the recent field
of oriented object detection has emerged, generalizing object detection to
arbitrary orientations which are commonly found in e.g. aerial view imagery or
security camera footage. This enables a tighter fit of bounding boxes, leading
to a better separation of bounding boxes especially in cases of dense object
distributions. In this work we present DAFNe: a Dense one-stage
Anchor-Free deep Network for oriented object detection. As one-stage model,
DAFNe performs predictions on a dense grid over the input image, being
architecturally simpler in design, as well as easier to optimize than their
two-stage alternatives. Being an anchor-free model, DAFNe additionally
reduces the prediction complexity by refraining from bounding box anchors
which come with many burdens: anchor specifications need more attentive
hyper-parameter fine-tuning on a per-dataset basis, increased model size and
computational overhead. Moreover, we introduce a novel vectorized corner
sorting algorithm to efficiently represent bounding boxes with a canonical
corner ordering batch-wise, an orientation-aware center-ness formulation for
arbitrary oriented bounding boxes to down-weight low-quality predictions, and
a center-to-corner bounding-box prediction strategy that improves object
localization performance. Our experiments show that DAFNe outperforms
all previous one-stage anchor-free models on DOTA 1.0, to the best of our
knowledge. DAFNe improves the prediction accuracy over the previous
best results by 4.65% mAP, setting the new state-of-the-art results by
achieving 76.95% mAP.
