---
title: "Non-Local Context Encoder: Robust Biomedical Image Segmentation against Adversarial Attacks"
authors:
- Xiang He*
- <font color=blue>Sibei Yang*</font>
- Guanbin Li
- Haofeng Li
- Huiyou Chang
- Yizhou Yu (* co-first authors)
date: "2019-01-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2020-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In *Proceedings of the AAAI Conference on Artificial Intelligence (AAAI), 2019 Oral*
#publication_short: In *STC*

abstract: Recent progress in biomedical image segmentation based on deep convolutional neural networks (CNNs) has drawn much attention. However, its vulnerability towards adversarial samples cannot be overlooked. This paper is the first one that discovers that all the CNN-based state-of-the-art biomedical image segmentation models are sensitive to adversarial perturbations. This limits the deployment of these methods in safety-critical biomedical fields. In this paper, we discover that global spatial dependencies and global contextual information in a biomedical image can be exploited to defend against adversarial attacks. To this end, non-local context encoder (NLCE) is proposed to model short- and longrange spatial dependencies and encode global contexts for strengthening feature activations by channel-wise attention. The NLCE modules enhance the robustness and accuracy of the non-local context encoding network (NLCEN), which learns robust enhanced pyramid feature representations with NLCE modules, and then integrates the information across different levels. Experiments on both lung and skin lesion segmentation datasets have demonstrated that NLCEN outperforms any other state-of-the-art biomedical image segmentation methods against adversarial attacks. In addition, NLCE modules can be applied to improve the robustness of other CNN-based biomedical image segmentation methods.
# Summary. An optional shortened abstract.
summary: AAAI Conference on Artificial Intelligence (AAAI), 2019, <font color=blue>Oral Presentation</font>


#tags:
#- Source Themes
#featured: true

links:
#- name: Custom Link
#  url: http://example.org
url_pdf: https://arxiv.org/pdf/1904.12181.pdf
#url_code: '#'
#url_dataset: '#'
#url_poster: '#'
url_project: https://sibeiyang.github.io/publication/nlce
#url_slides: ''
#url_source: '#'
#url_video: '#'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
#image:
#  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
#  focal_point: ""
#  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
# projects:
# -

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example
header:
  image: "nlce.png"
---
