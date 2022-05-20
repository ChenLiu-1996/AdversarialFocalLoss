# Adversarial Focal Loss

## TLDR
We proposed a generalizable adaptation of Focal Loss to keypoint detection leveraging difficulty scores from a discriminator. Under Review at NeurIPS 2022.

## Abstract
Focal Loss has reached incredible popularity as it uses a simple technique to identify and utilize hard examples to achieve better performance on classification.
However, this method does not easily generalize outside of classification tasks, such as in keypoint detection.
In this paper, we propose a novel adaptation of Focal Loss for keypoint detection tasks, called Adversarial Focal Loss (AFL).
AFL not only is semantically analogous to Focal loss, but also works as a plug-and-chug upgrade for arbitrary loss functions.
While Focal Loss requires output from a classifier, AFL leverages a separate adversarial network to produce a difficulty score for each input.
This difficulty score can then be used to dynamically prioritize learning on hard examples, even in absence of a classifier.
In this work, we show AFL's effectiveness in enhancing existing methods in keypoint detection and verify its capability to re-weigh examples based on difficulty.

