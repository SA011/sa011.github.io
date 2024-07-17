---
layout: page
title: Face Aging & De-Aging
description: A Deep Learning Project that uses Genarative Adverserial Network (GAN) and Cycle-GAN to Age or De-age
img: assets/img/face-de-aging.png
# redirect: https://github.com/SA011/FaceAging
importance: 1
category: work
visible: false
---
This project is a Deep Learning project on Computer Vision. It identifies image of a human page and tries to age or de-age it. It uses Generative Adverserial Network (GAN). It trains two model simultaneously (Generator Model and Discriminator Model). After completion of training, this model can be used to complete different tasks. Such that--
  - It can try to make a human face older or younger
  - It can try to detect whether the given image is a human face or not and if it's a human face whether it's older or younger.
  - We have also used age estimator which estimates the age of the given face image. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/face-de-aging.png" title="Example of Face-De-Aging" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/face-aging.png" title="Example of Face-Aging" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, we have 4 images of comparatively older people's images which have turned into a slightly younger image. On the right, we see the opposite.
</div>
