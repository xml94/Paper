Image translation with shape changing

## Control

1) Indirectly Control

These algorithms hypothesize that the shapes can be changed if
deep semantic information can be used.

2) Directly Control, conditions is based on applications, 
   binary masks, attentions, landmarks and so on.

a) two steps, shape change and image translation, then combine the 
shape and translated image.

b) integrated, couples (shape and image) to couples (shape and image)


## Background

1) global translation: when change the object, we do not care
   about the background. The background can be changed.
   
2) local translation: when translating object, we just want 
   to change the foreground, but we also want to keep the background.