# Image to Image Local

Image translation in local part is same with object transfiguration,
in which one image is split into two parts, foreground and background.
The foreground is desired to be translated but the background is desired
to be retained. If application gives the marks about the foreground
and the background, then it is a supervised learning or direct control.
Otherwise, it is a unsupervised learning or indirect control.

# Unsupervised Object Transfiguration
Attention mechanism is often employed to detect which part should be changed.
For example, attention is used to see which part is much different between 
two domains.

# Supervised Object Transfiguration
Binary masks, landmarks, and other markers are used to suggest where 
should be changed and where should be retained.