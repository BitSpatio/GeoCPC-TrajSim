# 🛰️ TS-CPC: Geometry-Consistent Self-Supervised Trajectory Similarity via Contrastive Predictive Coding

This repository contains the official implementation of **TS-CPC**, a self-supervised trajectory similarity measurement framework based on Contrastive Predictive Coding (CPC). TS-CPC is designed to handle complex trajectory datasets efficiently while delivering robust and accurate similarity measurements.

---

## 🔑 Key Features
- **Sliding-Window-based Linear Interpolation (SW-LI):** Enhances trajectory features by preserving fine-grained details and improving model performance.  
- **Trajectory Detour Point Offset (TDPO):** Improves robustness against real-world noise and drift.  
- **SFEM (Shallow Feature Extraction Module):** Extracts essential motion dynamics (speed, acceleration, orientation, angular velocity, curvature, etc.) to enrich trajectory representation.  
- **Enhanced CPC module:** Incorporates a principled positive–negative sampling strategy to strengthen InfoNCE discrimination and convergence.  

---

## 📘 Journal Extensions (Remote Sensing, 2025)

Compared with our **ICIC 2025 conference paper**, the journal version achieves **substantial extensions and systematic improvements** in theoretical depth, methodological design, experimental analysis, and reproducibility:

1. **Expanded literature review:** Covers contrastive learning, graph neural networks, and self-supervised trajectory learning.  
2. **Clearer methodology formulation:** Standardized definitions, notations, and evaluation metrics for interpretability.  
3. **Refined SRA-M module:** Integration of SW-LI and TDPO to address sampling inconsistency and GPS noise.  
4. **Extended SFEM module:** Expanded from 7D to 9D shallow motion features.  
5. **Enhanced CPC module:** Encoder details and improved sampling strategy.  
6. **TGCB benchmark:** Introduces Hausdorff distance, normalized Fréchet distance, angular deviation, and visual gallery.  
7. **New baselines:** Added CSTRM and TrajCL for stronger comparisons.  
8. **Broader robustness evaluation:** On Grab-Posisi and GeoLife datasets under down-sampling and distortion.  
9. **Efficiency analysis:** Includes training time, inference time, FLOPs, and parameter counts; TS-CPC achieves up to **70% faster training**.  
10. **Parameter sensitivity study:** Impact of encoder dimension, kernel size, and depth.  
11. **Comprehensive ablation study:** Validates SW-LI, TDPO, and SFEM independently.  
12. **Improved figures & visualization:** Optimized diagrams and enhanced clarity.  

---

## 📊 Key Results

### Datasets
- **Grab-Posisi:** High retrieval performance across varying down-sampling and distortion rates.  
- **GeoLife:** Significant improvements in trajectory similarity measurement accuracy.  

### Performance Highlights
- **Representation quality:** High-quality spatiotemporal embeddings for accurate comparisons.  
- **Robustness:** Maintains performance under noise, drift, and perturbations.  
- **Efficiency:** Achieves reduced training and inference time compared with competing methods.  

---

## 🔧 Version Information
- **OS:** Ubuntu 20.04  
- **Python:** 3.8  
- **PyTorch:** 1.13.1  
- **CUDA:** 11.7  
- **GPU:** NVIDIA A100  

---

## 📂 Data & Code Availability
- **GeoLife dataset:** Released by Microsoft Research — [link](https://www.microsoft.com/en-us/research/project/geolife-building-social-networks-using-human-location-history/).  
- **Grab-Posisi dataset:** Available upon request via email: [grab-posisi.geo@grab.com](mailto:grab-posisi.geo@grab.com).  
- **Source code & TGCB benchmark:** Available in this repository and maintained under version control.  
- **Reproducibility:** All preprocessing scripts and evaluation code are provided.  

---

## 📜 License
This project is licensed under the **MIT License**.  
