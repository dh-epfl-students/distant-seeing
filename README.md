# Distant-Seeing
Applying Machine Vision Algorithms to Historical Scientific Images
![](figures/banner.png)

# Info
Student: Naël Dillenbourg\
Supervisors: Mihailescu Ion-Gabriel & Sidorenko Semion\
Year: 2023

# About
Part of the distant-seeing project, this repository uses object detection to localize key features in physics books illustrations. We then explore ways of analysing these features, by comparing their usage, the frequency of appearance and by comparing duplicates found in the work of other authors.

# Research summary
In this paper, we tested numerous models made for object detection before concluding that fine-tuning a model was a necessary step towards the analysis of features in physics books.
We compared various parameters to fine-tune to the best of our ability a model capable of extracting features from a large dataset of illustrations. We find that optimal performances should be reached by a model using a Unet++ architecture, with a resnext101_32x16d encoder, using Instagram encoder weights, a batch size of 32 and a distribution of illustrations containing features between $50\%$ and $33\%$ according to our tests. We then analysed several books and found no particular trends in the usage of hands throughout time in physics books but did seem to find trends regarding the usage of hands with specific chapters. We also found examples of reused engraving plates with hands as features in illustrations or redrawn illustrations across authors.
![](figures/plot_predication_page.png)
![](figures/cummulative_predictions.png)

# Installation and Usage
A conda environment was used to during this project. A dependencies list was compiled from this environment.
```
conda create --name env_distant_seeing --file \notebooks\env.txt
```
# License
distant-seeing - Naël Dillenbourg    
Copyright (c) 2023 EPFL    
This program is licensed under the terms of the GPL. 
