---
title: "Graph-Structured Referring Expressions Reasonig in The Wild"
authors:
- <font color=blue>Sibei Yang</font>
- Guanbin Li
- Yizhou Yu
date: "2020-04-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2020-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In *Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition (CVPR), 2020, Oral*
#publication_short: In *STC*

abstract: Grounding referring expressions aims to locate in an imge an object referred to by a natural language expression. The linguistic structure of a referring expression provides a layout of reasoning over the visual contents, and it is of- ten crucial to align and jointly understand the image and the referring expression. In this paper, we propose a scene graph guided modular network (SGMN), which performs reasoning over a semantic graph and a scene graph with neural modules under the guidance of the linguistic struc- ture of the expression. In particular, we model the image as a structured semantic graph, and parse the expression into a language scene graph. The language scene graph not only decodes the linguistic structure of the expression, but also has a consistent representation with the image se- mantic graph. In addition to exploring structured solutions to grounding referring expressions, we also propose Ref- Reasoning, a large-scale real-world dataset for structured referring expression reasoning. We automatically generate referring expressions over the scene graphs of images us- ing diverse expression templates and functional programs. This dataset is equipped with real-world visual contents as well as semantically rich expressions with different reason- ing layouts. Experimental results show that our SGMN1 not only significantly outperforms existing state-of-the-art algorithms on the new Ref-Reasoning dataset, but also surpasses state-of-the-art structured methods on commonly used benchmark datasets. It can also provide interpretable visual evidences of reasoning.
# Summary. An optional shortened abstract.
summary: IEEE Conference on Computer Vision and Pattern Recognition (CVPR), 2020, <font color=blue>Oral Presentation</font>

#tags:
#- Source Themes
featured: true

links:
#- name: Custom Link
#  url: http://example.org
url_pdf: https://drive.google.com/file/d/1yogm2d5l49clAN3Hf4yZ5LMvi25WON8h/view?usp=sharing
url_code: https://github.com/sibeiyang/sgmn/
url_dataset: https://sibeiyang.github.io/dataset/ref-reasoning
#url_poster: '#'
url_project: https://sibeiyang.github.io/publication/sgmn
#url_slides: ''
#url_source: '#'
#url_video: '#'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
#image:
  #caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
  #focal_point: ""
  #preview_only: false

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

header:
  image: "sgmn.png"
---

