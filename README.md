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

## 🔍 Key Learnings
- Dataset quality and annotation accuracy heavily influence detection performance.  
- Even with limited training data, model V1 achieved robust detection reliability.  
- Lays groundwork for **Model V2**, which expanded to 1,200+ annotations and achieved mAP@0.5 = 0.979.

---

## 🧾 Reproducibility
This model is **fully reproducible** via the linked Colab notebook:  
[Open in Google Colab](https://colab.research.google.com/drive/1JtoRteMlE2KbhiwVHtgJV41LP9OUWLi8#scrollTo=bgmusWkjB0_e)

---

## ⚙️ Tools & Frameworks
- **YOLOv5** (ultralytics)  
- **Roboflow** for dataset management  
- **Google Colab** for training and evaluation  
- **Python 3.10**, Torch 2.x  

---

## 🛠️ Next Steps
- Expand dataset diversity (angles, distances, lighting conditions).  
- Implement Model V2 comparisons for benchmark visibility.  
- Prepare deployment-ready inference notebook for real-time detection scenarios.

---

## 📧 Contact
Created by **Tim Lonergan**  
For questions or collaboration, please connect via [LinkedIn](https://www.linkedin.com/in/timothylonergan/) or view my [AI Portfolio](https://projectsfortim.github.io/portfolio/).
