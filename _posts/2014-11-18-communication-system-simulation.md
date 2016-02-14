---
layout:     post
title:      Communication System Simulation
date:       2014-11-18 19:13:36
summary:    A basic communication system using MATLAB. It plots BER curves in order to compare the performance of several codification algorithms.
categories: research
tags:       [segmentation, english, research, evaluation, publication]
---

<p class="center"> [Github: Communication System Simulation](https://github.com/flandrade/communication-system-simulation)
</p>

This program simulates a basic communication system using MATLAB, and it plots BER curves in order to compare the performance of several codification algorithms. It includes the following components:

<img src="https://raw.githubusercontent.com/flandrade/communication-system-simulation/master/images/diagram.png" width="98%"/>

This simulation not only enables you to analyze to visualize signals, but it also obtains performance metrics such as probability of error (Pe) and bit error rate (BER). Several algorithms are available for quantization, modulation and codification.

__In case you're interested, I also implemented a [CDMA communication system](https://github.com/flandrade/cdma-simulation).__

### Quantization
- Uniform
- Mu-Law
- A-Law

### Modulation
- BPSK
- QPSK

### Codification
- Hamming (7,4)
- Convolutional codes: soft decision
- Convolutional codes: hard decision

### Graphs

<img src="https://raw.githubusercontent.com/flandrade/communication-system-simulation/master/images/graphs.jpg" width="98%"/>
