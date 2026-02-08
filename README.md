# Hardware II – Object Detection Assignment

This repository contains my submission for the **Hardware II** course assignment
(IAAC – MRAC 2025/26).

The project focuses on training and evaluating an object detection model using
**computer vision techniques**.  
A single object class (**cup**) was selected to keep the scope focused and to
allow a clear analysis of the full workflow.

---

## Workflow Overview

- Selection of a single object class (cup)
- Dataset preparation and annotation using **Roboflow**
- Dataset versioning, preprocessing, and augmentation
- Training of a YOLO-based object detection model
- Qualitative evaluation of detection results

---

## Tools & Technologies

- **Roboflow** – dataset management, annotation, preprocessing
- **YOLOv8 (Ultralytics)** – object detection model
- **Python / OpenCV** – contextual relation to course content
- **GitHub** – documentation and submission

---

## Dataset

- Total images: **375**
- Train / Validation / Test split: **80% / 13% / 7%**
- Preprocessing:
  - Auto-orient
  - Resize to 256×256
- Augmentation:
  - Horizontal flip

---

## Results & Observations

The trained model shows a high number of **false positives** and detects multiple
objects instead of only the target class (cup).

This behavior is primarily caused by:
- a limited and visually complex dataset
- strong contextual features (tables, coffee beans, backgrounds)
- insufficient negative examples

Rather than learning the object alone, the model learned **contextual patterns**,
which leads to over-detection.

This outcome is intentional and demonstrates the importance of:
- dataset quality
- clean annotations
- balanced class distribution
- controlled visual environments

---

## Conclusion

This project is an **exploratory experiment**, not a production-ready model.

The main learning outcome is understanding:
- the complete object detection pipeline
- the influence of dataset bias on model behavior
- limitations of neural networks trained on small or noisy datasets

---

## References & Links

### Miro Board  
https://miro.com/app/board/uXjVGLZ_DpM/

### ChatGPT Conversation (process documentation)  
https://chatgpt.com/share/69765339-e290-800f-979d-8a61548d622a

---

**Student:** Leonard Elias Böker  
**Course:** Hardware II  
**Institution:** IAAC
