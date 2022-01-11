# Basic question before reading papers
* What is the domain adaptation and How to classify the domain adaptation??
* What is the classic application?
* What is the classic dataset?
* How to classify the method to do domain adaptation?
* What is the difference between source and target domain?


# Resources
## Videos
* 李宏毅 中文版 Youtube https://www.youtube.com/watch?v=8AKqH6V9kjE

## Survey papers
* Wang, Mei, and Weihong Deng. "Deep visual domain adaptation: A survey." Neurocomputing 312 (2018): 135-153.
* Wilson, Garrett, and Diane J. Cook. "A survey of unsupervised deep domain adaptation." ACM Transactions on Intelligent Systems and Technology (TIST) 11.5 (2020): 1-46.


# Taxonomy
## The class difference between the target and source domain
* Closed set domain adaptation
* Partial domain adaptation
* Open set domain adaptation

## How many do we know about the target domain, or what we can get when training our model
* many or few data with annotations (not unsupervised domain adaptation (UDA))
* many unlabeled data 
* few unlabeled data
* many labeled data for some classes but no labeled data for other classes
* without any data: 
  * Domain Generalization
  * Zero-shot domain adaptation

## How many target domains
* one source and one target domain
* one source but more than one target domain

## Can we access the source data during the target task training
* Source data available
* Source data free (privacy issue), but with the source trained model

# Paradigm of the algorithm
* Domain invariant feature learning
* Data transfer and then do the task, given a target data point, transfer it 
to its counterpart source data point, and then do the task (classification or object detection)

# Datasets
* VisDA: 
  * 链接： https://github.com/VisionLearningGroup/visda-2019-public
  * Six domains: real RGB, sketch, quick draw (edges), painting, clip art, info graph.
  * 17 classes.
* Office-31: Amazon, Webcam, DSLR
* Digits: MNIST, USPS, SVHN
* Office-10 + Caltech-10
* NYU: RGBD dataset, cross-modality adaptation
* CAM Vid: driving videos under different weathers, such as cloudy and sunny
* CDTD: city dataset in four domains, sunny, cloudy, night, rainy