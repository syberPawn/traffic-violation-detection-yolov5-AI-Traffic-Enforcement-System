# AI Traffic Violation Detection System  
### **Research + Prototype Development (Ongoing Project)**  
This repository contains an ongoing research and development project aimed at building an academic prototype for **automated traffic violation detection** using **YOLOv5**, **OpenCV**, and **OCR**.

The goal is to create a **learning-oriented**, cost-effective system that mimics real-world AI-based traffic enforcement pipelines.

---

## 🚦 Project Overview
Modern traffic enforcement systems use artificial intelligence to automatically detect violations such as:

- Helmetless riding  
- Triple riding  
- Wrong-lane usage  
- Red-light jumping  
- Number plate recognition  

However, most available solutions are:

- Expensive  
- Black-box systems  
- Require heavy infrastructure  

This project aims to create a simplified, transparent model suitable for **academic learning and small-scale experimentation**.

---

## 📚 Literature Review (Completed)
A comprehensive review of **33+ research papers** was conducted to understand:

- YOLOv3–YOLOv8 detection models  
- CNN-based traffic detection  
- Low-light two-wheeler violation datasets (LoLTV)  
- Challenges in occlusion, motion blur, and nighttime detection  
- ALPR (Automatic License Plate Recognition) techniques  
- Limitations of current datasets  

All detailed notes, summaries, and PPTs are available in the `/research/` directory.

---

## 🧩 Identified Research Gaps
Key gaps found in existing systems:

- Low performance in **night-time / low-light** conditions  
- Most models detect **only one violation** (e.g., helmet detection)  
- Lack of **Indian traffic datasets** publicly available  
- High computation cost for real-time deployment  
- Limited end-to-end solutions combining detection + OCR + automation  

---

## ⚙️ Initial Model Training (YOLOv5)
To understand baseline performance, a YOLOv5 model was trained on the **Dhaka-AI YOLO dataset**.

**Training Configuration**
- Dataset: Dhaka-AI (Kaggle)  
- Images: 2390 (train) + 600 (val)  
- Image Size: 640 × 640  
- Model: YOLOv5s  
- Epochs: 100  
- Optimizer: SGD  
- Platform: Google Colab  

**Initial Results**
- **Precision:** 71.9%  
- **Recall:** 37.5%  
- **mAP@0.5:** 43.5%  
- **Box Loss Reduction:** 67.4%  
more in the repo
