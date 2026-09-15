# Hyperspectral-Image-Denoising-Benchmark

A list of hyperspectral image denoising resources collected by [Yongsen Zhao]( https://github.com/seniusen) and [Junjun Jiang](http://homepage.hit.edu.cn/jiangjunjun). Editted By Yui FUJIWARA. 

![visitors](https://visitor-badge.glitch.me/badge?page_id=junjun-jiang/Hyperspectral-Image-Denoising-Benchmark) Since 2022/5/7 

# Code
## Multi-band based methods

### **[---Transform domain method---]**
- Real Noise Decoupling for Hyperspectral Image Denoising, AAAI 2026, Yingkai Zhang, et al. [[PDF]](https://arxiv.org/pdf/2511.17196). [[Code]](https://github.com/yingkai-zhang/RND.git)

### **[---Spatial domain methods---]**
- HIR-Diff: Unsupervised Hyperspectral Image Restoration Via Improved Diffusion Models, CVPR 2024, Li Pang, et al. [[PDF]](https://openaccess.thecvf.com/content/CVPR2024/papers/Pang_HIR-Diff_Unsupervised_Hyperspectral_Image_Restoration_Via_Improved_Diffusion_Models_CVPR_2024_paper.pdf), [[Code]](https://github.com/LiPang/HIRDiff)

## Deep learning methods
### **[--- Earlist ---]**
- Hyperspectral Image Denoising Employing a Spatial-Spectral Deep Residual Convolutional Neural Network, TGRS2018, Q. Yuan et al. [[Code]](https://github.com/WHUQZhang/HSID-CNN)
- Deep Hyperspectral Prior: Denoising, Inpainting, Super-Resolution, arxiv2019, Oleksii Sidorov et al. [[Code]](https://github.com/acecreamu/deep-hs-prior) [[Pdf]](https://arxiv.org/pdf/1902.00301)
- Hybrid Noise Removal in Hyperspectral Imagery With a Spatial-Spectral Gradient Network, IEEE TGRS 2019, Qiang Zhang et al. [[Code]](https://github.com/WHUQZhang/SSGN) [[Pdf]](https://arxiv.org/pdf/1810.00495)
- Deep Spatial-Spectral Global Reasoning Network for Hyperspectral Image Denoising, IEEE TGRS 2021, X. Cao et al. [[Code]](https://github.com/xiangyongcao/GRN)

### **[--- Latest ---]**
- SSUMamba: Spatial–Spectral Selective State Space Model for Hyperspectral Image Denoising, IEEE TGRS 2024, Guanyiman Fu et al. [[PDF]](https://arxiv.org/pdf/2405.01726)[[Code]](https://github.com/lronkitty/SSUMamba).  
Core: Mamba。SSUMamba と比べて SSRT-UNet の方が性能良い？メモリ効率とかを未チェック。LaMamba は SSUMamba よりも性能が良い。
- SSRT-UNet: Hyperspectral Image Denoising via Spatial–Spectral Recurrent Transformer, IEEE TGRS 2024, Guanyiman Fu et al. [[PDF]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10463066)[[Code]](https://github.com/lronkitty/SSRT).  
Core: Transformer。SSUMamba と比べて SSRT-UNet の方が性能良い？メモリ効率とかを未チェック。
- HIR-Diff: Unsupervised Hyperspectral Image Restoration Via Improved Diffusion Models, CVPR 2024, Li Pang et al. [[PDF]](https://openaccess.thecvf.com/content/CVPR2024/papers/Pang_HIR-Diff_Unsupervised_Hyperspectral_Image_Restoration_Via_Improved_Diffusion_Models_CVPR_2024_paper.pdf)[[Code]](https://github.com/LiPang/HIRDiff).  
Core: Diffusion Models。教師なし機械学習である点は魅力的。他の Model-Based Methods (NGMeet) の方が優れている場合がある。どうしても教師データの取得が難しいときは選択肢に上がる？
- HSSD: Hybrid Spatial-Spectral Neural Network for Hyperspectral Image Denoising, ECCV 2024, Hao Liang, et al. [[HTML]](https://arxiv.org/html/2406.08782v1) [[Code]](https://github.com/lianghao2000/HSSD_official).  
Core: CNN + Transformer。CNN と Transformer のいいとこ取りをしたみたいやモデル。
- VolFormer: Explore More Comprehensive Cube Interaction for Hyperspectral Image Restoration and Beyond, CVPR 2025, Dabing Yu, et al. [[PDF]](https://openaccess.thecvf.com/content/CVPR2025/papers/Yu_VolFormer_Explore_More_Comprehensive_Cube_Interaction_for_Hyperspectral_Image_Restoration_CVPR_2025_paper.pdf), [[Code]](https://github.com/yudadabing/VolFormer).  
Core: Transformer。Transformer ベースで、空間方向とスペクトル方向をトークン化することで相関関係を取得する。超解像、ノイズ除去、分類のタスクで優れた実績を獲得している。
- LaMamba: Linear Attention Mamba for Hyperspectral Image Denoising, IEEE TGRS 2025, Puhong Duan, et al. [[PDF]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=11177616). [[Code]](https://github.com/PuhongDuan/LaMamba.git).   
Core: Mamba。既存のMamba は入力順序に強く依存し、長いシーケンスに対して損失が生じやすい。LaMamba は SSUMamba よりも性能が良い。
- MP-HSIR: A Multi-Prompt Framework for Universal Hyperspectral Image Restoration. ICCV 2025, Zhehui Wu, et al. [[PDF]](https://arxiv.org/pdf/2503.09131)[[Code]](https://github.com/ZhehuiWu/MP-HSIR.git).   
Core: プロンプトエンジニアリング + Transformer。ノイズ、ボケ、雲・霞、データ欠損などの多様な劣化に対して、プロンプトエンジニアリングを中人に解決する。ちょっとやりたいこととは違うかな。
- RAS2S: Region-Aware Sequence-to-Sequence Learning for Hyperspectral Denoising, ECCV 2024, Jiahua Xiao, et al. [[PDF]](https://link.springer.com/chapter/10.1007/978-3-031-73027-6_13)[[Code]](https://github.com/MIV-XJTU/RAS2S).  
Core: Sequence to Sequence。デノイジングをS2Sに置き換える。領域分割してより精度を向上させる。精度はもしかしてあまり良くない？
- QRNN3D: 3D Quasi-Recurrent Neural Network for Hyperspectral Image Denoising, IEEE 2020, Kaixuan Wei, et al. [[PDF]](https://arxiv.org/pdf/2003.04547)[[Code]](https://github.com/Vandermode/QRNN3D).  
Core: Neural Network。2020 年だから他と比較すると古い。データ分割とか性の比較でよく出てくるので一応出しておいく。
- MAC-Net: Model-Aided Nonlocal Neural Network for Hyperspectral Image Denoising, IEEE 2022, Fengchao Xiong, et al. [[PDF]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9631264)[[Code]](https://github.com/bearshng/mac-net).  
Core: 物理モデル + Spacial DL。他モデルよりも性能はひいが、ブラックボックス化の回避に一石投じている。

## Other methods for Non-i.i.d. Noise
- Region-Aware Sequence-to-Sequence Learning for Hyperspectral Denoising, ECCV 2024, Jiahua Xiao, et al. [[PDF]](https://link.springer.com/content/pdf/10.1007/978-3-031-73027-6_13.pdf?pdf=inline%20link), [[Code]](https://github.com/MIV-XJTU/RAS2S)
- Hipandas: Hyperspectral Image Joint Denoising and Super-Resolution by Image Fusion with the Panchromatic Image, ICCV 2025, Shuang Xu, et al. [[PDF]](https://openaccess.thecvf.com/content/ICCV2025/papers/Xu_Hipandas_Hyperspectral_Image_Joint_Denoising_and_Super-Resolution_by_Image_Fusion_ICCV_2025_paper.pdf), [[Code]](https://github.com/shuangxu96/Hipandas)

## Compare
#### SSUMamba: Spatial–Spectral Selective State Space Model for Hyperspectral Image Denoising
| Model-Based Methods | Deep Learning-Based Methods |
|---|---|
| BM4D, MTSNMF, LLRT, NGMeet, LRMR, FastFyDe, LRTFL_0, E-3DTV | T3SC, MAC-Net, NSSNN, TRQ3D, SST, SSUMemba |
#### SSRT-UNet: Hyperspectral Image Denoising via Spatial–Spectral Recurrent Transformer
| Model-Based Methods | Deep Learning-Based Methods |
|---|---|
| BM4D, MTSNMF, LLRT, NGMeet, LRMR, FastFyDe, LRTFL_0, E-3DTV | T3SC, MAC-Net, NSSNN, TRQ3D, SST, SSRT-UNet |
#### HSSD: Hybrid Spatial-Spectral Neural Network for Hyperspectral Image Denoising
| Model-Based Methods | Deep Learning-Based Methods |
|---|---|
| BM4D,  LLRT, NGMeet | HSID, GRNet, QRNN3D, T3SC, MAC-Net, SST, SERT, HSDT_L, SSRT-UNet |
#### VolFormer: Explore More Comprehensive Cube Interaction for Hyperspectral Image Restoration and Beyond
| Model-Based Methods | Deep Learning-Based Methods |
|---|---|
|BM4D, KBR, WLRTR, NGmeet| HSID-CNN, QRNN3D, DPPR, SST|
#### LaMamba: Linear Attention Mamba for Hyperspectral Image Denoising
| Model-Based Methods | Deep Learning-Based Methods |
|---|---|
|LRMR, NGMeet, HyDe, NMoG, LRTDTV| T2SC, MACNet, SST, SERT, HAC-Net, SSUMamba|
#### RAS2S: Region-Aware Sequence-to-Sequence Learning for Hyperspectral Denoising
| Model-Based Methods | Deep Learning-Based Methods |
|---|---|
|LLRT, LRTDTV, LLRGTV, NGMeet|QRNN3D, GRNet, MAC-Net, T3SC, GRUNet, MST, MAN, SST, SERT, HSDT-S|
#### MAC-Net: Model-Aided Nonlocal Neural Network for Hyperspectral Image Denoising
| Spare methods| Low-rank Methods|DL Methods|
|---|---|---|
|MB4D, TDL, MTSNMF|LLRT, NGMeet, LRMR, LRTDTV, FastHyDe|Dn-CNN, HSI-SDe, HSID-CNN, QRNN3D |

## Adopt methods. 
### 01: SSRT-UNet.   
Transformer. SSRT-UNet > SSUMamba. 
### 02: VolFormer.   
Transformer. 
### 03: LaMamba.   
Mamba. LaMamba > SSUMamba. 
### 04: RAS2S.   
Sequence to Sequence. 領域分割しているため. 
### 05: Mac-Net.  
物理モデル + Unet. ブラックボックス化の回避. 

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