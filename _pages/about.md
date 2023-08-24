---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

Hello! I'm Md Mubtasim Ahasan, a recent graduate from Brac University with a BSc. degree in Computer Science and Engineering. During my undergraduate studies, I was advised by [Jannatun Noor](https://sites.google.com/site/jannatun0abigzero/home) and conducted research at the [C2SG Lab](https://www.researchgate.net/lab/Computing-for-Sustainability-and-Social-Good-C2SG-Lab-Jannatun-Noor). My research interests encompass a range of exciting areas, such as Computer Vision, Audio Processing and Analysis, Machine Learning for Healthcare, and Natural Language Processing.

<!-- I have published more than 2 papers at the top international AI conferences with total <a href='https://scholar.google.com/citations?user=DhtAFkwAAAAJ'>google scholar citations <strong><span id='total_cit'>Number+</span></strong></a> (You can also use google scholar badge <a href='https://scholar.google.com/citations?user=DhtAFkwAAAAJ'><img src="https://img.shields.io/endpoint?url={{ url | url_encode }}&logo=Google%20Scholar&labelColor=f6f6f6&color=9cf&style=flat&label=citations"></a>). -->


<!-- # 🔥 News
- *2022.02*: &nbsp;🎉🎉 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
- *2022.02*: &nbsp;🎉🎉 Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet.  -->

# 📝 Publications 

<!-- <div class='paper-box'><div class='paper-box-image'><div><div class="badge">CVPR 2016</div><img src='images/500x300.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Deep Residual Learning for Image Recognition](https://openaccess.thecvf.com/content_cvpr_2016/papers/He_Deep_Residual_Learning_CVPR_2016_paper.pdf)

**Kaiming He**, Xiangyu Zhang, Shaoqing Ren, Jian Sun

[**Project**](https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=DhtAFkwAAAAJ&citation_for_view=DhtAFkwAAAAJ:ALROH1vI_8AC) <strong><span class='show_paper_citations' data='DhtAFkwAAAAJ:ALROH1vI_8AC'></span></strong>
- Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
</div>
</div> -->

<!-- - [Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet](https://github.com), A, B, C, **CVPR 2020** -->

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">3ICT2022</div><img src='images/pub1.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

<b>Classification of Respiratory Diseases and COVID-19 from Respiratory and Cough Sounds</b>

<b><u>Md Mubtasim Ahasan</u></b>, Mohammad Fahim, Himadri Mazumder, Nur E Fatema, Sheikh Mustafizur Rahman, A. B. M.
Alim Al Islam and Jannatun Noor
<br>
[[LINK]](https://ieeexplore.ieee.org/document/9990866)    [[PDF]](https://drive.google.com/file/d/1CYJ0196lmB-4o5EdLg9BttYaXMlIfKbi/view)

- Implemented and compared numerous deep learning model architectures and training procedures, determining the optimum methodology for audio classification.

- Assessed and adapted various image processing techniques for audio feature extraction, enhancing classification models’ performance and robustness.
</div>
</div>

<!-- # 🎖 Honors and Awards
- *2021.10* Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
- *2021.09* Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet.  -->

# 📖 Educations
<!-- - *2019.06 - 2022.04 (now)*, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet.  -->
- *2018.01 - 2022.06*, Bachelor of Science in Computer Science and Engineering, [Brac University](https://www.bracu.ac.bd/), Dhaka, Bangladesh.

<!-- # 💬 Invited Talks
- *2021.06*, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. 
- *2021.03*, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet.  \| [\[video\]](https://github.com/) -->

# 💻 Experience
- *2021.01 - 2022.01*, Undergraduate Researcher, [C2SG Lab](https://www.researchgate.net/lab/Computing-for-Sustainability-and-Social-Good-C2SG-Lab-Jannatun-Noor), Dhaka, Bangladesh

# 📚 Projects
<div class='paper-box-text' markdown="1">
<b>Histopathological Image Classification using Deep Learning</b> [[LINK]](https://www.kaggle.com/code/mubtasimahasan/pathmnist-image-classification-cnnmodels-pytorch)

- Developed a deep learning-based medical image classification system, utilizing histological slides to effectively classify tumor tissues.
- Designed multiple Deep Convolutional Neural Network (DCNN) models, achieving high accuracy in classification.
</div>

<div class='paper-box-text' markdown="1">
<b>Resume Categorization System using Deep Learning</b> [[LINK]](https://github.com/mubtasimahasan/resume-categorization-bert-pytorch/)

- Implemented and trained a BERT model for domain-based automatic resume categorization, conducted category distribution analysis, and applied tokenization for text preprocessing.
- Built a python script for command line execution, facilitating bulk resume sorting into category folders and CSV file creation with resume filenames and associated categories.
</div>

<div class='paper-box-text' markdown="1">
<b>3D Printer Defect Detection using Deep Learning</b> [[LINK]](https://www.kaggle.com/code/mubtasimahasan/3d-printer-defect-detection-basicmodels-tensorflow)

- Built a computer vision-based deep learning classifier, efficiently detecting anomalies during 3d printing process.
- Implemented two Convolutional Neural Network (CNN) models, ensuring high accuracy and scalability.
</div>

<div class='paper-box-text' markdown="1">
<b>Breast Cancer Classification using Machine Learning</b> [[LINK]](https://www.kaggle.com/code/mubtasimahasan/breast-cancer-classification-and-model-comparison)

- Utilized and compared five machine learning models, including Logistic Regression, Decision Tree, Support Vector Machine (SVM), Multi-layer Perceptron Classifier (MLPClassifier), and Random Forest.
- Performed data pre-processing, Principal Component Analysis (PCA) and automatic features selection using scikit-learn library, reducing data complexity
</div>