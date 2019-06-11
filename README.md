# A Deep Journey into Super-resolution: A survey
This repository is for super-resolution survey introduced in the following paper

[Saeed Anwar](https://saeed-anwar.github.io/), [Salman Khan], [Nick Barnes], "A Deep Journey into Super-resolution: A survey", [[arXiv]](https://arxiv.org/abs/1904.07523) 


## Contents
1. [Introduction](#introduction)
2. [Train](#train)
3. [Test](#test)
4. [Results](#results)
5. [Citation](#citation)
6. [Acknowledgements](#acknowledgements)

## Introduction
Deep convolutional networks based super-resolution is a fast-growing field with numerous practical applications. In this exposition, we extensively compare 30+ state-of-the-art super-resolution Convolutional Neural Networks (CNNs) over three classical and three recently introduced challenging datasets to benchmark single image super-resolution. We introduce a taxonomy for deep-learning based super-resolution networks that groups existing methods into nine categories including linear, residual, multi-branch, recursive, progressive, attention-based and adversarial designs. We also provide comparisons between the models in terms of network complexity, memory footprint, model input and output, learning details, the type of network losses and important architectural differences (e.g., depth, skip-connections, filters). The extensive evaluation performed, shows the consistent and rapid growth in the accuracy in the past few years along with a corresponding boost in model complexity and the availability of large-scale datasets. It is also observed that the pioneering methods identified as the benchmark have been significantly outperformed by the current contenders. Despite the progress in recent years, we identify several shortcomings of existing techniques and provide future research directions towards the solution of these open problems.

![CA](/Figs/CA.PNG)
Channel attention (CA) architecture.
![RCAB](/Figs/RCAB.PNG)
Residual channel attention block (RCAB) architecture.
![RCAN](/Figs/RCAN.PNG)
The architecture of our proposed residual channel attention network (RCAN).


### The whole test pipeline
1. Prepare test data.

    Place the original test sets (e.g., Set5, other test sets are available from [GoogleDrive](https://drive.google.com/drive/folders/1xyiuTr6ga6ni-yfTP7kyPHRmfBakWovo?usp=sharing) or [Baidu](https://pan.baidu.com/s/1yBI_-rknXT2lm1UAAB_bag)) in 'OriginalTestData'.

    Run 'Prepare_TestData_HR_LR.m' in Matlab to generate HR/LR images with different degradation models.
2. Conduct image SR. 

    See **Quick start**
3. Evaluate the results.

    Run 'Evaluate_PSNR_SSIM.m' to obtain PSNR/SSIM values for paper.



## Results
### Quantitative Results
![PSNR_SSIM_BI](/Figs/psnr_bi_1.PNG)
![PSNR_SSIM_BI](/Figs/psnr_bi_2.PNG)
![PSNR_SSIM_BI](/Figs/psnr_bi_3.PNG)
Quantitative results with BI degradation model. Best and second best results are highlighted and underlined

For more results, please refer to our [main papar](https://arxiv.org/abs/1807.02758) and [supplementary file](http://yulunzhang.com/papers/ECCV-2018-RCAN_supp.pdf).
### Visual Results
![Visual_PSNR_SSIM_BI](/Figs/fig1_visual_bi_x4.PNG)
Visual results with Bicubic (BI) degradation (4×) on “img 074” from Urban100


![Visual_PSNR_SSIM_BI](/Figs/fig5_visual_psnr_ssim_bi_x4.PNG)
![Visual_PSNR_SSIM_BI](/Figs/supp_fig1_visual_psnr_ssim_bi_x4_1.PNG)
![Visual_PSNR_SSIM_BI](/Figs/supp_fig1_visual_psnr_ssim_bi_x4_2.PNG)
![Visual_PSNR_SSIM_BI](/Figs/supp_fig1_visual_psnr_ssim_bi_x4_3.PNG)
Visual comparison for 4× SR with BI model

![Visual_PSNR_SSIM_BI](/Figs/fig6_visual_psnr_ssim_bi_x8.PNG)
Visual comparison for 8× SR with BI model

![Visual_PSNR_SSIM_BD](/Figs/fig7_visual_psnr_ssim_bd_x3.PNG)
Visual comparison for 3× SR with BD model

![Visual_Compare_GAN_PSNR_SSIM_BD](/Figs/supp_fig1_visual_compare_gan_psnr_ssim_bi_x4_1.PNG)
![Visual_Compare_GAN_PSNR_SSIM_BD](/Figs/supp_fig1_visual_compare_gan_psnr_ssim_bi_x4_2.PNG)
![Visual_Compare_GAN_PSNR_SSIM_BD](/Figs/supp_fig1_visual_compare_gan_psnr_ssim_bi_x4_3.PNG)
Visual comparison for 4× SR with BI model on Set14 and B100 datasets.
The best results are highlighted. SRResNet, SRResNet VGG22, SRGAN MSE, SR-
GAN VGG22, and SRGAN VGG54 are proposed in [CVPR2017SRGAN], ENet E and ENet PAT are
proposed in [ICCV2017EnhanceNet]. These comparisons mainly show the eﬀectiveness of our proposed
RCAN against GAN based methods

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


