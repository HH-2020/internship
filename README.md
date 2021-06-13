# Introduction
During the internship in Fusic, I used [StyleGan2-ADA model](https://github.com/NVlabs/stylegan2-ada-pytorch) to perform the task of generating a smiley and expressionless image from a face image.
Here, I used the pre-train model based on FFHQ.

Two step were needed to complete this task.
1. Align the Picture as FFHQ dataset and project the image into the latent space.
2. Found the latent space for smile expression.

The first step could be done by the method mentioned in [stylegan2-projecting-images](https://github.com/woctezuma/stylegan2-projecting-images).
The second step was completed by difference of mean value of two latent space and SVM model(not be optimized).

The explantation for the model was described in [Fusic techblog](https://tech.fusic.co.jp/posts/2021-05-31-stylegan2-ada-face-smile-change/).
