---
title: "Evaluating the Robustness of a 4D STEM Autoencoder to Noisy Inputs"
collection: projects
type: "REU project"
permalink: /projects/robustness-of-scientific-ml
venue: "University of California, San Diego"
location: "La Jolla, CA, USA"
slidesurl: 'http://cecilia7717.github.io/files/poster1.pdf'
---

Evaluated the robustness of multiple neural network models to different levels of noise at the inputs and enhanced the robustness.

Overview
======

Material scientists use 4D Scanning Transmission Electron Microscopy (4D STEM) to extract
structural properties of materials by directing an electron beam through thin specimens. While
this process is invaluable, collecting more detailed data can damage the specimen, as it requires a
higher electron beam fluence. To mitigate this, researchers have proposed reducing the fluence,
which minimizes specimen damage but introduces significant noise into the data. Existing neural
network models, such as CC-ST-AE by Qin et al., aim to extract spatial parameters like strain
and rotation but struggle with noisy datasets. To address this, I investigated the robustness of
CC-ST-AE by training and testing it on 4D STEM data with varying levels of noise, analyzing
metrics like training/testing loss and angle prediction accuracy. My results showed that
injecting 25% noise during training caused a 35.48% drop in performance on noise-free data, but
improved performance on similarly noisy data, highlighting the model’s limited robustness to noise.
To improve this, I am implementing data augmentation with mixed noise levels, hyperparameter
tuning, and quantization techniques using the brevitas library. Future work will focus on
enhancing the model’s robustness through regularization, pruning, and exploring the capabilities
of robust quantized models.

