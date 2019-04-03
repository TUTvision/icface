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
## Video

<iframe width="560" height="315" src="https://www.youtube.com/embed/VhWrAjI6z0M" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

> The training set contains 50 paired data out of total 2975 training images from this dataset.
> CycleGAN can only be trained on unpaired data and pix2pix can be trained on only 50 paired data.
> Our approach utilizes both paired and unpaired data to achive superior results.
![Bra](https://github.com/TUTvision/Learning-image-to-image-translation-using-paired-and-unpaired-training-samples/blob/master/com1.png?raw=true "Input Image")

### Satellite images to maps translation and vice versa
> The training set contains 50 paired data out of total 1096 training images from this dataset.
> Our approach produces better quality results with the help of small paired data cues.
![Bra](https://github.com/TUTvision/Learning-image-to-image-translation-using-paired-and-unpaired-training-samples/blob/master/comp2.png?raw=true "map Image")

## Translation using supervision across datasets
> The training set contains 2975 paired images from cityscapes dataset and 100 unpaired images from
Mapillary vistas dataset. All the models are tested on Mapillary vistas images that are
not involved in training.
> pix2pix is trained only on paired data (from cityscapes) and CycleGAN is trained only on unpaired data (from Mapillary vistas).
> Our model achives high quality results by utilizing both paired and unpaired data simultaneously and outperforms the state-of-the-art approaches.
![Bra](https://github.com/TUTvision/Learning-image-to-image-translation-using-paired-and-unpaired-training-samples/blob/master/comp3.png?raw=true "mapo Image")

```
#Citation 

@article{tripathy+kannala+rahtu,
  title={Learning image-to-image translation using paired and unpaired training samples},
  author={Tripathy, Soumya and Kannala, Juho and Rahtu, Esa},
  journal={arXiv preprint arXiv:1805.03189},
  year={2018}
}

```

```
Note: For the citations of the datasets and existing methods (e.g. cycleGAN, pix2pix) mentioned in this page, please refer to the paper: https://arxiv.org/abs/1805.03189. 
```
```
Related Work

1. Ian J. Goodfellow, Jean Pouget-Abadie, Mehdi Mirza, Bing Xu, David Warde-Farley, Sherjil Ozair, Aaron Courville, Yoshua Bengio "Generative Adversarial Networks", in NIPS 2014. 
2. Phillip Isola, Jun-Yan Zhu, Tinghui Zhou, and Alexei A. Efros. "Image-to-Image Translation with Conditional Adversarial Networks", in CVPR 2017.
3. J. Y. Zhu, T. Park, P. Isola, and A. A. Efros. "Unpaired image-to-image translation using cycle-consistent adversarial networks", In ICCV 2017.
```

![Octocat](https://github.com/TUTvision/Learning-image-to-image-translation-using-paired-and-unpaired-training-samples/blob/master/tut.jpeg?raw=true "tutImage")


