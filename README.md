# A Deep Journey into Super-resolution: A survey
This repository is for super-resolution survey introduced in the following paper

[Saeed Anwar](https://saeed-anwar.github.io/), [Salman Khan], [Nick Barnes], "A Deep Journey into Super-resolution: A survey", [[arXiv]](https://arxiv.org/abs/1904.07523) 


## Contents
1. [Introduction](#introduction)
2. [Overview](#overview)
3. [Datasets](#dataset)
4. [Results](#results)
5. [Ablation](#ablation)
6. [Citation](#citation)
7. [Acknowledgements](#acknowledgements)

## Introduction
Deep convolutional networks based super-resolution is a fast-growing field with numerous practical applications. In this exposition, we extensively compare 30+ state-of-the-art super-resolution Convolutional Neural Networks (CNNs) over three classical and three recently introduced challenging datasets to benchmark single image super-resolution. We introduce a taxonomy for deep-learning based super-resolution networks that groups existing methods into nine categories including linear, residual, multi-branch, recursive, progressive, attention-based and adversarial designs. We also provide comparisons between the models in terms of network complexity, memory footprint, model input and output, learning details, the type of network losses and important architectural differences (e.g., depth, skip-connections, filters). The extensive evaluation performed, shows the consistent and rapid growth in the accuracy in the past few years along with a corresponding boost in model complexity and the availability of large-scale datasets. It is also observed that the pioneering methods identified as the benchmark have been significantly outperformed by the current contenders. Despite the progress in recent years, we identify several shortcomings of existing techniques and provide future research directions towards the solution of these open problems.

![Overview](/Figs/Overview.PNG)
An overview of the existing single-image super-resolution techniques.

![Networks](/Figs/Net_archs.PNG)
A glimpse of diverse range of network architectures used for single-image super-resolution using deep networks.

## Datasets
We compare the state-of-the-art algorithms on publicly available benchmark datasets which include Set5, Set14, BSD100, Urban100, DIV2K and
Manga109.
![Images](/Figs/RepresentativeImages.PNG)
Representative test images from six super-resolution datasets used for comparing and evaluating algorithms

## Results
### Quantitative Results
![PSNR_SSIM_BI](/Figs/2xTable.PNG)
![PSNR_SSIM_BI](/Figs/3xTable.PNG)
![PSNR_SSIM_BI](/Figs/4xTable.PNG)
Mean PSNR and SSIM for the SR methods evaluated on the benchmark datasets. The ’-’ indicates that the method is not suitable to handle the
images of the corresponding dataset.

### Visual Results

![Visual_PSNR_SSIM_BI](/Figs/SRResults.PNG)
Super-resolution qualitative comparison for CNN-SR algorithms for 3x
![Visual_PSNR_SSIM_BI](/Figs/GAN.PNG)
Visual comparison for GAN-SR algorithms for 4x

## Ablation Studies
![PARAMETERS_TABLE](/Figs/parameters.PNG)
Parameters comparison of CNN-based SR algorithms. GRL stands for Global residual learning, LRL means Local residual learning, MST is
abbreviation of Multi-scale training.

![PARAMETERS_MULT_ADD](/Figs/mult_adds_comp.PNG)
Comparison of Multiplication-Addition operations in various SR networks. Note that FLOPs are roughly double the number of mult-adds.
Algorithmic runtime (during inference) is proportional to the multi-add operations.

![PARAMETERS_VS_PSNR](/Figs/params_comp.PNG)
Comparison of number of parameters in various SR architectures. The memory footprint and training time of the model is directly related
to the number of tunable parameters

## Citation
If you find the code helpful in your resarch or work, please cite the following papers.
```
@article{anwar2019deep,
  title={A Deep Journey into Super-resolution: A survey},
  author={Anwar, Saeed and Khan, Salman and Barnes, Nick},
  journal={arXiv preprint arXiv:1904.07523},
  year={2019}
}
```
## Acknowledgements


