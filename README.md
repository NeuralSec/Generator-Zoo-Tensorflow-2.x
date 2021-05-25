# Generator-Zoo-TensorFlow-2.x
It is a growing pain for transfer learners working under TF2.x to conduct few-shot learning/tuning on pretrained GANs. Beyond the fact that some pretrained generative models can be easily found for TF1.x and torch, I am amazed by how hard it is to have off-the-shelf generators to be used in TF2.x.

**The aim of this repo is to provide a collection of pretrained generators from various GANs for Tensorflow 2.x / Keras.** Welcome to contribute by adding pretrained tf2.x GANs you discovered to this repo. 

Related repos:

https://github.com/POSTECH-CVLab/PyTorch-StudioGAN

https://github.com/rosasalberto/StyleGAN2-TensorFlow-2.x

##  Included GANs (generator only)

| Method | Venue | Architecture |
|:-----------|:-------------:|:-------------:|
| [**DCGAN**](https://arxiv.org/abs/1511.06434) | arXiv'15 | CNN/ResNet<sup>[[1]](#footnote_1)</sup> |
| [**WGAN-WC**](https://arxiv.org/abs/1701.04862) | ICLR'17 |  ResNet |
| [**SNGAN**](https://arxiv.org/abs/1802.05957) | ICLR'18 |  ResNet |
| [**BigGAN-Mod + DiffAug**](https://arxiv.org/abs/1809.11096) | ICLR'19 |  Big ResNet |
| [**StyleGAN2**](https://arxiv.org/abs/1912.04958) | CVPR'20 |  StyleGAN2 |

## Pretrained Generators by Dataset
### Tiny ImageNet (64x64x3)
| Method | Reference | IS(⭡) | FID(⭣) | F_1/8(⭡) | F_8(⭡) | Weights / Keras.Model |
|:-----------|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:
| **DCGAN** | StudioGAN | 5.640 | 91.625 | 0.606 | 0.391 | [Keras.Model](https://drive.google.com/file/d/1f5Tti12gZ2lEvTQnTQND74pZNpxWqp0r/view?usp=sharing) |
| **WGAN-WC** | StudioGAN | 9.696 | 41.454 | 0.940 | 0.735 | [Keras.Model](https://drive.google.com/file/d/1E7afAqBenJWcgcuum0FyCIjugYC68TuD/view?usp=sharing) |
| **SNGAN** | StudioGAN | 8.412 | 53.590 | 0.900 | 0.703 | In converting |
| **BigGAN-Mod + DiffAug** | StudioGAN | 17.075 | 16.338 | 0.979 | 0.971 | [Weights](https://drive.google.com/drive/folders/1cRcvUjGhkaZF-jK2tv6DOIKjZmhzEuE9?usp=sharing) |

### ImageNet (128x128x3)
| Method | Reference | IS(⭡) | FID(⭣) | F_1/8(⭡) | F_8(⭡) | Weights / Keras.Model |
|:-----------|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:
| **SNGAN** | StudioGAN | 32.247 | 26.792 |	0.938 |	0.913 | [Keras.Model](https://drive.google.com/file/d/1p0TKswKj0sGse19ClyGr26aNJgLKKIw3/view?usp=sharing) |

### FFHQ (1024x1024x3)
| Method | Reference | IS(⭡) | FID(⭣) | F_1/8(⭡) | F_8(⭡) | Weights / Keras.Model |
|:-----------|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:
| **StyleGAN2** | [StyleGAN2-TensorFlow-2.x](https://github.com/rosasalberto/StyleGAN2-TensorFlow-2.x) | N/A | N/A | N/A | N/A | [Weights](https://drive.google.com/drive/folders/1_cfyqRl4G3oW5LT6Bnrp-crmAotyTlKE?usp=sharing) |

### FFHQ (256x256x3)
| Method | Reference | IS(⭡) | FID(⭣) | F_1/8(⭡) | F_8(⭡) | Weights / Keras.Model |
|:-----------|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:
| **BigGAN** | [U-Net GAN](https://github.com/boschresearch/unetgan) | N/A | N/A | N/A | N/A | [Weights](https://drive.google.com/drive/folders/1C1jUHs3RMOP1UW5IGBcYB20jaEMO-3ls?usp=sharing) |
