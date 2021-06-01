# Semantic Image Synthesis

Semantic image synthesis aims to produce image given semantic segmentation,
which can also be used by image editing and image manipulation.

## Related Applications
* **Image Editing** aims to change one thing's label or style.
* **Image Manipulation**


## Datasets
* COCO-Stuff
* ADE20K
* Cityscapes
* CelebAMask-HQ
* Flickr Landscapes (not public)
* Facades ()

## Evaluations
* FID
* mIoU
* Pixel Accuracy
* Human Evaluation
* Number of parameters

## Questions
* Those classes with little number of pixels are not as good as 
    those classes with many number of pixels
  
* 

## Related Papers
* 2018 CVPR High-Resolution Image Synthesis and Semantic Manipulation with Conditional GANs
    * Coarse-to-fine generator
    * Multi-scale discriminators
    * Using instance map and instance feature
* 2019 CVPR Semantic Image Synthesis with Spatially-Adaptive Normalization
    * Spatially adaptive normalization
    * Multimodal synthesis with VAE
    * Image-level Style Control
* 2020 CVPR SEAN Image Synthesis with Semantic Region-Adaptive Normalization
    * Region Style Encoder
    * Semantic Region Adaptive Normalization
    * Region-level Style Control
    
* 2021 ICLR You Only Need Adversarial Supervision for Semantic Image Synthesis
    * Segmentation based discriminator
        * Balance weight for classes according to the number of pixels
        * When training discriminator
            * Do semantic segmentation for real image
            * Do binary classification for fake image
        * When training generator
            * Do semantic segmentation for fake image
    * LabelMix Regularization
    * 3-D noise to achieve multimodal control