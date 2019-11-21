# A Deep Journey into Super-resolution: A survey
This repository is for super-resolution survey introduced in the following paper

[Saeed Anwar](https://saeed-anwar.github.io/), [Salman Khan], [Nick Barnes], "A Deep Journey into Super-resolution: A survey", [[arXiv]](https://arxiv.org/abs/1904.07523) 


## Contents
1. [Introduction](#introduction)
2. [Overview](#overview)
3. [Datasets](#datasets)
4. [Results](#results)
5. [Ablation](#ablation)
6. [Citation](#citation)
7. [Acknowledgements](#acknowledgements)

## Introduction
Deep convolutional networks based super-resolution is a fast-growing field with numerous practical applications. In this exposition, we extensively compare 30+ state-of-the-art super-resolution Convolutional Neural Networks (CNNs) over three classical and three recently introduced challenging datasets to benchmark single image super-resolution. We introduce a taxonomy for deep-learning based super-resolution networks that groups existing methods into nine categories including linear, residual, multi-branch, recursive, progressive, attention-based and adversarial designs. We also provide comparisons between the models in terms of network complexity, memory footprint, model input and output, learning details, the type of network losses and important architectural differences (e.g., depth, skip-connections, filters). The extensive evaluation performed, shows the consistent and rapid growth in the accuracy in the past few years along with a corresponding boost in model complexity and the availability of large-scale datasets. It is also observed that the pioneering methods identified as the benchmark have been significantly outperformed by the current contenders. Despite the progress in recent years, we identify several shortcomings of existing techniques and provide future research directions towards the solution of these open problems.

## Overview
![Overview](/Figs/Overview.png)
An overview of the existing single-image super-resolution techniques.

![Networks1](/Figs/Net1.PNG)
![Networks2](/Figs/Net2.PNG)
![Networks3](/Figs/Net3.PNG)

A glimpse of diverse range of network architectures used for single-image super-resolution using deep networks.

## Datasets
We compare the state-of-the-art algorithms on publicly available benchmark datasets which include Set5, Set14, BSD100, Urban100, DIV2K and
Manga109.
![Images](/Figs/RepresentativeImages.PNG)
Representative test images from six super-resolution datasets used for comparing and evaluating algorithms

## Results
### Quantitative Results
![PSNR_SSIM_2x](/Figs/2xTable.PNG)
![PSNR_SSIM_3x](/Figs/3xTable.PNG)
![PSNR_SSIM_4x](/Figs/4xTable.PNG)
Mean PSNR and SSIM for the SR methods evaluated on the benchmark datasets. The ’-’ indicates that the method is not suitable to handle the images of the corresponding dataset.

![PSNR_SSIM_8x](/Figs/8xTable.PNG)
The results for 8x Super-resolution.

### Visual Results

![Visual_PSNR_SSIM_BI](/Figs/Urban.PNG)
Super-resolution qualitative comparison for CNN-SR algorithms for 4x and 8x
![Visual_PSNR_SSIM_BI](/Figs/SR_GAN.PNG)
Visual comparison for GAN-SR algorithms for 4x

## Ablation
![PARAMETERS_TABLE](/Figs/parameters.PNG)

Parameters comparison of CNN-based SR algorithms. GRL stands for Global residual learning, LRL means Local residual learning, MST is
abbreviation of Multi-scale training.


<p align="center">
  <img width="500" src="https://github.com/saeed-anwar/SRsurvey/blob/master/Figs/mult_adds_comp.PNG">
</p>
Comparison of Multiplication-Addition operations in various SR networks. Note that FLOPs are roughly double the number of mult-adds.
Algorithmic runtime (during inference) is proportional to the multi-add operations.

<p align="center">
  <img width="500" src="https://github.com/saeed-anwar/SRsurvey/blob/master/Figs/params_comp.PNG">
</p>
Comparison of number of parameters in various SR architectures. The memory footprint and training time of the model is directly related to the number of tunable parameters.

## Citation
If you find the code helpful in your resarch or work, please cite the following papers.
```
@article{anwar2019deep,
  title={A Deep Journey into Super-resolution: A survey},
  author={Anwar, Saeed and Khan, Salman and Barnes, Nick},
  journal={arXiv preprint arXiv:1904.07523},
  year={2019}
}

@article{anwar2019drln,
  title={Densely Residual Laplacian Super-Resolution},
  author={Anwar, Saeed and Barnes, Nick},
  journal={arXiv preprint arXiv:1906.12021},
  year={2019}
}

```
## Acknowledgements


