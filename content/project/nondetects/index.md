---
title: Non-detects in qPCR data
summary: Methods to model and impute non-detects in the results of qPCR experiments.
tags:
- qPCR
- nondetects
date: "2016-04-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: 
  focal_point: 

links:
#- icon: twitter
#  icon_pack: fab
#  name: Follow
#  url: https://twitter.com/georgecushen
url_code: "https://bioconductor.org/packages/release/bioc/html/nondetects.html"
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---

Quantitative real-time PCR (qPCR) proceeds via repeated cycles of sequence-specific DNA amplification followed by fluorescence measurements in which the fluorescence is proportional to the amount of target transcript present. The raw data produced by a qPCR experiment are fluorescence signal intensities measured at each amplification cycle. These data are used to estimate either relative or absolute expression of the target transcript.

Our group demonstrated that previous methods of handling non-detects often introduce substantial bias in estimates of differential gene expression. Specifically, we demonstrated that non-detects likely represent a specific type of missing data, called missing not at random, for which the probability of a missing value depends on unobserved data or the missing value itself. To address this, we developed an expectation- maximization (EM) algorithm in which we explicitly model the missing data mechanism. Finally, we showed that our method achieves a sizeable reduction in bias compared to previous methods.
