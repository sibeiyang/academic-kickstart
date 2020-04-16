---
title: "Ref-Reasoning"
authors:
- <font color=blue>Sibei Yang</font>
- Guanbin Li
- Yizhou Yu
date: "2020-04-01T00:00:00Z"

# Schedule page publish date (NOT publication's date).
publishDate: "2020-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent; 9=Dataset
publication_types: ["9"]

# Summary. An optional shortened abstract.
summary: Ref-Reasoning is a large-scale real-word dataset for referring expressions reasoning, which contains 791,956 referring expressions in 83,989 images. 

#tags:
#- Source Themes
featured: true

links:
- name: Expressions
  url: https://drive.google.com/drive/folders/1w4qhQgrgUeGOr_wG5KP0yUouMzRNBAxo?usp=sharing
- name: Object Features
  url: https://drive.google.com/drive/folders/10woLRXMEHuiqyMrikRGMiBGNqRqo81HH?usp=sharing
url_pdf: https://drive.google.com/file/d/1yogm2d5l49clAN3Hf4yZ5LMvi25WON8h/view?usp=sharing
url_project: https://github.com/sibeiyang/sgmn
#url_dataset: '#'
#url_poster: '#'
#url_slides: ''
#url_source: '#'
#url_video: '#'
---

Ref-Reasoning is a large-scale real-word dataset for grounding referring expressions, 
which contains 791,956 referring expressions in 83,989 images. It includes semantically rich expressions describing objects, attributes, direct relations and indirect relations with different reasoning layouts. 

![](/img/ref-reasoning_example.png)

## Images and Objects 
Ref-Reasoning is built on the scenes from the [GQA dataset](https://cs.stanford.edu/people/dorarad/gqa/about.html) and share the same [training images](https://nlp.stanford.edu/data/gqa/allImages.zip) with GQA. 
We generate referring expressions according to the [image scene graph annotations](https://nlp.stanford.edu/data/gqa/sceneGraphs.zip) provided by the [Visual Genome dataset](https://visualgenome.org/) and further normalized by the GQA dataset.
In oder to use the scene graphs for referring expression generation, we remove some unnatural edges and classes, e.g., "nose left of eyes". 
In addition, we add edges between objects to represent same-attribute relations between objects, i.e., "same material", "same color" and "same shape''. 
In total, there are 1,664 object classes, 308 relation classes and 610 attribute classes in the adopted scene graphs.

We provide the info and extracted visual features ([bottom-up features](https://github.com/peteanderson80/bottom-up-attention)) from Faster R-CNN for ground-truth objects in the images. 
The [gt_objects](https://drive.google.com/drive/folders/10woLRXMEHuiqyMrikRGMiBGNqRqo81HH?usp=sharing) contains:
    
  * The `gt_objects_info.json` is a dictionary from each image id to the info about the image and the image's index in the h5 file.
  * The `gt_objects_*.h5` includes objects' visual features and bounding boxes in pixels.

## Expressions and Referents
Ref-Reasoning has 721,164, 36,183 and 34,609 expression-referent pairs for training, validation and testing, respectively. 
In order to generate referring expressions with diverse reasoning layouts,
for each specified number of nodes, we design a family of referring expression templates for each reasoning layout.
We generate expressions according to layouts and templates using functional programs, 
and the functional program for each template can be easily obtained according to the layout. 
An example of a triplet of layout, template and functional program is shown as below. Please see more details in section 4 of the paper. 

![](/img/ref-reasoning_template.png)

In Ref-Reasoning [expressions](https://drive.google.com/drive/folders/1w4qhQgrgUeGOr_wG5KP0yUouMzRNBAxo?usp=sharing),
  * The `*_expressions.json` is a dictionary from each expression id to the info about the expression and its referent, 
  including image id, referent id, referent's bounding box in pixel, expression and the number of objects described by the expression.
  
## Citation
If you find the work useful in your research, please consider citing:

```
@inproceedings{yang2020graph-structured,
  title={Graph-Structured Referring Expressions Reasoning in The Wild},
  author={Yang, Sibei and Li, Guanbin and Yu, Yizhou},
  journal={Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition},
  year={2020}
}
```
