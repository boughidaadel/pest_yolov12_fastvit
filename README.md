# 🐛 Pest–YOLOv12–FastViT

This repository contains the implementation of **Pest–YOLOv12–FastViT**, a modular two-stage deep learning framework for automatic detection and fine-grained recognition of agricultural pests.

The framework combines a real-time **YOLOv12** detector for pest localization with a **FastViT-SA12** classifier for species-level identification, trained and evaluated on the [IP102 dataset](https://github.com/xpwu95/IP102).  
It is optimized for real-time deployment on resource-constrained devices and includes ONNX model export for mobile integration.

---

## 📂 Repository Structure

| File | Description |
|------|--------------|
| `detection_yolov12_training.ipynb` | Demonstrates how to train the **YOLOv12** model for pest detection using the IP102 dataset. Includes data preprocessing, anchor optimization, and mAP evaluation. |
| `fastvit_training.ipynb` | Details the **FastViT-SA12** training pipeline for pest recognition, covering augmentation, fine-tuning strategy, and performance evaluation (Top-1/Top-5 accuracy). |
| `fv_mobile.ipynb` | Provides the **ONNX export** and optimization workflow for deploying the FastViT model on mobile or embedded devices. |

---

## 📊 Dataset
The experiments use the **IP102 benchmark dataset**, which contains more than 75,000 pest images spanning **102 categories** with over **19,000 bounding-box annotations** for detection tasks.  
Dataset link: [IP102 on GitHub](https://github.com/xpwu95/IP102)

---

## 🚀 Models and Results
Pretrained models, training logs, and evaluation results are available in the following shared folder:  
🔗 [Google Drive – Models & Results](https://drive.google.com/drive/folders/13O-qrl1vLy75-wXlk0Pw7f5fVFJ5jRcl)

- YOLOv12 detector: mAP@50 = **95.8 %**
- FastViT-SA12 classifier: Top-1 = **73.77 %**, Top-5 = **90.82 %**
- Average classification latency: **≈ 9 ms** on mobile hardware

---

## 🧠 Key Features
- **Two-stage modular architecture** (Detection → Recognition)
- **Real-time performance** with low latency on mobile hardware
- **Fine-grained classification** across 102 pest categories
- **Open, reproducible pipeline** with public dataset and pretrained models
- **ONNX export** for edge and mobile deployment

---

## 📚 Citation
If you use this code or models in your research, please cite:
> Boughida A., Benoughidene A., Kouahla M.N., Farou B., Ferdi M.  
> *Pest–YOLOv12–FastViT: A Modular Two-Stage System for Detection and Fine-Grained Recognition of Agricultural Pests.*  
> 2025.

---

## 🧩 License
This project is released under the **MIT License**.

---

**Author:** [Adil Boughida](mailto:boughida.adil@gmail.com)  
Department of Computer Science, LabSTIC Laboratory, University of 8 Mai 1945 - Guelma, Algeria
