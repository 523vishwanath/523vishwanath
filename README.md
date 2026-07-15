<!-- Banner: replace github-profile/assets/banner.svg in this repo with the new banner.svg -->
<p align="center">
  <img src="https://raw.githubusercontent.com/523vishwanath/523vishwanath/main/github-profile/assets/banner.svg" alt="Vishwanath Reddy Ninganolla — Computer Vision Engineer" width="100%"/>
</p>

<p align="center">
  <a href="https://linkedin.com/in/vishwanathninganolla"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:vninganolla@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  <a href="https://github.com/523vishwanath"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
  <a href="https://www.kaggle.com/vishwanath523"><img src="https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white" alt="Kaggle"/></a>
</p>

---

## 👋 About Me

I'm a **Computer Vision Engineer** and MSIT candidate at **Florida State University** (GPA 3.9, graduating May 2026), focused on building real-world autonomous perception systems that actually ship.

I design end-to-end deep learning pipelines across **detection, segmentation, and tracking** — and I care as much about the systems engineering as the model. On my BDD100K perception stack I took inference from ~3.3 FPS to ~14 FPS through pipeline-level optimization alone, with no change to the model. My work spans autonomous driving perception, medical imaging, aerial/UAV inspection, and deployed classification services with FastAPI + Cloud Run front ends.

Previously a Software Engineer at **HCLTech**, where I built scalable data pipelines in Python and SQL. I'm now focused on shipping fast, reliable CV systems — and **actively seeking roles in autonomous driving and perception.**

- 🔭 Building multi-task perception stacks with **YOLO, RF-DETR, SegFormer, DeepLabV3, Depth Anything V2**
- ⚡ Optimizing inference with **TensorRT (FP16) and ONNX** for low-latency deployment
- 🧪 Tracking every experiment with **Weights & Biases / Comet ML**
- 📫 Reach me at **vninganolla@gmail.com**

---

## 🔬 Featured Projects

### 🚗 Autonomous Traffic Perception — BDD100K Pipeline (TensorRT)
> **YOLO26l · YOLO26l-seg · Depth Anything V2 · TensorRT FP16 · NVIDIA A100/T4**

A production-grade, multi-task autonomous driving perception pipeline on the **BDD100K** dataset. Runs **object detection (9 classes), drivable-area segmentation, and monocular depth** simultaneously on 1080p driving video — then optimized end-to-end with TensorRT.

**Detection mAP50: 56.3% · Drivable-area Mask mAP50: 91.8% · ~14 FPS at 1080p.** Pipeline engineering alone took throughput from **3.3 → 14 FPS (4.3×)** with zero model changes.

[![Autonomous Traffic Perception Demo](https://raw.githubusercontent.com/523vishwanath/Autonomous-Traffic-Perception/main/assets/demo.gif)](https://github.com/523vishwanath/Autonomous-Traffic-Perception)

🔗 **[Repository](https://github.com/523vishwanath/Autonomous-Traffic-Perception)** · ▶️ **[Full demo on YouTube](https://www.youtube.com/watch?v=PDP2xSCtjgk)**

---

### 🦟 VectorID — Mosquito Species & Sex Classifier
> **EfficientNet-B0 (multi-head) · PyTorch · FastAPI · Google Cloud Run · Comet ML**

A two-head classifier (7 species, 2 sexes) replicating the architecture behind **VectorCam**, the Johns Hopkins platform for AI-assisted malaria vector surveillance. Carried end to end: data pipeline → multi-task training → containerized API → cloud deployment → live web front end.

**Species accuracy: 89.4% · Sex accuracy: 92.6%** (with test-time augmentation).

[![VectorID Live Demo](https://raw.githubusercontent.com/523vishwanath/VectorCam_Mosquito_classifier/main/results/demo.gif)](https://523vishwanath.github.io/VectorCam_Mosquito_classifier/)

🔗 **[Repository](https://github.com/523vishwanath/VectorCam_Mosquito_classifier)** · 🌐 **[Try the live web app](https://523vishwanath.github.io/VectorCam_Mosquito_classifier/)**

---

### ⚡ Power Line Asset Detection for UAV Inspection — RF-DETR
> **RF-DETR (Detection Transformer) · InsPLAD-det · COCO mAP · PyTorch**

Fine-tuned **RF-DETR** to detect and classify **17 fine-grained transmission-line hardware components** (insulators, dampers, shackles, spacers, yokes, tower ID plates) from high-resolution drone imagery — the perception layer that makes large-scale, AI-assisted line inspection viable.

**mAP50: 94.6% · mAP50-95: 76.9% · Precision/Recall ≈ 91%.**

[![Power Line Asset Detection](https://raw.githubusercontent.com/523vishwanath/Power-Line-Asset-Detection-for-Automated-UAV-Inspection/main/insplad_project/assets/pred_sample_1.png)](https://github.com/523vishwanath/Power-Line-Asset-Detection-for-Automated-UAV-Inspection)

🔗 **[Repository](https://github.com/523vishwanath/Power-Line-Asset-Detection-for-Automated-UAV-Inspection)**

---

### 🚦 Real-Time Traffic Signal State Recognition — YOLOv8
> **YOLOv8x · SAHI Sliced Inference · NVIDIA A100**

End-to-end detection of tiny traffic lights (**Red / Yellow / Green / Wait-On**) in high-resolution images. Tile-based fine-tuning and SAHI sliced inference handle the small-object problem.

**mAP50-95 improved 42 → 55 · mAP50: 80 · ~22 FPS on video.**

[![Traffic Signal Recognition Demo](https://raw.githubusercontent.com/523vishwanath/523vishwanath/main/github-profile/assets/demo.gif)](https://github.com/523vishwanath/Real-Time-Traffic-Signal-State-Recognition-Red-Yellow-Green-with-YOLOv8)

🔗 **[Repository](https://github.com/523vishwanath/Real-Time-Traffic-Signal-State-Recognition-Red-Yellow-Green-with-YOLOv8)**

---

### 🩺 Retinal Blood Vessel Segmentation — SegFormer
> **SegFormer-B3 · Albumentations · Mixed Precision · Weights & Biases · NVIDIA A100**

Fine-tuned SegFormer-B3 on retinal fundus images with a custom **Dice + Cross-Entropy loss** to address severe class imbalance (~10% vessel pixels).

**78.02% mIoU** across thin and thick vessel structures.

[![Retinal Vessel Segmentation](https://raw.githubusercontent.com/523vishwanath/523vishwanath/main/github-profile/assets/icprInference.png)](https://github.com/523vishwanath/retinal-vessel-segmentation)

🔗 **[Repository](https://github.com/523vishwanath/retinal-vessel-segmentation)**

---

### 🛰️ Aerial Drone Image Segmentation — DeepLabV3
> **DeepLabV3-ResNet101 · Dice + CE Loss · Albumentations · Kaggle Competition**

12-class semantic segmentation of drone aerial imagery, built for the OpenCV × PyTorch Kaggle competition. Combined Dice + Cross-Entropy loss with an auxiliary head to handle heavy class imbalance (sky/vegetation/road vs. tiny people/bikes/animals).

**Kaggle leaderboard: 0.57 Dice** across all 12 classes.

[![Aerial Drone Segmentation Results](https://raw.githubusercontent.com/523vishwanath/Aerial-Drone-Image-Segmentation/main/drone_seg_project/assets/predictions/valid_sample_0.png)](https://github.com/523vishwanath/Aerial-Drone-Image-Segmentation)

🔗 **[Repository](https://github.com/523vishwanath/Aerial-Drone-Image-Segmentation)**

---

## 🛠️ Tech Stack

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white)

**Computer Vision & Deep Learning**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![Ultralytics](https://img.shields.io/badge/Ultralytics_YOLO-00BFFF?style=flat-square&logoColor=white)
![Albumentations](https://img.shields.io/badge/Albumentations-F0364E?style=flat-square&logoColor=white)

**Model Architectures**

`YOLO26 / YOLOv8` · `RF-DETR` · `DETR / RT-DETR` · `SegFormer` · `DeepLabV3` · `EfficientNet` · `ViT` · `Depth Anything V2` · `CNNs`

**Deployment & MLOps**

![TensorRT](https://img.shields.io/badge/TensorRT-76B900?style=flat-square&logo=nvidia&logoColor=white)
![ONNX](https://img.shields.io/badge/ONNX-005CED?style=flat-square&logo=onnx&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Google Cloud](https://img.shields.io/badge/Cloud_Run-4285F4?style=flat-square&logo=googlecloud&logoColor=white)
![WandB](https://img.shields.io/badge/Weights_&_Biases-FFBE00?style=flat-square&logo=weightsandbiases&logoColor=black)
![CUDA](https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white)

**Techniques**

`Mixed Precision (AMP)` · `SAHI Sliced Inference` · `Dice + CE Loss` · `Multi-Task Learning` · `TensorRT FP16 Optimization` · `Data Augmentation Pipelines` · `mIoU / mAP Evaluation`

---

## 💼 Experience

**HCLTech — Software Engineer** · *Sep 2022 – Aug 2024*
Built scalable data analysis pipelines in Python and SQL, created visualization dashboards on Google PLX, and led Agile sprint execution as POD Lead for a team of engineers.

**Capgemini — Software Engineer Intern** · *Feb 2022 – Aug 2022*
Engineered backend modules for a Java-based banking system with MySQL/JDBC integration.

---

## 🎓 Education

**Florida State University** — *Master of Science in Information Technology (MSIT)*
GPA 3.9 · Expected May 2026 · Focus: Computer Vision, Deep Learning, Autonomous Perception

---

## 🏅 Certifications

- Advanced Vision Applications with Deep Learning & Transformers
- Deep Learning with PyTorch 2.x
- Computer Vision & Image Processing in Python — OpenCV University
- Machine Learning Specialization

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=523vishwanath&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" height="165" alt="GitHub Stats"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=523vishwanath&layout=compact&theme=tokyonight&hide_border=true" height="165" alt="Top Languages"/>
</p>

---

## 📫 Connect

<p align="center">
  <a href="https://linkedin.com/in/vishwanathninganolla"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:vninganolla@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  <a href="https://github.com/523vishwanath"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=523vishwanath&color=58a6ff&style=flat-square&label=Profile+Views" alt="Profile Views"/>
</p>
