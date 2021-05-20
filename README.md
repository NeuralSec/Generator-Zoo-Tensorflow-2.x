# Generator-Zoo-Tensorflow-2.x
It is a growing pain for transfer learners working on tf2.x code. **The aim of this repo is to provide a collection of pretrained generators of various GANs for using in Tensorflow 2.x / Keras.** Welcome to contribute by including pretrained tf2.x GANs you discovered to this repo. 

Related repos:

https://github.com/POSTECH-CVLab/PyTorch-StudioGAN

https://github.com/rosasalberto/StyleGAN2-TensorFlow-2.x

#  Included GANs (generator only)

| Method | Venue | Architecture |
|:-----------|:-------------:|:-------------:|
| [**DCGAN**](https://arxiv.org/abs/1511.06434) | arXiv'15 | CNN/ResNet<sup>[[1]](#footnote_1)</sup> |
| [**WGAN-WC**](https://arxiv.org/abs/1701.04862) | ICLR'17 |  ResNet |
| [**SNGAN**](https://arxiv.org/abs/1802.05957) | ICLR'18 |  ResNet |
| [**BigGAN-Mod + DiffAug**](https://arxiv.org/abs/1809.11096) | ICLR'19 |  Big ResNet |
| [**StyleGAN2**](https://arxiv.org/abs/1912.04958) | CVPR'20 |  StyleGAN2 |

## Generators by Datasets
### Tiny ImageNet (64x64x3)

| Method | Reference | IS(⭡) | FID(⭣) | F_1/8(⭡) | F_8(⭡) | Weights / Keras.Model |
|:-----------|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:
| **DCGAN** | StudioGAN | 5.640 | 91.625 | 0.606 | 0.391 | [Link](https://drive.google.com/file/d/1f5Tti12gZ2lEvTQnTQND74pZNpxWqp0r/view?usp=sharing) |
| **WGAN-WC** | StudioGAN | 9.696 | 41.454 | 0.940 | 0.735 | [Link](https://drive.google.com/file/d/1E7afAqBenJWcgcuum0FyCIjugYC68TuD/view?usp=sharing) |
| **SNGAN** | StudioGAN | 8.412 | 53.590 | 0.900 | 0.703 | In converting |
| **BigGAN-Mod + DiffAug** | StudioGAN | 17.075 | 16.338 | 0.979 | 0.971 | [Link](https://drive.google.com/drive/folders/1cRcvUjGhkaZF-jK2tv6DOIKjZmhzEuE9?usp=sharing) |

### FFHQ (1024x1024x3)
| Method | Reference | IS(⭡) | FID(⭣) | F_1/8(⭡) | F_8(⭡) | Weights / Keras.Model |
|:-----------|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:|:-------------:
| **StyleGAN2** | https://github.com/rosasalberto/StyleGAN2-TensorFlow-2.x | N/A | N/A | N/A | N/A | [Link](https://drive.google.com/drive/folders/1_cfyqRl4G3oW5LT6Bnrp-crmAotyTlKE?usp=sharing) |
