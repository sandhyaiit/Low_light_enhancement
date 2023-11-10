# Low_light_enhancement
Presenting a deep learning based method for low-light image enhancement. This problem is challenging due to the difficulty in handling various factors simultaneously including brightness, contrast, artifacts and noise. To address this task, here proposes the multi-branch low-light enhancement network (MBLLEN).
The key idea is to extract rich features up to different levels, so that we can apply enhancement via multiple subnets and finally produce the output image via multi-branch fusion. In this manner, image quality is improved from different aspects. Through extensive experiments, our proposed MBLLEN is found to outperform the state-of-art techniques by a large margin. We additionally show that our method can be directly extended to handle low-light videos. 

Related Work:
The first category is built upon the well-known histogram equalization (HE) technique and also uses additional priors and constraints. 
In particular, BPDHE [15] tries to preserve image brightness dynamically; 
Arici et al. [2] propose to analyze and penalize the unnatural visual effects for better visual quality; 
DHECI [29] introduces and uses the differential gray-level histogram;
CVC [5] uses the interpixel contextual information; 
LDR [26] focuses on the layered difference representation of 2D histogram to try to enlarge the gray-level differences between adjacent pixels. 

The other category is based on the Retinex theory [22], which assumes that an image is composed of reflection and illumination. 
Typical methods, e.g., MSR [17] and SSR [18], try to recover and use the illumination map for low-light image enhancement. 
Recently, AMSR [24] proposes a weighting strategy based on SSR. 
NPE [37] balances the enhancement level and image naturalness to avoid over-enhancement. 
MF [11] processes the illumination map in a multi-scale fashion to improve the local contrast and maintain naturalness. 
SRIE [12] develops a weighted vibrational model for illumination map estimation. 
LIME [14] considers both the illumination map estimation and denoising. 
BIMEF [41, 42] proposes a dual-exposure fusion algorithm and Ying et al. [43] use the camera response model for further enhancement. 
In general, conventional low-light enhancement methods rely on certain statistical models and assumptions, which only partially explain the real world scenes.

Deep learning-based methods
There are also methods proposed for low-light image enhancement. LLNet [28] uses the deep autoencoder for low-light image denoising. However, it does not take advantage of recent developments in deep learning. Other CNN-based methods like LLCNN [35] and [34] do not handle brightness/contrast enhancement and image denoising simultaneously.
