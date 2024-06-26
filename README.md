# FG2024 - Visual Saliency Guided Gaze Target Estimation with Limited Labels
## Abstract
Current models of gaze target estimation can present excellent performance, but the success of these models relies on large-scale annotated datasets. In real-world applications, obtaining large amounts of labelled data is often impractical due to the high cost of annotation. Therefore, in this paper, we investigate a relatively unexplored problem and introduce a semi-supervised method for gaze target estimation, which uses a small number of labels without compromising performance. We achieve this by leveraging the visual saliency map, which has been widely used in previous gaze target estimation studies. More explicitly, unlike previous studies, we build a multi-task model which can learn visual saliency and gaze target simultaneously. To train this model, in the lack of real labels, we propose a method to generate pseudo labels by combining the state-of-the-art approaches for visual saliency estimation, object detection, and head pose estimation. First, we train the multi-task model with the pseudo labels. Then, to compensate for the information loss due to the lack of reliable annotation, we fine-tune the network using a small number of real labels. We validate the performance of our model by creating a set of baseline models for comparison on two publicly available datasets, namely, GazeFollow and VideoAttention. The experimental results show that our method achieves the best performance in semi-supervised settings, as well as a competitive performance as compared to the existing fully supervised models.

## Strucuture Overview
Gaze Target Estimator
![Gaze Target Estimator](pics/GE.png)
Pseudo-label generation
![Pseudo-label generation](pics/pl.png)
## Code
We use [SalGAN](https://github.com/imatge-upc/salgan) as our visual saliency estimator. Thanks!
