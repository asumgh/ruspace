# ruspace
There is a repository of my 4d place solution for terraevolution competition.
Link: https://www.kaggle.com/c/roscosmos-rucode
Task: we have pairs of satellite images that contains such terrirory of forests. On two images in pair is shown the same region of Earth in different times. We need to recignize changes in landscape. For instance, fire or deforestation.
We have two 16-bit four-channel images, wich have shape approximately 1920x2000 pixels, with spatial resolution 10 meters for each.

My solution contains blending of two UnetPlusPlus models with different thresholds for predicted probability. On the one hand, first input is 1-dimension Gray Scale image, which is differense between two-times images, that was gray scaled and normalized. On the other hand, second input has another approach, which has firstly do normalization and secondly grayscaling images.
