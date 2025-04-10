# Wafer Defect Detection - Lightweight Mask R-CNN

## 🧪 Overview

This project aims to build a lightweight and efficient Mask R-CNN-based model to detect **single and mixed-type defects** in wafer maps.  
The model incorporates:
- **MobileNetV3 + CBAM** as the backbone,
- **FCOS (Anchor-Free RPN)** for object proposal,
- **GhostConv** for efficient mask head processing.

The goal is to achieve **real-time defect detection** suitable for semiconductor production environments.

---

## 📁 Dataset

- **WM-811K**: [Kaggle WM-811K Dataset](https://www.kaggle.com/datasets/qingyi/wm811k-wafer-map)
- **Mixed-Type WM38**: [Kaggle Mixed-Type Dataset](https://www.kaggle.com/datasets/co1d7era/mixedtype-wafer-defect-datasets)

We apply preprocessing including:
- Noise removal, resizing, normalization
- Data augmentation (rotation, flipping) to address class imbalance

---

## 🧠 Model Architecture
- MobileNetV3 + CBAM 
- FCOS 
- RoI Align + FC layers 
- Classification + BBox Regression 
- GhostConv-based Mask Head

> ⚡ Designed for efficient instance segmentation and pixel-wise defect localization.

---

## 📊 Evaluation Metrics

We use both **detection** and **efficiency** metrics:

### Detection:
- Precision / Recall / F1-Score
- Accuracy
- IoU
- Multi-label Classification Accuracy

### Efficiency:
- FLOPs
- Model Size (MB)
- Parameter Count
- FPS (Frames Per Second)

---

## 🔧 Tools

- Python, PyTorch
- Google Colab Pro
- OpenCV, Matplotlib
- Scikit-learn, NumPy

---

## 👨‍💻 Team Members

| Name     | Student ID |
|----------|------------|
| 백지원   | 2033014    |
| 정윤수   | 2172045    |
| 한지민   | 2172126    |
| 황수빈   | 2176422    |
| 김지우   | 2272008    |

---

## 📅 Timeline

- Week 1–3: Project planning, goal setting
- Week 2–6: Dataset collection and preprocessing
- Week 4–11: Model development, tuning, and evaluation
- Regular team meetings: 3 times/week

---

## 📌 Keywords

`Semiconductor`, `Wafer Defect`, `Instance Segmentation`, `Mask R-CNN`, `MobileNetV3`, `GhostConv`, `FCOS`, `Edge AI`, `Lightweight Model`

---

## 🔗 References

- GhostNet (CVPR 2020)  
- MobileNetV3 (ICCV 2019)  
- CBAM (ECCV 2018)  
- FCOS (ICCV 2019)  
- WM-811K & Mixed-Type Wafer Datasets on Kaggle
