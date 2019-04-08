---
layout: default
---
# Abstract
This paper presents a generic face animator that is
able to control the pose and expressions of a given face image.
The animation is driven by human interpretable control signals
consisting of head pose angles and the Action Unit (AU) values.
The control information can be obtained from multiple sources
including external driving videos and manual controls. Due to the
interpretable nature of the driving signal, one can easily mix the
information between multiple sources (e.g. pose from one image
and expression from another) and apply selective post-production
editing. The proposed face animator is implemented as a two
stage neural network model that is learned in self-supervised
manner using a large video collection. The proposed Interpretable
and Controllable face reenactment network (ICface) is compared
to the state-of-the-art neural network based face animation
techniques in multiple tasks. The results indicate that ICface
produces better visual quality, while being more versatile than
most of the comparison methods. The introduced model could
provide a lightweight and easy to use tool for multitude of
advanced image and video editing tasks.
## ICface in action

<iframe width="800" height="515" src="https://www.youtube.com/embed/VhWrAjI6z0M" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## The Architecture of ICface

![](https://github.com/TUTvision/icface/blob/master/model_2-1.jpg?raw=true | width=500)
>The overall architecture of the proposed model (ICface)
for face animation. In the training phase, we select two frames
from the same video and denote them as source and driving
image. The generator G\_N takes the encoded source image and
neutral facial attributes (FA\_N ) as input and produces an image
representing the source identity with central pose and neutral
expression (neutral image). In the second phase, the generator
G\_A takes the encoded neutral image and attributes extracted
from the driving image (FA\_D ) as an input and produces an
image representing the source identity with desired attribute
parameters FA\_D . The generators are trained using multiple
loss functions implemented using the discriminator D (see
Section 3 for details). In addition, since the driving and
source images have the same identity, a direct pixel based
reconstruction loss can also be utilized. Note that this is
assumed to be true only during training and in the test case
the identities are likely to be different.

<!--## Translation using supervision across datasets
> The training set contains 2975 paired images from cityscapes dataset and 100 unpaired images from
Mapillary vistas dataset. All the models are tested on Mapillary vistas images that are
not involved in training.
> pix2pix is trained only on paired data (from cityscapes) and CycleGAN is trained only on unpaired data (from Mapillary vistas).
> Our model achives high quality results by utilizing both paired and unpaired data simultaneously and outperforms the state-of-the-art approaches.
![Bra](https://github.com/TUTvision/Learning-image-to-image-translation-using-paired-and-unpaired-training-samples/blob/master/comp3.png?raw=true "mapo Image")
-->
## Paper

<blockquote class="embedly-card"><h4><a href="https://arxiv.org/abs/1904.01909">ICface: Interpretable and Controllable Face Reenactment Using GANs</a></h4><p>This paper presents a generic face animator that is able to control the pose and expressions of a given face image. The animation is driven by human interpretable control signals consisting of head pose angles and the Action Unit (AU) values. The control information can be obtained from multiple sources including external driving videos and manual controls.</p></blockquote>
<script async src="//cdn.embedly.com/widgets/platform.js" charset="UTF-8"></script>

## Code 

Check for updates in my github page. 

<blockquote class="embedly-card"><h4><a href="https://github.com/Blade6570/icface">Blade6570/icface</a></h4><p>ICface: Interpretable and Controllable Face Reenactment Using GANs - Blade6570/icface</p></blockquote>
<script async src="//cdn.embedly.com/widgets/platform.js" charset="UTF-8"></script>

<!--<iframe width="360" height="315" src="https://arxiv.org/abs/1904.01909"></iframe> -->
```  
#Citation 

@article{tripathy+kannala+rahtu,
  title={ICface: Interpretable and Controllable Face Reenactment Using GANs},
  author={Tripathy, Soumya and Kannala, Juho and Rahtu, Esa},
  journal={arXiv preprint arXiv:1904.01909},
  year={2019}
}

```
<!--
```
Note: For the citations of the datasets and existing methods (e.g. cycleGAN, pix2pix) mentioned in this page, please refer to the paper: https://arxiv.org/abs/1805.03189. 
```
-->
```
Related Work
1. O. Wiles, A. S. Koepke, A. Zisserman "X2Face: A network for controlling face generation by using images, audio, and pose codes", in ECCV 2018.
2. Zhixin Shu, Mihir Sahasrabudhe, Alp Guler, Dimitris Samaras ,Nikos Paragios, Iasonas Kokkinos "Deforming Autoencoders: Unsupervised Disentangling of Shape and Appearance", in ECCV 2018.
3. Ian J. Goodfellow, Jean Pouget-Abadie, Mehdi Mirza, Bing Xu, David Warde-Farley, Sherjil Ozair, Aaron Courville, Yoshua Bengio "Generative Adversarial Networks", in NIPS 2014. 
```
## ICface in News

<blockquote class="embedly-card"><h4><a href="https://www.tal-mi-or.de/news/icface-gesichtsanimator">Video anderer Person als Vorlage</a></h4><p>Fritz Lang und der Kameramann Curt Courant bei Dreharbeiten [Foto: Georg Pahl, Quelle: Bundesarchiv/ Wikimedia Commons , Lizenz: CC BY-SA 3.0 de ] Wissenschaftler haben den Gesichtsanimator ICface entwickelt, mit dem ein Standbild einer Person durch eine Videoaufnahme von einer anderen Person mit den gleichen Gesichtsausdrücken und Haltungen animiert werden kann.</p></blockquote>
<script async src="//cdn.embedly.com/widgets/platform.js" charset="UTF-8"></script>

<!--<img src="https://github.com/TUTvision/icface/blob/master/logo_tau.png" width="288" height="158"> -->
![Octocat](https://github.com/TUTvision/icface/blob/master/logo_tau.png?raw=true | width=288)


