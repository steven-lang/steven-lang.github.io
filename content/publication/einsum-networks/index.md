---
title: "Einsum Networks: Fast and Scalable Learning of Tractable Probabilistic Circuits"
authors:
- Robert Peharz
- Steven Lang
- Antonio Vergari
- Karl Stelzner
- Alejandro Molina
- Martin Trapp
- Guy Van den Broeck
- Kristian Kersting
- Zoubin Ghahramani

date: "2020-04-13T00:00:00Z"
# doi: "https://doi.org/10.1016/j.knosys.2019.04.013"

# Schedule page publish date (NOT publication's date).
publishDate: ""

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In *Proceedings of the 37th International Conference on Machine Learning (ICML)*
publication_short: In *ICML*

abstract: Probabilistic circuits (PCs) are a promising avenue for probabilistic modeling, as they permit a wide range of exact and efficient inference routines. Recent “deep-learning-style” implementations of PCs strive for a better scalability, but are still difficult to train on real-world data, due to their sparsely connected computational graphs. In this paper, we propose Einsum Networks (EiNets), a novel implementation design for PCs, improving prior art in several regards. At their core, EiNets combine a large number of arithmetic operations in a single monolithic einsum-operation, leading to speedups and memory savings of up to two orders of magnitude, in comparison to previous implementations. As an algorithmic contribution, we show that the implementation of Expectation-Maximization (EM) can be simplified for PCs, by leveraging automatic differentiation. Furthermore, we demonstrate that EiNets scale well to datasets which were previously out of reach, such as SVHN and CelebA, and that they can be used as faithful generative image models. 

# Summary. An optional shortened abstract.
summary: A novel approach to efficient Sum-Product Networks.
tags:
- Sum-Product Networks
- Probabilistic Circuits
- Einsum
featured: true

links:
 - name: Code
   url: https://github.com/cambridge-mlg/EinsumNetworks
 - name: Slides
   url: https://icml.cc/media/Slides/icml/2020/virtual(no-parent)-15-19-00UTC-6418-einsum_networks.pdf
 - name: Video
   url: https://slideslive.com/38928148
 - name: PDF
   url: http://proceedings.mlr.press/v119/peharz20a/peharz20a.pdf

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: ''
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
# projects:
# - internal-project

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example
---

<!-- {{% callout note %}} -->
<!-- Click the *Cite* button above to demo the feature to enable visitors to import publication metadata into their reference management software. -->
<!-- {{% /callout %}} -->

<!-- {{% callout note %}} -->
<!-- Create your slides in Markdown - click the *Slides* button to check out the example. -->
<!-- {{% /callout %}} -->

<!-- Supplementary notes can be added here, including [code, math, and images](https://wowchemy.com/docs/writing-markdown-latex/). -->
