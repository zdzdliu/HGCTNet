# HGCTNet: Handcrafted Feature-Guided CNN and Transformer Network for Wearable Cuffless Blood Pressure Measurement

## Abstract
Biosignals collected by wearable devices, such as electrocardiogram and photoplethysmogram, exhibit redundancy and global temporal dependencies, posing a challenge in extracting discriminative features for blood pressure (BP) estimation. To address this challenge, we propose HGCTNet, a handcrafted feature-guided CNN and transformer network for cuffless BP measurement based on wearable devices. By leveraging convolutional operations and self-attention mechanisms, we design a CNN-Transformer hybrid architecture to learn features from biosignals that capture both local information and global temporal dependencies. Then, we introduce a handcrafted feature-guided attention module that utilizes handcrafted features extracted from biosignals as query vectors to eliminate redundant information within the learned features. Finally, we design a feature fusion module that integrates the learned features, handcrafted features, and demographics to enhance model performance. We validate our approach using two large wearable BP datasets: the CAS-BP dataset and the Aurora-BP dataset. Experimental results demonstrate that HGCTNet achieves an estimation error of 0.9 ± 6.5 mmHg for diastolic BP (DBP) and 0.7 ± 8.3 mmHg for systolic BP (SBP) on the CAS-BP dataset. On the Aurora-BP dataset, the corresponding errors are -0.4 ± 7.0 mmHg for DBP and -0.4 ± 8.6 mmHg for SBP. Compared to the current state-of-the-art approaches, HGCTNet reduces the mean absolute error of SBP estimation by 10.68% on the CAS-BP dataset and 9.84% on the Aurora-BP dataset. These results highlight the potential of HGCTNet in improving the performance of wearable cuffless BP measurements.

## Methodology
The proposed HGCTNet comprises several modules: handcrafted feature extraction and selection (HFES), CNN, handcrafted feature-guided (HGA), transformer, feature fusion, and regression.

<p align = "center">  
<img src="fig1.png" alt="img" width=650>
</p>

## Dataset
Two wearable blood pressure datasets were used in this study:
- [Aurora-BP Dataset](https://github.com/microsoft/aurorabp-sample-data)
- [CAS-BP Dataset](https://github.com/zdzdliu/CAS-BP)
