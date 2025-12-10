# HyperAgri-RGB2HSI-Dataset

---

## Overview

**HyperAgri-RGB2HSI** is an open-source agricultural hyperspectral dataset.  
This dataset is constructed from publicly available **crop RGB image datasets**, where hyperspectral image (HSI) cubes are generated using an **RGB-to-HSI reconstruction algorithm**, enabling a unified, standardized, and reusable agricultural multimodal dataset.

The dataset is designed to support research in:

- Crop disease recognition and severity analysis  
- Weed and crop object detection and segmentation  
- Hyperspectral reconstruction and cross-modal generation  
- Spectral analysis and decision-making in precision agriculture  

> This GitHub repository only provides dataset documentation, structure description, and license information.  
> **The actual data files are hosted on Baidu Netdisk.**
<img width="350" height="245" alt="image" src="https://github.com/user-attachments/assets/b86b50fb-a895-4806-b444-a503baf47f34" />
<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/9e05bcb9-8445-489a-abd7-296c413f9b48" />

---

## Dataset Summary

| Item | Description |
|------|-------------|
| **Dataset Name** | HyperAgri-RGB2HSI |
| **Upstream RGB Datasets** | DeepWeeds, Global Wheat Head Dataset 2021 (GWHD 2021) |
| **Release Date** | 2025-12-01 |
| **Task Types** | Image classification, segmentation, object detection, hyperspectral reconstruction |
| **Modalities** | RGB, HSI |
| **Spatial Resolution** | Same as original RGB images |
| **Spectral Bands** | 31 bands (400–760 nm) |
| **Data Format** | `.mat` |
| **License** | CC BY 4.0 (for reconstructed HSI) + upstream licenses |

---

## Download


The dataset is available via **Baidu Netdisk**:

- **Dataset Name**: `HyperAgri-RGB2HSI-Dataset`  
- **Download Link**:  
  https://pan.baidu.com/s/108FijCjdtrMED6J_9UHFtQ?pwd=87y1  
- **Access Code**: `87y1`

After downloading, please extract the archive locally and keep the original directory structure to avoid potential path or indexing issues.

---

## Directory Structure

The directory structure of this dataset **follows the original RGB datasets exactly**,  
with reconstructed hyperspectral `.mat` files added to the same directories as the corresponding RGB images.

In other words:
- Original RGB images remain unchanged  
- Each RGB image has a corresponding HSI `.mat` file stored in the same directory  

---

## Upstream Datasets and Licenses

The hyperspectral data in this dataset are reconstructed from the following publicly available RGB datasets.  
**Each upstream dataset retains its original license and usage restrictions**.

1. **DeepWeeds**
   - Description: An in-field weed recognition dataset collected in Australia, containing 8 weed classes and 17,509 RGB images  
   - Original purpose: Weed classification and detection  
   - License: Creative Commons Attribution 4.0 (CC BY 4.0)  
   - Source: https://github.com/AlexOlsen/DeepWeeds  

2. **Global Wheat Head Dataset 2021 (GWHD 2021)**
   - Description: A multi-country, multi-scenario wheat head detection dataset  
   - Original purpose: Wheat head object detection  
   - License: Creative Commons Attribution 4.0 (CC BY 4.0)  
   - Source: https://www.kaggle.com/datasets/vbookshelf/global-wheat-head-dataset-2021  

---
