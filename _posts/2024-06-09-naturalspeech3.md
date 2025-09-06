---
layout: post
title: "Paper Review - NaturalSpeech 3: Zero-Shot Speech Synthesis with Factorized Codec and Diffusion Models"
date: 2024-06-09 11:30:00
description: 
tags: 
categories: paper-review
thumbnail: assets/img/paper_review/naturalspeech3/1.png
images:
  compare: false
  slider: true
---

**Review of the Paper: NaturalSpeech 3: Zero-Shot Speech Synthesis with Factorized Codec and Diffusion Models**  
**Paper Link:** [arXiv:2403.03100](https://arxiv.org/abs/2403.03100)

This paper presents an innovative approach to speech synthesis, specifically by introducing a codec model, FACodec, which disentangles speech representation into different subspaces. FACodec's architecture and capabilities particularly captured my attention, as it addresses key challenges in speech tokenization and effective speech representation disentanglement.

I presented this paper at CCDS, IUB, where I had thoughtful discussions with lab members and supervisors about its methodology and implications for advancing speech research. For those interested, I'm sharing the presentation slides below.

**Presentation Slides:** [Link to slides](https://docs.google.com/presentation/d/1qG2v2LouVBl9piZd3B2lXZh3WPCCu4yZ01uzOsfWgAI/)

<swiper-container keyboard="true" navigation="true" pagination="true" pagination-clickable="true" pagination-dynamic-bullets="true" rewind="true">
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/paper_review/naturalspeech3/1.png" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/paper_review/naturalspeech3/2.png" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/paper_review/naturalspeech3/3.png" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/paper_review/naturalspeech3/4.png" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/paper_review/naturalspeech3/5.png" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/paper_review/naturalspeech3/6.png" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/paper_review/naturalspeech3/7.png" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/paper_review/naturalspeech3/8.png" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/paper_review/naturalspeech3/9.png" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/paper_review/naturalspeech3/10.png" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/paper_review/naturalspeech3/11.png" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/paper_review/naturalspeech3/12.png" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/paper_review/naturalspeech3/13.png" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/paper_review/naturalspeech3/14.png" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/paper_review/naturalspeech3/15.png" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/paper_review/naturalspeech3/16.png" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/paper_review/naturalspeech3/17.png" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/paper_review/naturalspeech3/18.png" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/paper_review/naturalspeech3/19.png" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/paper_review/naturalspeech3/20.png" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/paper_review/naturalspeech3/21.png" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/paper_review/naturalspeech3/22.png" class="img-fluid rounded z-depth-1" %}</swiper-slide>
</swiper-container>
 