
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
rtfolio/).
