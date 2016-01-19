---
layout:     post
title:      Novel Dataset for Interactive Segmentation Evaluation
date:       2015-07-25 18:32:52
summary:    A novel seed-based user input dataset that extends the well-known GrabCut dataset and the Geodesic Star convexity dataset.
categories: research
tags:       segmentation english
---

This dataset consists of 50 images, ground-truth data and two sets of _scribbles_, and it has been made publicly [available](http://sapyc.espe.edu.ec/segevaluation). As can be seen, the images contain an object that could be unambiguously extracted by users.

<img src="https://raw.githubusercontent.com/flandrade/flandrade.github.io/master/images/segmentation-01.jpg" width="49%"/> <img src="https://raw.githubusercontent.com/flandrade/flandrade.github.io/master/images/segmentation-08.jpg" width="49%"/>

For this compilation, the publicly available [GrabCut](http://research.microsoft.com/en-us/um/cambridge/projects/visionimagevideoediting/segmentation/grabcut.htm) and [Geodesic Star convexity dataset](http://www.robots.ox.ac.uk/~vgg/research/iseg/#Dataset) were taken as starting point. Original images and ground-truth data are from the GrabCut database.

<img src="https://raw.githubusercontent.com/flandrade/flandrade.github.io/master/images/segmentation-05.jpg" width="49%"/> <img src="https://raw.githubusercontent.com/flandrade/flandrade.github.io/master/images/segmentation-06.jpg" width="49%"/>

User inputs are provided by means of two sets of _scribbles_ which indicate foreground and background regions. For the first set, we use the _scribbles_ for initializing robot user from the Geodesic Star Convexit dataset. These employ on average about 4 strokes per image, yet they mark a small area of the foreground object. Finally, a new set of _scribbles_ was created in order to extend this dataset. In this set, the _scribbles_ indicate and mark in more detail the foreground region.

These sets reflect two degrees of user effort: the second set marks in more detail foreground regions when compared to the first set of _scribbles_.

__NOTE:__ _This note is the second of two notes. See the [presentation entry](http://flandrade.github.io/research/segmentation/english/2015/07/24/evaluation-interactive-image-segmentation-/) for more information._
