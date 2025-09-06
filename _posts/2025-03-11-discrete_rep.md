---
layout: post
title: "Paper Reviews on Vector Quantization and Discrete Representation Learning"
date: 2025-03-11 12:00:00
description: A review of two key works on discrete representation learning and neural audio compression VQ-VAE and Encodec.
tags:
categories: paper-review
thumbnail: assets/img/paper_review/discrete_rep/slide1.png
images:
  compare: false
  slider: true
---


**Review of Two Papers on Discrete Representation Learning**  
- **Paper 1:** [Neural Discrete Representation Learning (VQ-VAE)](https://arxiv.org/abs/1711.00937)  
- **Paper 2:** [High Fidelity Neural Audio Compression (Encodec)](https://arxiv.org/abs/2210.13438)  

---

### 1. Neural Discrete Representation Learning (VQ-VAE)  
This paper introduces the **Vector Quantised-Variational AutoEncoder (VQ-VAE)**, a generative model that learns **discrete latent representations**. Unlike standard VAEs, VQ-VAE outputs discrete codes and learns the prior distribution, avoiding the problem of *posterior collapse*.  

The use of **vector quantization** ensures that latent codes remain meaningful even when paired with powerful autoregressive decoders. When combined with autoregressive priors, VQ-VAE enables high-quality generation across multiple domains, including images, video, and speech. Importantly, it also supports applications such as **speaker conversion** and **unsupervised phoneme discovery**, showing the broad utility of discrete representations.  

---

### 2. High Fidelity Neural Audio Compression (Encodec)  
This work presents **Encodec**, a state-of-the-art neural audio codec for real-time, high-fidelity compression. It uses a **streaming encoder-decoder architecture** with quantized latent space, trained end-to-end. Training is stabilized with a novel **loss balancer** that normalizes gradient contributions across objectives, improving convergence.  

Encodec employs a **multiscale spectrogram adversary** to reduce artifacts and lightweight Transformers to further compress the discrete representation by up to 40% while remaining faster than real-time. Extensive subjective and objective evaluations demonstrate superior performance over existing codecs across speech, music, and noisy conditions, at both 24 kHz and 48 kHz.  

---

### My Notes  
These two papers illustrate the evolution of **discrete representation learning** in audio:  
- **VQ-VAE** provided the foundation, showing how vector quantization can unlock powerful latent representations for generative modeling.  
- **Encodec** built upon this idea, applying quantized latents to practical **neural audio compression**, achieving both high fidelity and efficiency.  

Together, they highlight how discrete representations have become central to **modern audio modeling**, bridging unsupervised representation learning and real-world applications like neural codecs. The presentation slides are shared below.  

**Presentation Slides:** [Link to slides](https://docs.google.com/presentation/d/1sTcriwGd_zoZUB0Ge5Mhuwvbxzgozbm8GnE_-dCCGLQ/)


<swiper-container keyboard="true" navigation="true" pagination="true" pagination-clickable="true" pagination-dynamic-bullets="true" rewind="true">
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/discrete_rep/slide1.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/discrete_rep/slide2.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/discrete_rep/slide3.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/discrete_rep/slide4.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/discrete_rep/slide5.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/discrete_rep/slide6.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/discrete_rep/slide7.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/discrete_rep/slide8.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/discrete_rep/slide9.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/discrete_rep/slide10.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/discrete_rep/slide11.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/discrete_rep/slide12.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/discrete_rep/slide13.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/discrete_rep/slide14.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/discrete_rep/slide15.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/discrete_rep/slide16.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
</swiper-container>


