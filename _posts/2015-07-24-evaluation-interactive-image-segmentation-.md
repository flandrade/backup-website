---
layout:     post
title:      Evaluation of seed-based Interactive Segmentation Algorithms
date:       2015-07-24 14:57:10
summary:    Despite some significant advances and extensive research, the selection of interactive segmentation algorithms is still a challenging task because people incorporate some semantic considerations that lead to more than one acceptable solution.
categories: research segmentation english
---

Extensive research has been conducted in an effort to evaluate methods and techniques for image segmentation. However, while most literature has focused on evaluating automatic and semi-automatic algorithms, works evaluating interactive segmentation algorithms are less numerous. Note that interactive segmentation can improve results by adding prior knowledge from users into the process. Although this user guidance improves segmentation results, it also makes difficult to conduct objective evaluations. For this reason, some works only present non-canonical evaluations.

In this paper, we present an objective and empirical evaluation of seed-based interactive segmentation algorithms. We first compare popular metrics that are employed in image-segmentation evaluations in order to define which one reflects most accurately the performance of segmentation algorithms. Then, in the aim of presenting reproducible results, we introduce a novel seed-based user input dataset that extends the well-known GrabCut dataset. In addition, we evaluate and contrast four state-of-the-art interactive segmentation algorithms. The analysis of the results demonstrates that Jaccard coefficient and Precision-Recall curves provide a good insight into the performance of the evaluated algorithms. Finally, the GrabCut algorithm presents the most robust and useful segmentation among all the evaluated algorithms.

## Dataset

[Dataset for Interactive Image Segmentation](http://sapyc.espe.edu.ec/segevaluation)

## Research Notes

* The Problem of Evaluating Interactive Segmentation
* Novel Dataset for Interactive Segmentation Evaluation
