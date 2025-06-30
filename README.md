# Awesome Semantic Communication

**This is a resource list for Semantic Communication, including datasets, methods/codes/papers, metrics, blogs and so on.**

## Introduction

Semantic communication has drawn significant attention in recent years as a transformative approach to wireless communication. Unlike traditional systems that focus on transmitting raw data bits, semantic communication aims to convey the meaning of the data, making it particularly suitable for scenarios such as autonomous driving, smart cities, remote surgery, and human-AI interaction. However, realizing robust semantic communication remains a grand challenge due to issues such as task alignment, dynamic channel conditions, and the need for joint optimization across perception, language, and signal processing.

We hope this compilation can serve as a valuable reference for those developing advanced systems and exploring open challenges in semantic-aware information transmission.


## Table of Contents

- [Highlights](#highlights)
- [Datasets](#datasets)
- [Review and Benchmark](#Review-and-Benchmark)
- [Methods](#methods)
  * [Learning-based methods](#learning-based-methods)
  * [HE-based methods](#he-based-methods)
  * [Retinex-based methods](#retinex-based-methods)
  * [Other methods](#other-methods)
- [Related Works](#Related-Works)
- [Metrics](#metrics)
- [Blogs](#blogs)
- [Reference](#reference)



## Highlights

:high_brightness: <font color='red'> **News!** </font>

- Our new paper "[A mutually boosting dual sensor computational camera for high quality dark videography](https://linkinghub.elsevier.com/retrieve/pii/S1566253523000222)" based on RGB-NIR fusion have been published on **Infomation fusion**!
- Papers from **CVPR2022** have been updated!
- A new review article "Low-Light Image and Video Enhancement Using Deep Learning: A Survey" from **TPAMI** have been added!



## Datasets

|              Dataset              |                         Brief intro                          |                           Website                            |
| :-------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
|           VIP-LowLight            |  Eight Natural Images Captured in Very Low-Light Conditions  | [link](https://uwaterloo.ca/vision-image-processing-lab/research-demos/vip-lowlight-dataset) |
|              ReNOIR               | RENOIR - A Dataset for Real Low-Light Image Noise Reduction  | [link]([http://ani.stat.fsu.edu/~abarbu/Renoir.html](http://adrianbarburesearch.blogspot.com/p/renoir-dataset.html)) |
|    Raw Image Low-Light Object     |                              -                               |    [link](https://wiki.qut.edu.au/display/cyphy/Datasets)    |
|              **SID**              | Learning to see in the dark; <br />light level (outdoor scene 0.2 lux - 5 lux; indoor scene: 0.03 lux - 0.3 lux) |  [link](http://vladlen.info/publications/learning-see-dark)  |
|            **ExDARK**             | Getting to Know Low-light Images with The Exclusively Dark Dataset | [github](https://github.com/cs-chan/Exclusively-Dark-Image-Dataset) |
|          MIT-Adobe FiveK          | Learning Photographic Global Tonal Adjustment with a Database of Input / Output Image Pairs;<br />(with ~4% low light images) |      [link](https://data.csail.mit.edu/graphics/fivek)       |
|          LRAICE-Dataset           |   A Learning-to-Rank Approach for Image Color Enhancement    |                              -                               |
|         The 500px Dataset         |    Exposure: A White-Box Photo Post-Processing Framework     |                              -                               |
|               DPED                | DSLR-quality photos on mobile devices with deep convolutional networks |          [link](http://people.ee.ethz.ch/~ihnatova)          |
|              **LOL**              |     Deep Retinex Decomposition for Low-Light Enhancement     |      [link](https://daooshee.github.io/BMVC2018website)      |
|    VV - most challenging cases    | Busting image enhancement and tone-mapping algorithms: A collection of the most challenging cases;<br />from [Vassilios Vonikakis](https://sites.google.com/site/vonikakis/) | [link](https://sites.google.com/site/vonikakis/datasets/challenging-dataset-for-enhancement) |
|             VV - Phos             | A color image database of 15 scenes captured under different illumination conditions;<br />from [Vassilios Vonikakis](https://sites.google.com/site/vonikakis/) |        [link](http://robotics.pme.duth.gr/phos2.html)        |
|             **SICE**              | A large-scale multi-exposure image dataset, which contains 589 elaborately selected high-resolution multi-exposure sequences with 4,413 images |           [github](https://github.com/csjcai/SICE)           |
| The Extended Yale Face Database B | The extended Yale Face Database B contains 16128 images of 28 human subjects under 9 poses and 64 illumination conditions. | [link](http://vision.ucsd.edu/~iskwak/ExtYaleDatabase/ExtYaleB.html) |
|    the nighttime image dataset    | A dataset which contains source images in bad visibility and their enhanced images processed by different enhancement algorithms |              [link](http://mlg.idm.pku.edu.cn/)              |
|              VE-LOL               | A large-scale low-light image dataset serving both low/high-level vision with diversified scenes and contents as well as complex degradation in real scenarios, called Vision Enhancement in the LOw-Light condition (VE-LOL). |   [link](https://flyywh.github.io/IJCV2021LowLight_VELOL/)   |
|           SDSD dataset            | Seeing Dynamic Scene in the Dark: High-Quality Video Dataset with Mechatronic Alignment |       [github](https://github.com/dvlab-research/SDSD)       |
|                MID                | Matching in the Dark: A Dataset for Matching Image Pairs of Low-light Scenes |    [link](https://wenzhengchina.github.io/projects/mid/)     |
|       DeepHDRVideo-Dataset        | HDR Video Reconstruction: A Coarse-to-fine Network and A Real-world Benchmark Dataset |  [link](https://guanyingc.github.io/DeepHDRVideo-Dataset/)   |
|               LLVIP               | LLVIP: A visible-infrared paired dataset for low-light vision |         [link](https://bupt-ai-cz.github.io/LLVIP/)          |
|             RELLISUR              |  RELLISUR: A Real Low-Light Image Super-Resolution Dataset   |             [link](https://vap.aau.dk/rellisur/)             |
|               LSRW                | R2RNet: Low-light Image Enhancement via Real-low to Real-normal Network; <br />3170 paired images using the Nikon camera and 2480 paired images using the Huawei mobile phone. |    [github](https://github.com/abcdef2000/R2RNet#dataset)    |
|                MCR                | Mono-colored raw Paired dataset; <br />a dataset of colored raw and monochrome raw image pairs, captured with the same exposure setting. Each image has a resolution of 1280×1024. Totally 498 different scenes, each scene has 1 corresponding RGB and Monochrome ground truth and 8 different exposure color Raw inputs. | [Google Drive](https://drive.google.com/file/d/1_GWW1P1kjVBMFfN9AuaFq29w-kQ31ncd/view?usp=sharing) \| [Baidu Netdisk](https://pan.baidu.com/s/1b3cmUenebeDT_8HdLGa9dQ?from=init&pwd=22cv) |



## Review and Benchmark

| Year | Pub       | Paper                                                        | Link                                                         | Note       |
| :--: | --------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ---------- |
| 2021 | IJCV      | Benchmarking Low-Light Image Enhancement and Beyond          | [pdf](https://link.springer.com/article/10.1007%2Fs11263-020-01418-8) |            |
| 2021 | IEEE PAMI | Low-Light Image and Video Enhancement Using Deep Learning: A Survey | [pdf](https://doi.org/10.1109/TPAMI.2021.3126387)            |            |
| 2022 | ArXiv     | Low-Light Image and Video Enhancement: A Comprehensive Survey and Beyond | [pdf](http://arxiv.org/abs/2212.10772) [code](https://github.com/shenzheng2000/llie_survey) |            |
| 2023 | ArXiv     | DarkVision: A Benchmark for Low-Light Image/Video Perception | [pdf](https://arxiv.org/abs/2301.06269)                      | DarkVision |



## Methods

### Learning-based methods

| Year | Pub                     | Paper                                                        | Link                                                         | Note                 |
| ---- | ----------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | -------------------- |
| 2017 | ArXiv                   | MSR-net:Low-light Image Enhancement Using Deep Convolutional Network | [pdf](https://arxiv.org/pdf/1711.02488v1.pdf)                | MSR-net              |
| 2017 | ECCV                    | Deep Burst Denoising                                         | [pdf](http://arxiv.org/abs/1712.05790)                       |                      |
| 2017 | VCIP                    | LLCNN: A convolutional neural network for low-light image enhancement | [pdf](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8305143) [dataset](http://decsai.ugr.es/cvg/dbimagenes/) | LLCNN                |
| 2017 | Pattern Recognit.       | LLNet: A deep autoencoder approach to natural low-light image enhancement | [pdf](https://doi.org/10.1016/j.patcog.2016.06.008)          | LLNet                |
| 2017 | ACM Trans. Graph.       | Deep bilateral learning for real-time image enhancement      | [pdf](https://arxiv.org/abs/1707.02880) [web](https://groups.csail.mit.edu/graphics/hdrnet/) [code](https://github.com/google/hdrnet) | HDRNet               |
| 2017 | ICCV                    | DSLR-Quality Photos on Mobile Devices with Deep Convolutional Networks | [pdf](https://arxiv.org/abs/1704.02470)                      |                      |
| 2018 | BMVC                    | Deep Retinex Decomposition for Low-Light Enhancement         | [pdf](https://arxiv.org/abs/1808.04560) [web](https://daooshee.github.io/BMVC2018website/) [code](https://github.com/weichen582/RetinexNet) | Retinex-Net          |
| 2018 | BMVC                    | MBLLEN: Low-light Image/Video Enhancement Using CNNs         | [pdf](http://bmvc2018.org/contents/papers/0700.pdf) [web](http://phi-ai.org/project/MBLLEN/default.htm) [code](https://github.com/Lvfeifan/MBLLEN) | MBLLEN               |
| 2018 | Pattern Recognit. Lett. | LightenNet: A Convolutional Neural Network for weakly illuminated image enhancement | [pdf](https://doi.org/10.1016/j.patrec.2018.01.010)          | LightenNet           |
| 2018 | CVPR                    | Learning to See in the Dark                                  | [pdf](https://cchen156.github.io/paper/18CVPR_SID.pdf) [web](https://cchen156.github.io/SID.html) [code](https://github.com/cchen156/Learning-to-See-in-the-Dark.git) [dataset](https://github.com/cchen156/Learning-to-See-in-the-Dark) |                      |
| 2018 | IEEE TIP                | Learning a Deep Single Image Contrast Enhancer from Multi-Exposure Images | [pdf](https://doi.org/10.1109/TIP.2018.2794218) [code](https://github.com/csjcai/SICE) | SICE                 |
| 2018 | ACM TOG                 | Exposure: A White-Box Photo Post-Processing Framework        | [pdf](https://doi.org/10.1145/3181974) [code](https://github.com/yuanming-hu/exposure) |                      |
| 2018 | FG conference           | GLADNet: Low-Light Enhancement Network with Global Awareness | [pdf](https://github.com/daooshee/fgworkshop18Gladnet/blob/master/wwj_fg2018.pdf)  [web](https://daooshee.github.io/fgworkshop18Gladnet/) [code](https://github.com/weichen582/GLADNet) [dataset](https://daooshee.github.io/fgworkshop18Gladnet/) | GLADNet              |
| 2019 | IEEE TIP                | DeepISP: Towards Learning an End-to-End Image Processing Pipeline | [pdf](https://arxiv.org/abs/1801.06724)                      | DeepISP              |
| 2019 | IEEE TIP                | Low-Light Image Enhancement via a Deep Hybrid Network        | [pdf](https://ieeexplore.ieee.org/document/8692732)          |                      |
| 2019 | IEEE TIP                | EnlightenGAN: Deep Light Enhancement without Paired Supervision | [code](https://github.com/TAMU-VITA/EnlightenGAN) [pdf](https://arxiv.org/abs/1906.06972) | EnlightenGAN         |
| 2019 | ACM MM                  | Kindling the Darkness: A Practical Low-light Image Enhancer  | [pdf](http://arxiv.org/abs/1905.04161) [code](https://github.com/zhangyhuaee/KinD) [code+](https://github.com/zhangyhuaee/KinD_plus) | KinD                 |
| 2019 | IEEE Access             | A Pipeline Neural Network for Low-Light Image Enhancement    | [pdf](https://ieeexplore.ieee.org/document/8607964/)         |                      |
| 2019 | Neurocomputing          | Learning Digital Camera Pipeline for Extreme Low-Light Imaging | [pdf](https://arxiv.org/abs/1904.05939)                      |                      |
| 2019 | CVPR                    | Underexposed Photo Enhancement Using Deep Illumination Estimation | [pdf](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8953588) [code](https://github.com/wangruixing/DeepUPE) | DeepUPE              |
| 2019 | ICCV                    | Enhancing Low Light Videos by Exploring High Sensitivity Camera Noise | [pdf](https://ieeexplore.ieee.org/document/9011000)          |                      |
| 2019 | ICIP                    | Enhancement of Weakly Illuminated Images by Deep Fusion Networks | [pdf](https://ieeexplore.ieee.org/document/8803041)          |                      |
| 2019 | ICCP                    | A Bit Too Much? High Speed Imaging from Sparse Photon Counts | [pdf](https://ieeexplore.ieee.org/document/8747325/)         |                      |
| 2019 | ICIP                    | Llrnet: A Multiscale Subband Learning Approach for Low Light Image Restoration | [pdf](https://ieeexplore.ieee.org/document/8803765)          | Llrnet               |
| 2019 | ICIP                    | Low-Lightgan: Low-Light Enhancement Via Advanced Generative Adversarial Network With Task-Driven Training | [pdf](https://ieeexplore.ieee.org/document/8803328)          | Low-Lightgan         |
| 2019 | ICME                    | RDGAN: Retinex Decomposition Based Adversarial Learning for Low-Light Enhancement | [code](https://github.com/WangJY06/RDGAN/) [pdf](https://ieeexplore.ieee.org/document/8785047) | RDGAN                |
| 2019 | ICMEW                   | Low-Light Image Enhancement with Attention and Multi-level Feature Fusion | [pdf](http://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8794872) |                      |
| 2019 | PRCV                    | An Effective Network with ConvLSTM for Low-Light Image Enhancement | [pdf](https://doi.org/10.1007/978-3-030-31723-2_19)          |                      |
| 2019 | VISIGRAPP               | End-to-End Denoising of Dark Burst Images Using Recurrent Fully Convolutional Networks | [pdf](https://arxiv.org/abs/1904.07483v1)                    |                      |
| 2020 | CVPR                    | Zero-Reference Deep Curve Estimation for Low-Light Image Enhancement | [pdf](https://openaccess.thecvf.com/content_CVPR_2020/papers/Guo_Zero-Reference_Deep_Curve_Estimation_for_Low-Light_Image_Enhancement_CVPR_2020_paper.pdf) [web](https://li-chongyi.github.io/Proj_Zero-DCE.html) [code](https://github.com/Li-Chongyi/Zero-DCE) | Zero-DCE             |
| 2020 | CVPR                    | Learning to Restore Low-Light Images via Decomposition-and-Enhancement | [pdf](https://ieeexplore.ieee.org/document/9156446)          |                      |
| 2020 | CVPR                    | From Fidelity to Perceptual Quality: A Semi-Supervised Approach for Low-Light Image Enhancement | [pdf](http://openaccess.thecvf.com/content_CVPR_2020/papers/Yang_From_Fidelity_to_Perceptual_Quality_A_Semi-Supervised_Approach_for_Low-Light_CVPR_2020_paper.pdf) [web](https://github.com/flyywh/CVPR-2020-Semi-Low-Light) [slides](https://github.com/flyywh/CVPR-2020-Semi-Low-Light/blob/master) | DRBN                 |
| 2020 | CVPR                    | DeepLPF: Deep Local Parametric Filters for Image Enhancement | [pdf](https://arxiv.org/abs/2003.13985) [code](https://github.com/sjmoran/DeepLPF) | DeepLPF              |
| 2020 | IEEE PAMI               | Learning Image-adaptive 3D Lookup Tables for High Performance Photo Enhancement in Real-time | [pdf](https://ieeexplore.ieee.org/document/9206076) [code](https://github.com/HuiZeng/Image-Adaptive-3DLUT) | Image-Adaptive-3DLUT |
| 2020 | IET Image Proc.         | Learning an Adaptive Model for Extreme Low-Light Raw Image Processing | [pdf](https://arxiv.org/pdf/2004.10447.pdf) [code](https://github.com/505030475/ExtremeLowLight) |                      |
| 2020 | ArXiv                   | Visual Perception Model for Rapid and Adaptive Low-light Image Enhancement | [pdf](http://arxiv.org/abs/2005.07343) [code](https://github.com/MDLW/Low-Light-Image-Enhancement) |                      |
| 2020 | ArXiv                   | Self-supervised Image Enhancement Network: Training with Low Light Images Only | [pdf](https://arxiv.org/abs/2002.11300) [code](https://github.com/hitzhangyu/Self-supervised-Image-Enhancement-Network-Training-With-Low-Light-Images-Only) |                      |
| 2020 | ICPR                    | Unsupervised Real-world Low-light Image Enhancement with Decoupled Networks | [pdf](http://arxiv.org/abs/2005.02818)                       |                      |
| 2021 | IJCV                    | Attention Guided Low-Light Image Enhancement with a Large Scale Low-Light Simulation Dataset | [pdf](https://link.springer.com/10.1007/s11263-021-01466-8) [code](https://github.com/yu-li/AGLLNet) |                      |
| 2021 | CVPR                    | Retinex-Inspired Unrolling with Cooperative Prior Architecture Search for Low-Light Image Enhancement | [pdf](https://openaccess.thecvf.com/content/CVPR2021/papers/Liu_Retinex-Inspired_Unrolling_With_Cooperative_Prior_Architecture_Search_for_Low-Light_Image_CVPR_2021_paper.pdf) [web](http://dutmedia.org/RUAS/) [code](https://github.com/dut-media-lab/RUAS) | RUAS                 |
| 2021 | CVPR                    | Deep Denoising of Flash and No-Flash Pairs for Photography in Low-Light Environments | [pdf](https://openaccess.thecvf.com/content/CVPR2021/papers/Xia_Deep_Denoising_of_Flash_and_No-Flash_Pairs_for_Photography_in_CVPR_2021_paper.pdf) [code](https://github.com/likesum/deepFnF) |                      |
| 2021 | CVPR                    | Extreme Low-Light Environment-Driven Image Denoising over Permanently Shadowed Lunar Regions with a Physical Noise Model | [pdf](https://openaccess.thecvf.com/content/CVPR2021/papers/Moseley_Extreme_Low-Light_Environment-Driven_Image_Denoising_Over_Permanently_Shadowed_Lunar_Regions_CVPR_2021_paper.pdf) | HORUS                |
| 2021 | CVPR                    | Learning Temporal Consistency for Low Light Video Enhancement from Single Images | [pdf](https://openaccess.thecvf.com/content/CVPR2021/papers/Zhang_Learning_Temporal_Consistency_for_Low_Light_Video_Enhancement_From_Single_CVPR_2021_paper.pdf) [code](https://github.com/zkawfanx/StableLLVE) |                      |
| 2021 | CVPR                    | Nighttime Visibility Enhancement by Increasing the Dynamic Range and Suppression of Light Effects | [pdf](https://openaccess.thecvf.com/content/CVPR2021/papers/Sharma_Nighttime_Visibility_Enhancement_by_Increasing_the_Dynamic_Range_and_Suppression_CVPR_2021_paper.pdf) |                      |
| 2021 | ICCV                    | Seeing Dynamic Scene in the Dark: A High-Quality Video Dataset with Mechatronic Alignment | [pdf](https://openaccess.thecvf.com/content/ICCV2021/papers/Wang_Seeing_Dynamic_Scene_in_the_Dark_A_High-Quality_Video_Dataset_ICCV_2021_paper.pdf) [code](https://github.com/dvlab-research/SDSD) | SDSD                 |
| 2021 | ICCV                    | HDR Video Reconstruction: A Coarse-to-Fine Network and a Real-World Benchmark Dataset | [pdf](https://openaccess.thecvf.com/content/ICCV2021/papers/Chen_HDR_Video_Reconstruction_A_Coarse-To-Fine_Network_and_a_Real-World_Benchmark_ICCV_2021_paper.pdf) [web](https://guanyingc.github.io/DeepHDRVideo) [code](https://github.com/guanyingc/DeepHDRVideo) | DeepHDRVideo         |
| 2021 | ICCV                    | Matching in the Dark: A Dataset for Matching Image Pairs of Low-Light Scenes | [pdf](https://openaccess.thecvf.com/content/ICCV2021/papers/Song_Matching_in_the_Dark_A_Dataset_for_Matching_Image_Pairs_ICCV_2021_paper.pdf) [web](https://wenzhengchina.github.io/projects/mid/) [code](https://github.com/Wenzhengchina/Matching-in-the-Dark) | MID                  |
| 2021 | ICCV                    | Adaptive Unfolding Total Variation Network for Low-Light Image Enhancement | [pdf](https://openaccess.thecvf.com/content/ICCV2021/papers/Zheng_Adaptive_Unfolding_Total_Variation_Network_for_Low-Light_Image_Enhancement_ICCV_2021_paper.pdf) [code](https://github.com/CharlieZCJ/UTVNet/tree/5e76495bf371371a7fc63a521fb6dd9de35ee241) | UTVNet               |
| 2021 | ICCVW                   | LLVIP: A Visible-Infrared Paired Dataset for Low-Light Vision | [pdf](https://openaccess.thecvf.com/content/ICCV2021W/RLQ/papers/Jia_LLVIP_A_Visible-Infrared_Paired_Dataset_for_Low-Light_Vision_ICCVW_2021_paper.pdf) [code](https://github.com/bupt-ai-cz/LLVIP) [web](https://bupt-ai-cz.github.io/LLVIP/) | LLVIP                |
| 2021 | JVCIR                   | R2RNet: Low-Light Image Enhancement via Real-Low to Real-Normal Network | [pdf](http://arxiv.org/abs/2106.14501) [code](https://github.com/abcdef2000/R2RNet) | R2RNet               |
| 2022 | CVPR                    | Toward Fast, Flexible, and Robust Low-Light Image Enhancement | [pdf](https://openaccess.thecvf.com/content/CVPR2022/html/Ma_Toward_Fast_Flexible_and_Robust_Low-Light_Image_Enhancement_CVPR_2022_paper.html) [code](https://github.com/vis-opt-group/SCI) | SCI                  |
| 2022 | CVPR                    | Deep Color Consistent Network for Low-Light Image Enhancement | [pdf](https://openaccess.thecvf.com/content/CVPR2022/html/Zhang_Deep_Color_Consistent_Network_for_Low-Light_Image_Enhancement_CVPR_2022_paper.html) | DCC-Net              |
| 2022 | CVPR                    | URetinex-Net: Retinex-Based Deep Unfolding Network for Low-Light Image Enhancement | [pdf](https://openaccess.thecvf.com/content/CVPR2022/html/Wu_URetinex-Net_Retinex-Based_Deep_Unfolding_Network_for_Low-Light_Image_Enhancement_CVPR_2022_paper.html) [code](https://github.com/AndersonYong/URetinex-Net) | URetinex-Net         |
| 2022 | CVPR                    | Day-to-Night Image Synthesis for Training Nighttime Neural ISPs | [pdf](https://openaccess.thecvf.com/content/CVPR2022/html/Punnappurath_Day-to-Night_Image_Synthesis_for_Training_Nighttime_Neural_ISPs_CVPR_2022_paper.html) [code](https://github.com/SamsungLabs/day-to-night) |                      |
| 2022 | CVPR                    | SNR-Aware Low-Light Image Enhancement                        | [pdf](https://openaccess.thecvf.com/content/CVPR2022/html/Xu_SNR-Aware_Low-Light_Image_Enhancement_CVPR_2022_paper.html) [code](https://github.com/dvlab-research/SNR-Aware-Low-Light-Enhance) |                      |
| 2022 | CVPR                    | Dancing Under the Stars: Video Denoising in Starlight        | [pdf](https://openaccess.thecvf.com/content/CVPR2022/html/Monakhova_Dancing_Under_the_Stars_Video_Denoising_in_Starlight_CVPR_2022_paper.html) |                      |
| 2022 | CVPR                    | Abandoning the Bayer-Filter To See in the Dark               | [pdf](https://openaccess.thecvf.com/content/CVPR2022/html/Dong_Abandoning_the_Bayer-Filter_To_See_in_the_Dark_CVPR_2022_paper.html) [code](https://github.com/TCL-AILab/Abandon_Bayer-Filter_See_in_the_Dark) |                      |
| 2022 | ECCV                    | Unsupervised Night Image Enhancement: When Layer Decomposition Meets Light-Effects Suppression | [pdf](https://arxiv.org/pdf/2207.10564.pdf) [code](https://github.com/jinyeying/night-enhancement) |                      |
| 2022 | ECCV                    | Deep Fourier-Based Exposure Correction Network with Spatial-Frequency Interaction | [pdf](https://www.ecva.net/papers/eccv_2022/papers_ECCV/papers/136790159.pdf) [code](https://github.com/KevinJ-Huang/FECNet) |                      |
| 2022 | ECCV                    | LEDNet: Joint Low-Light Enhancement and Deblurring in the Dark | [pdf](https://link.springer.com/chapter/10.1007/978-3-031-20068-7_33) [code](https://github.com/sczhou/LEDNet) | LEDNet               |
| 2022 | AAAI                    | Low-Light Image Enhancement with Normalizing Flow            | [pdf](https://arxiv.org/pdf/2109.05923.pdf) [code](https://github.com/wyf0912/LLFlow) [web](https://wyf0912.github.io/LLFlow/) | LLFlow               |
| 2022 | AAAI                    | DarkVisionNet: Low-Light Imaging via RGB-NIR Fusion with Deep Inconsistency Prior | [pdf](https://doi.org/10.1609/aaai.v36i1.19995)              | DarkVisionNet        |
| 2022 | ACM MM                  | ChebyLighter: Optimal Curve Estimation for Low-Light Image Enhancement | [pdf](https://dl.acm.org/doi/10.1145/3503161.3548135) [code](https://github.com/eeerpjw/ChebyLighter)        | ChebyLighter         |
| 2022 | BMCV                    | You only need 90K parameters to adapt light: a light weight transformer for image enhancement and exposure correction | [pdf](https://bmvc2022.mpi-inf.mpg.de/0238.pdf) [code](https://github.com/cuiziteng/Illumination-Adaptive-Transformer) | IAT                  |
| 2022 | IJCV                    | Low-Light Image Enhancement via Breaking down the Darkness   | [pdf](http://dx.doi.org/10.1007/s11263-022-01667-9) [code](https://github.com/mingcv/Bread?utm_source=catalyzex.com) | Bread                |
| 2022 | Neurocomputing          | Low-Light Image Enhancement with Knowledge Distillation      | [pdf](https://doi.org/10.1016/j.neucom.2022.10.083)          |                      |
| 2022 | Neurocomputing          | LSR: Lightening Super-Resolution Deep Network for Low-Light Image Enhancement | [pdf](https://doi.org/10.1016/j.neucom.2022.07.058)          | LSR                  |
| 2022 | Pattern Recognit.       | Brain-like Retinex: A Biologically Plausible Retinex Algorithm for Low Light Image Enhancement | [pdf](http://dx.doi.org/10.1016/j.patcog.2022.109195)        |                      |
| 2022 | Pattern Recognit.       | LAE-Net: A Locally-Adaptive Embedding Network for Low-Light Image Enhancement | [pdf](http://dx.doi.org/10.1016/j.patcog.2022.109039)        | LAE-Net              |
| 2022 | Knowl-Based Syst        | LE-GAN: Unsupervised Low-Light Image Enhancement Network Using Attention Module and Identity Invariant Loss | [pdf](https://www.sciencedirect.com/science/article/pii/S0950705121011151) | LE-GAN               |
| 2022 | Opt. Lasers Eng.        | Infrared and Low-Light Visible Image Fusion Based on Hybrid Multiscale Decomposition and Adaptive Light Adjustment | [pdf](https://doi.org/10.1016/j.optlaseng.2022.107268)       |                      |
| 2022 | Applied Soft Computing  | A predictive intelligence approach for low-light enhancement | [pdf](https://linkinghub.elsevier.com/retrieve/pii/S1568494622004173) |                      |
| 2022 | IEEE TMM  | Purifying Low-light Images via Near-Infrared Enlightened Image | [pdf](https://ieeexplore.ieee.org/document/9999306/) |                      |
| 2023 | Information Fusion      | A Mutually Boosting Dual Sensor Computational Camera for High Quality Dark Videography | [pdf](https://doi.org/10.1016/j.inffus.2023.01.013) [code](https://github.com/jarrycyx/dual-channel-low-light-video-public) | DCMAN                |
| 2023 | Pattern Recognit.      | TreEnhance: A tree search method for low-light image enhancement | [pdf](https://www.sciencedirect.com/science/article/pii/S0031320322007282?via%3Dihub) [code](https://github.com/OcraM17/TreEnhance) | TreEnhance                |
| 2023 | AAAI                    | Ultra-high-definition low-light image enhancement: A benchmark and transformer-based method | [pdf](https://arxiv.org/abs/2212.11548) [code](https://github.com/TaoWangzj/LLFormer) [web](https://taowangzj.github.io/projects/LLFormer/) |                      |
| 2023 | AAAI                    | Low-Light Video Enhancement with Synthetic Event Guidance | [pdf](https://arxiv.org/abs/2208.11014) [code](https://gitee.com/mindspore/models/tree/master/research/cv/LLVE-SEG) |                      |


### HE-based methods

| Year | Pub      | Paper                                                        | Link                                                         | Note  |
| :--: | -------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ----- |
| 1990 | IEEE TCE | Contrast limited adaptive histogram equalization: speed and effectiveness | [pdf](https://ieeexplore.ieee.org/document/109340?arnumber=109340) | CLAHE |
| 2007 | IEEE TCE | Brightness Preserving Dynamic Histogram Equalization for Image Contrast Enhancement | [pdf](https://ieeexplore.ieee.org/document/4429280) [code](codes/bpdhe.m) | BPDHE |
| 2007 | IEEE TCE | A Dynamic Histogram Equalization for Image Contrast Enhancement | [pdf](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=4266947) | DHE   |
| 2007 | IEEE TCE | Fast Image/Video Contrast Enhancement Based on Weighted Thresholded Histogram Equalization | [pdf](https://ieeexplore.ieee.org/document/4266969?arnumber=4266969) | WTHE  |
| 2011 | IEEE TIP | Contextual and Variational Contrast Enhancement              | [pdf](http://ieeexplore.ieee.org/abstract/document/5773086/) | CVC   |
| 2013 | IEEE TIP | Contrast enhancement based on layered difference representation of 2D histograms | [pdf](http://mcl.korea.ac.kr/projects/LDR/2013_tip_cwlee_final_hq.pdf)  [web](http://mcl.korea.ac.kr/cwlee_tip2013/) | LDR   |
| 2013 | ICASSP   | High efficient contrast enhancement using parametric approximation | [pdf](http://150.162.46.34:8080/icassp2013/pdfs/0002444.pdf) | POHE  |


- **See also: [link](https://github.com/elliestath/HelpTest/blob/c7e269239a9d67bffc60f44ff1cae70d20770748/docs/Image%20Preprocessing.md)**



### Retinex-based methods

| Year | Pub                    | Paper                                                        | Link                                                         | Note  |
| ---- | ---------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ----- |
| 1997 | IEEE TIP               | Properties and performance of a center/surround retinex      | [pdf](https://ieeexplore.ieee.org/document/557356)           | SSR   |
| 1997 | IEEE TIP               | A multiscale retinex for bridging the gap between color images and the human observation of scenes | [pdf](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=597272) [code1](http://www.ipol.im/pub/art/2014/107/) [code2](https://github.com/upcAutoLang/MSRCR-Restoration) | MSRCR |
| 2013 | SITIS                  | Adaptive Multiscale Retinex for Image Contrast Enhancement   | [code](codes/amsr.m) [pdf](https://doi.ieeecomputersociety.org/10.1109/SITIS.2013.19) | AMSR  |
| 2013 | IEEE TIP               | Naturalness Preserved Enhancement Algorithm for Non-Uniform Illumination Images | [pdf](https://ieeexplore.ieee.org/document/6512558) [web](https://shuhangwang.wordpress.com/2015/12/14/naturalness-preserved-enhancement-algorithm-for-non-uniform-illumination-images/) [code](https://www.dropbox.com/s/096l3uy9vowgs4r/Code.rar) | NPE   |
| 2015 | IEEE TIP               | A Probabilistic Method for Image Enhancement With Simultaneous Illumination and Reflectance Estimation | [pdf](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=7229296) [code](codes/PM_SIRE.zip) | SRIE  |
| 2016 | CVPR                   | A Weighted Variational Model for Simultaneous Reflectance and Illumination Estimation | [pdf](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Fu_A_Weighted_Variational_CVPR_2016_paper.pdf)  [code](codes/WV_SIRE.zip) | SRIE  |
| 2016 | Signal Processing      | A fusion-based enhancing method for weakly illuminated images | [pdf](https://doi.org/10.1016/j.sigpro.2016.05.031) [code](codes/MF.rar) | MF    |
| 2016 | ACM MM                 | LIME: A Method for Low-light Image Enhancement               | [pdf](https://arxiv.org/pdf/1605.05034.pdf ) [web](https://sites.google.com/view/xjguo/lime) [code](https://drive.google.com/file/d/0BwVzAzXoqrSXb3prWUV1YzBjZzg/view) | LIME  |
| 2017 | IEEE TIP               | LIME: Low-Light Image Enhancement via Illumination Map Estimation | [pdf](http://ieeexplore.ieee.org/document/7782813/) [code1](https://github.com/Sy-Zhang/LIME) [code2](https://github.com/estija/LIME) [code3](https://github.com/pvnieo/Low-light-Image-Enhancement) | LIME  |
| 2017 | ICCV                   | A Joint Intrinsic-Extrinsic Prior Model for Retinex          | [pdf](http://caibolun.github.io/papers/JieP.pdf) [web](http://caibolun.github.io/JieP/) [code](https://github.com/caibolun/JieP/) | JieP  |
| 2018 | IEEE TIP               | Structure-Revealing Low-Light Image Enhancement Via Robust Retinex Model | [pdf](https://www.microsoft.com/en-us/research/uploads/prod/2018/04/2018-TIP-Structure-Revealing-Low-Light-Image-Enhancement-Via-Robust-Retinex-Model.pdf) [code1](https://github.com/martinli0822/Low-light-image-enhancement)  [code2](codes/robustRetinex.m) |       |
| 2018 | Symmetry               | A Smart System for Low-Light Image Enhancement with Color Constancy and Detail Manipulation in Complex Light Environments | [pdf](https://www.mdpi.com/2073-8994/10/12/718/pdf)          |       |
| 2019 | Symmetry               | Fractional-Order Fusion Model for Low-Light Image Enhancement | [pdf](https://www.mdpi.com/2073-8994/11/4/574/pdf)           |       |
| 2019 | ICIP                   | A Hybrid L2 −LP Variational Model For Single Low-Light Image Enhancement With Bright Channel Prior | [pdf](https://ieeexplore.ieee.org/document/8803197)          |       |
| 2019 | IET Image Proc.        | Low light image enhancement based on non-uniform illumination prior model | [pdf](https://ieeexplore.ieee.org/document/8911585)          | NIPM  |
| 2019 | Comput. Graphics Forum | Dual illumination estimation for robust exposure correction  | [pdf](https://arxiv.org/pdf/1910.13688.pdf) [code](https://github.com/pvnieo/Low-light-Image-Enhancement) |       |
| 2020 | ic-ETITE               | A comparative analysis of illumination estimation based Image Enhancement techniques | [pdf](https://ieeexplore.ieee.org/document/9077919)          |       |
| 2020 | IEEE TIP               | LR3M: Robust Low-Light Enhancement via Low-Rank Regularized Retinex Model | [pdf](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9056796) | LR3M  |
| 2023 | Vis Comput             | Illumination estimation for nature preserving low-light image enhancement | [pdf](https://link.springer.com/article/10.1007/s00371-023-02770-9) | NPLIE |


### Other methods

| Year | Pub             | Paper                                                        | Link                                                         | Note  |
| :--: | --------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ----- |
| 2008 | IET Image Proc. | Fast centre-surround contrast modification                   | [pdf](https://ieeexplore.ieee.org/document/4455541)          |       |
| 2011 | ICME            | Fast efficient algorithm for enhancement of low lighting video | [pdf](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6012107) [code](codes/XuanDong-Method.m) |       |
| 2017 | ICCVW           | A New Low-Light Image Enhancement Algorithm Using Camera Response Model | [pdf](http://ieeexplore.ieee.org/document/8265567/) [code](https://github.com/baidut/OpenCE/blob/master/ours/Ying_2017_ICCV.m) |       |
| 2017 | ArXiv           | A Bio-Inspired Multi-Exposure Fusion Framework for Low-light Image Enhancement | [pdf](http://arxiv.org/abs/1711.00591) [code](https://github.com/baidut/BIMEF) | BIMEF |
| 2017 | ICCAIP          | A New Image Contrast Enhancement Algorithm Using Exposure Fusion Framework | [pdf](https://link.springer.com/chapter/10.1007%2F978-3-319-64698-5_4) [web](https://baidut.github.io/OpenCE/caip2017.html) [code1](https://github.com/baidut/OpenCE/blob/master/ours/Ying_2017_CAIP.m) [code2](https://github.com/AndyHuang1995/Image-Contrast-Enhancement) |       |
| 2019 | IEEE TIP        | Low-Light Image Enhancement via the Absorption Light Scattering Model | [pdf](https://doi.org/10.1109/TIP.2019.2922106)              | ALSM  |
| 2019 | ICIP            | Fast Image Enhancement Based on Maximum and Guided Filters   | [pdf](https://ieeexplore.ieee.org/document/8803591)          |       |



## Related Works

| Year | Pub      | Paper                                                        | Link                                                         | Note        | Tag              |
| :--: | -------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ----------- | ---------------- |
| 2012 | IST      | Improving the robustness in feature detection by local contrast enhancement | [dataset](https://sites.google.com/site/vonikakis/datasets)  |             |                  |
| 2015 | ACM ToG  | Automatic Photo Adjustment Using Deep Neural Networks        | [web](https://sites.google.com/site/homepagezhichengyan/home/dl_img_adjust) [code](https://github.com/stephenyan1984/dl-image-enhance/wiki) [pdf](https://arxiv.org/abs/1412.7725v2) |             |                  |
| 2018 | CVPR     | Distort-and-Recover: Color Enhancement using Deep Reinforcement Learning | [code](https://sites.google.com/view/distort-and-recover/) [pdf](https://doi.org/10.1109/CVPR.2018.00621) |             |                  |
| 2021 | TMM      | Recurrent exposure generation for low-light face detection   | [pdf](https://arxiv.org/abs/2007.10963) [code](https://github.com/sherrycattt/REGDet) | REGDet      | face detection   |
| 2021 | CVPR     | HLA-Face: Joint High-Low Adaptation for Low Light Face Detection | [web](https://daooshee.github.io/HLA-Face-Website/) [pdf](https://openaccess.thecvf.com/content/CVPR2021/papers/Wang_HLA-Face_Joint_High-Low_Adaptation_for_Low_Light_Face_Detection_CVPR_2021_paper.pdf) [code](https://github.com/daooshee/HLA-Face-Code) | HLA-Face    | face detection   |
| 2021 | ICCV     | Multitask AET With Orthogonal Tangent Regularity for Dark Object Detection | [pdf](https://openaccess.thecvf.com/content/ICCV2021/papers/Cui_Multitask_AET_With_Orthogonal_Tangent_Regularity_for_Dark_Object_Detection_ICCV_2021_paper.pdf) [code](https://github.com/cuiziteng/ICCV_MAET) | MAET        | object detection |
| 2021 | ICCV     | Photon-Net: Photon-Starved Scene Inference using Single Photon Cameras | [pdf](https://openaccess.thecvf.com/content/ICCV2021/papers/Goyal_Photon-Starved_Scene_Inference_Using_Single_Photon_Cameras_ICCV_2021_paper.pdf) [code](https://github.com/bhavyagoyal/spclowlight/) [video](https://www.youtube.com/watch?v=r1YvHnGbi6k) | Photon-Net  | single photon    |
| 2021 | ICCVW    | Single-Stage Face Detection under Extremely Low-Light Conditions | [pdf](https://openaccess.thecvf.com/content/ICCV2021W/RLQ/papers/Yu_Single-Stage_Face_Detection_Under_Extremely_Low-Light_Conditions_ICCVW_2021_paper.pdf) |             | face detection   |
| 2021 | ICCVW    | DeLiEve-Net: Deblurring Low-Light Images with Light Streaks and Local Events | [pdf](https://www.semanticscholar.org/paper/DeLiEve-Net%3A-Deblurring-Low-light-Images-with-Light-Zhou-Teng/105bf9ccbc749d976ab1f4b455d379f30b1d6508) | DeLiEve-Net | event camera     |
| 2022 | ArXiv    | An Efficient Low-Light Restoration Transformer for Dark Light Field Images |                                                              | LRT         | light field      |
| 2023 | IEEE TIP | INFWIDE: Image and feature space wiener deconvolution network for non-blind image deblurring in low-light conditions | [pdf](https://ieeexplore.ieee.org/document/10047966) [code](https://github.com/zhihongz/INFWIDE) | INFWIDE     | deblurring       |



## Metrics

- MSE
- SSIM
- entropy (DE)
- EME
- AB
- PixDist
- LOE



## Blogs



## Reference
