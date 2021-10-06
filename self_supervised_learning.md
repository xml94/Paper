# Semi-supervised learning
* Semi-supervised learning aims to use labeled data and unlabled data, different from only use labeled data or unlabeled data.
* Why we can use unlabled data? Theory guarantees the function.
* Taxonomy:
  *  Sequence to use the labeled data and unlabeled data: use labeled first, use unlabled first, use them at same time
  *  

## Self-Supervised Learning
* Self-supervised learning aims to learn a better feature space with the unlabled data. To achieve it, a pre-task should be defined for the unlabeled data, where the pre-task is not related with the label, label-agnostic task. For example, delete one image patch and then predict the patch (image inpainting), randomly change the place of image patch and the pre-task is predicting the correct image patch location (jigsaw puzzle).
* Paper list
 * 2015 ICCV Unsupervised Visual Representation Learning by Context Prediction
 * 2016 ECCV Unsupervised learning of visual representations by solving jigsaw puzzles
 * 2018 ICLR Unsupervised representation learning by predicting image rotations
 * 2019 CVPR Revisiting self-supervised visual representation learning
 * 2021 SiT Self-supervised vIsion Transformer

## Self training
## Pre-training
## Distillation learning
## Consistency training
## Data augmentation
