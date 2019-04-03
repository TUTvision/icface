---
layout: default
---
# Abstract

Image-to-image translation is a general name for a task where
an image from one domain is converted to a corresponding image in an-
other domain, given sufficient training data. Traditionally different ap-
proaches have been proposed depending on whether aligned image pairs
or two sets of (unaligned) examples from both domains are available for
training. While paired training samples might be difficult to obtain, the
unpaired setup leads to a highly under-constrained problem and inferior
results. In this paper, we propose a new general purpose image-to-image
translation model that is able to utilize both paired and unpaired training
data simultaneously. We compare our method with two strong baselines
and obtain both qualitatively and quantitatively improved results. Our
model outperforms the baselines also in the case of purely paired and un-
paired training data. To our knowledge, this is the first work to consider
such hybrid setup in image-to-image translation.
## Semantic maps to photo translation on cityscapes dataset

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


