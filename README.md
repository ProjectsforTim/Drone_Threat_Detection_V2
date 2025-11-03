# 🛡️ Threat Detection Model V2

**Model V2** is an upgraded version of the original Threat Detection Model, designed to enhance small-drone recognition accuracy through expanded datasets and refined annotation standards.  
It demonstrates the evolution from prototype experimentation to near-production-grade model performance in civilian-drone threat detection contexts.

---

## 🚀 Overview
This version builds directly on Model V1 by:
- Expanding from **200 → 1,200+ annotated images**  
- Improving annotation precision and bounding-box consistency  
- Extending training to **165 epochs** for deeper convergence  
- Incorporating validation and augmentation workflows  

The result is a model capable of detecting drones at simulated long-range distances (200–240 m) with exceptional accuracy.

---

## 📊 Model V2 Performance

| Metric | Value |
|:--------|:------|
| **Precision** | 0.96 |
| **Recall** | 0.95 |
| **mAP@0.5** | **0.979 ⭐** |
| **mAP@0.5–0.95** | 0.74 |

> **IoU (Intersection over Union)** measures how much predicted and actual bounding boxes overlap.  
> *mAP@0.5* = Mean Average Precision at 50% IoU threshold.  
> *mAP@0.5–0.95* = Average across IoU thresholds 0.5–0.95.

---

## 🧠 Methodology
1. **Data Expansion** — 1,200+ drone images sourced and annotated via **Roboflow**, covering varied altitudes, lighting, and environments.  
2. **Annotation QA** — Manual verification to remove inconsistent or duplicate bounding boxes.  
3. **Training Setup** — YOLOv5 (Ultralytics) trained on Google Colab Pro with GPU acceleration, 165 epochs.  
4. **Validation** — 80/20 train-validation split with on-the-fly augmentation (rotation, scale, brightness).  
5. **Evaluation** — COCO metrics used for precision, recall, and mAP tracking across epochs.

---

## 📂 Repository Structure

---

## 🖼️ Visual Performance

**mAP@0.5 Comparison (V1 vs V2):**  
V2 outperforms early and maintains a smoother convergence curve, reaching 0.979 mAP@0.5 by epoch 165.

**Learning Curve Observation:**  
By epoch 13, V2 achieved mAP@0.5 levels that V1 did not reach until epoch 30 — a clear indicator of improved dataset and label quality.

---

## 🧾 Reproducibility
This project is **fully reproducible** via the hosted Colab notebook:  
[🔗 Open in Google Colab](https://colab.research.google.com/drive/1JtoRteMlE2KbhiwVHtgJV41LP9OUWLi8#scrollTo=bgmusWkjB0_e)

> All required dependencies, training configurations, and dataset references are included in the notebook and `requirements.txt`.

---

## ⚙️ Tools & Frameworks
- **YOLOv5 (Ultralytics)**  
- **Roboflow** for dataset creation & management  
- **Google Colab Pro** (GPU runtime)  
- **Python 3.10**, Torch 2.x, OpenCV, Matplotlib  

---

## 🧩 Key Takeaways
- Dataset quality and annotation precision directly influence detection performance.  
- Small, high-quality datasets can rival much larger public models when cleanly labeled.  
- Model V2 achieved **0.979 mAP@0.5** — comparable to leading lightweight drone-detection benchmarks.

---

## 🔭 Future Work
- Extend dataset to **3,000+ images** for robustness testing.  
- Integrate real-world drone footage for inference validation.  
- Experiment with **YOLOv8** and hybrid transformer backbones.  
- Deploy lightweight model variant for edge-device testing.

---

## 📧 Contact
Created by **Tim Lonergan**  
For collaboration or technical enquiries:  
📎 [LinkedIn](https://www.linkedin.com/in/timothylonergan/) | 🌐 [AI Portfolio](https://projectsfortim.github.io/portfolio/)

