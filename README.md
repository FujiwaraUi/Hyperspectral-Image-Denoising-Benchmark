# Hyperspectral-Image-Denoising-Benchmark

A list of hyperspectral image denoising resources collected by [Yongsen Zhao]( https://github.com/seniusen) and [Junjun Jiang](http://homepage.hit.edu.cn/jiangjunjun).

# Databases 
- [CAVE dataset](http://www.cs.columbia.edu/CAVE/databases/multispectral/)
- [AVIRIS](http://www.ehu.eus/ccwintco/index.php/Hyperspectral_Remote_Sensing_Scenes)
- [ROSIS](http://lesun.weebly.com/hyperspectral-data-set.html)
- [HYDICE](https://www.erdc.usace.army.mil/Media/Fact-Sheets/Fact-Sheet-Article-View/Article/610433/hypercube/)
- [EO-1 Hyperion Data](https://lta.cr.usgs.gov/ALI)
- [Harvard dataset](http://vision.seas.harvard.edu/hyperspec/explore.html)
- [iCVL dataset](http://icvl.cs.bgu.ac.il/hyperspectral/)
- [NUS datase](https://sites.google.com/site/hyperspectralcolorimaging/dataset/general-scenes)
- [NTIRE18 dataset](http://www.vision.ee.ethz.ch/ntire18/)

# Image Quality Measurement 
- Peak Signal to Noise Ratio (PSNR)
- Structural SIMilarity index (SSIM)
- Feature SIMilarity index (FSIM)
- Erreur Relative Globale Adimensionnelle de Synthèse (ERGAS)
- Spectral Angle Mapper (SAM)

![visitors](https://visitor-badge.glitch.me/badge?page_id=junjun-jiang/Hyperspectral-Image-Denoising-Benchmark) Since 2022/5/7 

# Code
## Multi-band based methods

#### **[---Transform domain method---]**
- Real Noise Decoupling for Hyperspectral Image Denoising, AAAI 2026, Yingkai Zhang, et al. [[PDF]](https://arxiv.org/pdf/2511.17196). [[Code]](https://github.com/yingkai-zhang/RND.git)

#### **[---Spatial domain methods---]**
- HIR-Diff: Unsupervised Hyperspectral Image Restoration Via Improved Diffusion Models, CVPR 2024, Li Pang, et al. [[PDF]](https://openaccess.thecvf.com/content/CVPR2024/papers/Pang_HIR-Diff_Unsupervised_Hyperspectral_Image_Restoration_Via_Improved_Diffusion_Models_CVPR_2024_paper.pdf), [[Code]](https://github.com/LiPang/HIRDiff)

## Deep learning methods
#### **[--- Earlist ---]**
- Hyperspectral Image Denoising Employing a Spatial-Spectral Deep Residual Convolutional Neural Network, TGRS2018, Q. Yuan et al. [[Code]](https://github.com/WHUQZhang/HSID-CNN)
- Deep Hyperspectral Prior: Denoising, Inpainting, Super-Resolution, arxiv2019, Oleksii Sidorov et al. [[Code]](https://github.com/acecreamu/deep-hs-prior) [[Pdf]](https://arxiv.org/pdf/1902.00301)
- Hybrid Noise Removal in Hyperspectral Imagery With a Spatial-Spectral Gradient Network, IEEE TGRS 2019, Qiang Zhang et al. [[Code]](https://github.com/WHUQZhang/SSGN) [[Pdf]](https://arxiv.org/pdf/1810.00495)
- Deep Spatial-Spectral Global Reasoning Network for Hyperspectral Image Denoising, IEEE TGRS 2021, X. Cao et al. [[Code]](https://github.com/xiangyongcao/GRN)

#### **[--- Latest ---]**
- SSUMamba: Spatial–Spectral Selective State Space Model for Hyperspectral Image Denoising, IEEE TGRS 2024, Guanyiman Fu et al. [[PDF]](https://arxiv.org/pdf/2405.01726)[[Code]](https://github.com/lronkitty/SSUMamba).  
この論文は、Denoising にコア技術として Menba を用いることで, 長距離依存性を扱う能力と計算効率を向上させた。
- Hyperspectral Image Denoising via Spatial–Spectral Recurrent Transformer, IEEE TGRS 2024, Guanyiman Fu et al. [[PDF]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10463066)[[Code]](https://github.com/lronkitty/SSRT)
- HIR-Diff: Unsupervised Hyperspectral Image Restoration Via Improved Diffusion Models, CVPR 2024, Li Pang et al. [[PDF]](https://openaccess.thecvf.com/content/CVPR2024/papers/Pang_HIR-Diff_Unsupervised_Hyperspectral_Image_Restoration_Via_Improved_Diffusion_Models_CVPR_2024_paper.pdf)[[Code]](https://github.com/LiPang/HIRDiff)
- Hybrid Spatial-Spectral Neural Network for Hyperspectral Image Denoising, ECCV 2024, Hao Liang, et al. [[Code]](https://github.com/lianghao2000/HSSD_official)
- VolFormer: Explore More Comprehensive Cube Interaction for Hyperspectral Image Restoration and Beyond, CVPR 2025, Dabing Yu, et al. [[PDF]](https://openaccess.thecvf.com/content/CVPR2025/papers/Yu_VolFormer_Explore_More_Comprehensive_Cube_Interaction_for_Hyperspectral_Image_Restoration_CVPR_2025_paper.pdf), [[Code]](https://github.com/yudadabing/VolFormer)
- LaMamba: Linear Attention Mamba for Hyperspectral Image Denoising, IEEE TGRS 2025, Puhong Duan, et al. [[PDF]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=11177616). [[Code]](https://github.com/PuhongDuan/LaMamba.git).
- MP-HSIR: A Multi-Prompt Framework for Universal Hyperspectral Image Restoration. ICCV 2025, Zhehui Wu, et al. [[PDF]](https://arxiv.org/pdf/2503.09131)[[Code]](https://github.com/ZhehuiWu/MP-HSIR.git).
- RAS2S: Region-Aware Sequence-to-Sequence Learning for Hyperspectral Denoising, ECCV 2024, Jiahua Xiao, et al. [[PDF]](https://link.springer.com/chapter/10.1007/978-3-031-73027-6_13)[[Code]](https://github.com/MIV-XJTU/RAS2S)
- QRNN3D: 3D Quasi-Recurrent Neural Network for Hyperspectral Image Denoising, IEEE 2020, Kaixuan Wei, et al. [[PDF]](https://arxiv.org/pdf/2003.04547)[[Code]](https://github.com/Vandermode/QRNN3D)
- MAC-Net: Model-Aided Nonlocal Neural Network for Hyperspectral Image Denoising, IEEE 2022, Fengchao Xiong, et al. [[PDF]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9631264)[[Code]](https://github.com/bearshng/mac-net)

## Other methods for Non-i.i.d. Noise
- Region-Aware Sequence-to-Sequence Learning for Hyperspectral Denoising, ECCV 2024, Jiahua Xiao, et al. [[PDF]](https://link.springer.com/content/pdf/10.1007/978-3-031-73027-6_13.pdf?pdf=inline%20link), [[Code]](https://github.com/MIV-XJTU/RAS2S)
- Hipandas: Hyperspectral Image Joint Denoising and Super-Resolution by Image Fusion with the Panchromatic Image, ICCV 2025, Shuang Xu, et al. [[PDF]](https://openaccess.thecvf.com/content/ICCV2025/papers/Xu_Hipandas_Hyperspectral_Image_Joint_Denoising_and_Super-Resolution_by_Image_Fusion_ICCV_2025_paper.pdf), [[Code]](https://github.com/shuangxu96/Hipandas)