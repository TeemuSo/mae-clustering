# MAE-clustering

This repository was created as a part of a coursework at Aalto University. It contains notebook that can be ran from Colab to reproduce the results. 

Abstract:

*The main goal of this study was to examine whether the self-attention patterns
between patches in a Masked Autoencoder (MAE) model could be utilized to
distinguish between objects within the same class. To answer this goal, we applied
various clustering techniques on the self-attentions of the MAE model using ran-
domly selected images that contained multiple instances of the same class. Our
objective was to qualitatively determine whether the self-attention patterns of the
MAE model could be used to identify differences between objects within the same
class. Our results revealed that the seventh attention head self-attentions contained
distinct clusters of attention for different objects within the same class if they were
not overlapping with each other. These findings suggest that the self-attentions of
MAE models trained through self-supervised masking may contain valuable knowl-
edge that can be distilled. However, further research is needed to fully understand
the capabilities and limitations of these methods.*

## Results

### The self-attentions of MAE

![The self-attentions of the last layer in the MAE model, clustered by attention head from 1
to 6, are visualized for three images with the number of clusters indicated. From top to bottom, the
number of clusters used is 7, 3, and 4, respectively](figures/final-last-first.png)
*The self-attentions of the last layer in the MAE model, clustered by attention head from 1
to 6, are visualized for three images with the number of clusters indicated. From top to bottom, the
number of clusters used is 7, 3, and 4, respectively*

![The self-attentions of the last layer in the MAE model, clustered by attention head from 7 to 12, are visualized for three images with the number of clusters indicated. From top to bottom, the
number of clusters used is 7, 3, and 4, respectively](figures/final-last-second.png)
*The self-attentions of the last layer in the MAE model, clustered by attention head from 7 to 12, are visualized for three images with the number of clusters indicated. From top to bottom, the
number of clusters used is 7, 3, and 4, respectively*

![Visualization of the self-attentions in the seventh attention head for the final layer. ](figures/head7-final.png)
*Visualization of the self-attentions in the seventh attention head for the final layer.*

### The self-attentions of DINO

![The last layer self-attentions clustered with attentions calculated with DINO. From top to
bottom, the number of clusters for each image used is 7, 3, and 4, respectively.](figures/last-self-dino.png)
*The last layer self-attentions clustered with attentions calculated with DINO. From top to
bottom, the number of clusters for each image used is 7, 3, and 4, respectively.*