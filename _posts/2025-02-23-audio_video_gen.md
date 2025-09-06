---
layout: post
title: "Paper Reviews on Advances in Audio-Video Generation (VATT, AV-Link, Frieren)"
date: 2025-02-23 12:00:00
description: Review of three recent works on controllable video-to-audio generation, unified cross-modal diffusion, and flow-based approaches for audio synthesis from video.
tags: 
categories: paper-review
thumbnail: assets/img/paper_review/audio_video_gen/slide1.png
images:
  compare: false
  slider: true
---

**Review of Three Papers on Audio-Video Generation**  
- **Paper 1:** [Tell What You Hear From What You See (VATT)](https://arxiv.org/abs/2411.05679)  
- **Paper 2:** [AV-Link: Temporally-Aligned Diffusion Features for Cross-Modal Audio-Video Generation](https://arxiv.org/abs/2412.15191)  
- **Paper 3:** [Frieren: Efficient Video-to-Audio Generation Network with Rectified Flow Matching](https://arxiv.org/abs/2406.00320)  

---

### 1. VATT: Controllable Video-to-Audio Generation through Text
This work introduces **VATT**, a multi-modal generative framework for video-to-audio generation. Unlike prior methods that lack controllability, VATT incorporates an optional text prompt to guide audio generation. The system consists of two components: **VATT Converter**, a fine-tuned LLM that maps video features into the language space, and **VATT Audio**, a transformer that generates audio tokens from video frames (optionally conditioned on text). These tokens are decoded into waveforms using a pretrained neural codec.  

The framework supports both **text-guided video-to-audio generation** and **video-to-audio captioning**, enabling more controllable and interpretable outputs. Experiments show competitive results without captions, and significant improvements when captions are provided as guidance.  

---

### 2. AV-Link: Cross-Modal Audio-Video Generation
**AV-Link** proposes a unified framework for both video-to-audio and audio-to-video generation. It leverages activations from frozen diffusion models and introduces a **Fusion Block** that aligns modalities via temporally-aware self-attention.  

Unlike prior work that trains separate models for each direction, AV-Link handles both tasks within a single system, directly exchanging complementary audio and video features. Evaluations show that AV-Link achieves superior synchronization compared to existing baselines, including MovieGen, while remaining more efficient.  

---

### 3. Frieren: Efficient Video-to-Audio with Rectified Flow Matching
**Frieren** addresses efficiency and temporal alignment in video-to-audio generation. Built on **rectified flow matching**, it learns to map noise to spectrogram latents with straight paths and performs fast sampling through ODE solvers.  

The model uses a feed-forward transformer with channel-level cross-modal fusion for strong temporal alignment, achieving state-of-the-art results on **VGGSound**. Frieren also supports fast generation through reflow and one-step distillation, producing synchronized, high-quality audio in only a few steps. Experiments report 97.22% alignment accuracy and a 6.2% improvement in inception score over strong diffusion baselines.  

---

### My Notes
I presented these three papers at **CCDS, IUB**, where they sparked discussions on the future of **controllable**, **unified**, and **efficient** audio-video generation. VATT highlights the role of **text guidance**, AV-Link demonstrates **bidirectional cross-modal generation**, and Frieren shows how **efficiency and synchronization** can be achieved together. The presentation slides are shared below.  

**Presentation Slides:** [Link to slides](https://docs.google.com/presentation/d/17iT87GIMzCC-u5r-C51BOhbnk37YknIUGVoq1SNoHZE/)


<swiper-container keyboard="true" navigation="true" pagination="true" pagination-clickable="true" pagination-dynamic-bullets="true" rewind="true">
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide1.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide2.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide3.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide4.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide5.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide6.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide7.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide8.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide9.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide10.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide11.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide12.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide13.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide14.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide15.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide16.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide17.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide18.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide19.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide20.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide21.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide22.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide23.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide24.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide25.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide26.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide27.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide28.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide29.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide30.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide31.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide32.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide33.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide34.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading='eager' path='assets/img/paper_review/audio_video_gen/slide35.png' class='img-fluid rounded z-depth-1' %}</swiper-slide>
</swiper-container>
