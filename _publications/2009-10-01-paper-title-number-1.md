---
title: "Local Saliency-Guided Dynamic Matching for Cross-Modal Remote Sensing Image–Text Retrieval"
collection: publications
category: manuscripts
permalink: /publication/2009-10-01-paper-title-number-1
excerpt: 'This paper is about the number 1. The number 2 is left for future work.'
date: 2025-12-26
venue: '64'
# slidesurl: 'https://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://ieeexplore.ieee.org/document/11310837/'
bibtexurl: 'https://scholar.googleusercontent.com/scholar.bib?q=info:RDp3daCUlsYJ:scholar.google.com/&output=citation&scisdr=CoFwRCVrENySwE_Ln-g:AIVdB-wAAAAAaoXNh-hKG8Jkk9bITlar73DYPyQ&scisig=AIVdB-wAAAAAaoXNh7ZcMIZlLKVIc8FmEivxwPo&scisf=4&ct=citation&cd=-1&hl=zh-CN'
citation: 'Shao, J., Xie, Y., Wang, P., & Feng, G. (2025). Local Saliency-Guided Dynamic Matching for Cross-Modal Remote Sensing Image–Text Retrieval. IEEE Transactions on Geoscience and Remote Sensing, 64, 1-15.'
---
1. 针对现有CLIP仅依赖全局特征导致缺乏细粒度语义理解的问题，提出结合局部显著性特征提升遥文检索性能。
2. 创新性的提出先对文本显著特征提取，并以此作为语义先验，引导图像编码器生成细粒度视觉显著特征。
3. 如何利用不同粒度的特征，采用了跨粒度特征相似度对比损失优化现有CLIP的InfoNCE损失。
4. 现有KL散度由于非对称性导致检索性能变差，设计了一种基于JS散度的动态匹配损失。
5. 从流形角度出发，采用了图扩散的全局优化，设计了全局和局部双分支优化算法对检索结果进行后处理优化。
