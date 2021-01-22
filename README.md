# Neural Style Transfer Improvement Method

### Intro

In this project, we implemented the neural style transfer based on existing study by [Gatys, etc](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Gatys_Image_Style_Transfer_CVPR_2016_paper.pdf). Briefly, Neural style transfer will take 3 images, a content image, a style image and an input image you want to style, then the style of style image will be transferred to the input image with content from content image. Our goal is to improve the transfer quality by adjusting intermediate layers used in content and style representations and discuss why certain layers are selected instead of others. An experimental model will be developed to compare with the baseline model that was designed by previous scholars. The performance of the models will be tested with respect of training iterations, random seeds and relative weight of content and style loss in the loss function.

### Input

Content images are:

![img](https://github.com/xinyi0351/STAT5242/blob/main/images/content1.jpg) | ![img](https://github.com/xinyi0351/STAT5242/blob/main/images/content2.jpg)

Style images are:

![img](https://github.com/xinyi0351/STAT5242/blob/main/images/style1.jpg)![img](https://github.com/xinyi0351/STAT5242/blob/main/images/style2.jpg)

The output printed with the final models are:

![img](https://github.com/xinyi0351/STAT5242/blob/main/images/final1.png)![img](https://github.com/xinyi0351/STAT5242/blob/main/images/final2.png)

![img](https://github.com/xinyi0351/STAT5242/blob/main/images/final3.png)![img](https://github.com/xinyi0351/STAT5242/blob/main/images/final4.png)

### Model Comparison 

|             | Running Time |  Total Loss   |                    Features                     |
| :---------: | :----------: | :-----------: | :---------------------------------------------: |
|  Baseline   |    111.73    |   1780934.4   |                    Smoother                     |
| Final Model |    23.38     | 1643762800.00 | With clearer structure and more saturated color |