# Self-Supervised Learning
* Self-supervised learning aims to learn a better feature space with. To achieve it, a pre-task should be defined for the dataset, where the pre-task is not related with the label, label-agnostic task. For example, delete one image patch and then predict the patch (image inpainting), randomly change the place of image patch and the pre-task is predicting the correct image patch location (jigsaw puzzle). In general, self-supervised learning is used in unlabled data, but also can be used in labeled dataset, or we can say the self-supervised learning does not think about the label.
* Paper list
  * 2015 ICCV Unsupervised Visual Representation Learning by Context Prediction
  * 2016 ECCV Unsupervised learning of visual representations by solving jigsaw puzzles
  * 2018 ICLR Unsupervised representation learning by predicting image rotations
  * 2019 CVPR Revisiting self-supervised visual representation learning
  * 2021 SiT Self-supervised vIsion Transformer
* Key issues
  * How to define a good pre-task
  * Self-supervised learning alone is far inferior to the supervised learning, but why and how can we improve it?
 
 # Semi-supervised learning
* Semi-supervised learning aims to use labeled data and unlabled data, different from only use labeled data or unlabeled data.
* Why we can use unlabled data? Theory guarantees the function.
* Taxonomy:
  *  Sequence to use the labeled data and unlabeled data: use labeled first, use unlabled first, use them at same time
* Survey Paper
  * 2021 A survey on semi-supervised learning
 
 ## Consistency Learning
 * The basic assumption behind the consistency learning is that we change the input a little, the output should be similar or same as we want to have a robust network. For example, adding gaussian noise to an image would not change the label of the image. So we use the consistency of output when changing the input a little bit to make a loss function. The consistency is also called as perturbation method in terms of the input.
 * Paper list
   * 2017 ICLR mixup Beyond Empirical Risk Minimization
   * 2017 Improved regularization of convolutional neural networks with cutout
   * 2019 ICCV CutMix Regularization Strategy to Train Strong Classifiers with Localizable Features
   * 2020 NIPS Unsupervised Data Augmentation for Consistency Training
* Questions
  * The difference between consistency learning and contrasting learning (metric learning).

## Self Training
* In general, self training tries to train a network in labeled data, then generate pseudo label for the unlabeled dataset, latter uses the pseudo label to train the network again, finnaly use the labeled data to train again (may iteratively do several times).
* Taxonomy
  * How many networks are used, single or many? (**Co-training** uses multiple networks.)
  * How many kinds of networks are used, only one or more than one (ensemble method).
* Key issues
  * How to generate pseduo label.
  * How to use the pseduo label dataset.
  * How to select the unlabeled dataset.
  * The stopping criteria.

## Pre-training
* Pre-training aims to learn a good feature space in the unlabeled dataset with unsupervised learning and then fintuning the learned network in the labeled dataset. In the fintuning stage, the feature extractor can be froozed and only the classifier is learned, or finetune both extractor and the classifier.
* Basic unsupervised learning algorithms can be leveraged.
  * Auto-encoder used the reconstruction loss.
  * Variants of auto-encoder, such as denoising auto-encoder.

## Data augmentation
