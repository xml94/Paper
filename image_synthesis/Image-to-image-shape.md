# Image Translation with Shape Changing

## Control

### Indirectly Control

   These algorithms hypothesize that the shapes can be changed if
   deep semantic information can be used.

### Directly Control, conditions is based on applications, 
   binary masks, attentions, landmarks and so on.
   
   * Two steps, shape change is independent on image translation, 
   but in the end we can combine the shape and translated image to
   a final translated image with shape change.

   * Integrated, couples (shape and image) to couples (shape and image).
   the changed shape and translated image are generated at same time.


## Background

* Global Translation: when change the object, we do not care
   about the background. The background can be changed.
   
* Local Translation: when translating object, we just want 
   to change the foreground, but we also want to keep the background.
   

## Questions

* If using GAN, how to let the discriminator check the alignment between
translated image and corresponding mask, landmarks if there is.
  
* Based on the applications, the marks of the shape are different.

* What results in shape change? What is the relation between the marks
and source image, translated image?