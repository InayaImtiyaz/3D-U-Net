
# 🧠 3D U-Net for Medical Image Segmentation

This repository contains a clean and customizable implementation of a **3D U-Net** model, designed for volumetric (3D) medical image segmentation tasks. It is particularly useful for segmenting organs or tumors in **CT** or **MRI** scans.

---

## 🏥 Application

This implementation was tested on the **Liver Tumor Segmentation (LiTS)** dataset. It can be adapted for any medical image dataset that provides 3D volumetric data (NIfTI or NumPy format).

---

## 📌 Features

- ✅ 3D U-Net architecture with encoder-decoder structure  
- ✅ Works with NIfTI or `.npy` 3D data  
- ✅ Patch-based training for memory efficiency  
- ✅ Visualizes slices and segmentation results  
- ✅ Easy integration with new datasets  
- ✅ Save/load model checkpoints  

---

## 🧱 Model Architecture

The 3D U-Net consists of:

- **Encoder:** 3D Convolution → BatchNorm → ReLU → MaxPool  
- **Bottleneck:** Deepest feature representation  
- **Decoder:** Transposed 3D Convolutions + Skip Connections  
- **Output:** 1×1×1 convolution for voxel-wise classification  

---

Trained on https://www.kaggle.com/datasets/andrewmvd/liver-tumor-segmentation

