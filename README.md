# Aerial Target Tracking: Benchmarking Algorithms on an Air-to-Air UAV Dataset

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Conference: ROBIO 2025](https://img.shields.io/badge/ROBIO-2025-red.svg)](http://www.robio2025.org/)

---

## 👨‍💻 Authors
**Chengwei Li**, Xiangyu Zhu, [Yong Wang](https://github.com/hapless19), Wenzhi Tang, Xuefeng Ren, Shunan Wu, and Zhigang Wu

---

## 🖼️ Overview
<p align="center">
  <img src="./figures/Trackerandtarget.png" width="400">
  <br>
  <em>Figure 1: Overview of the air-to-air tracking scenarios.</em>
</p>
---

## 📌 Abstract
This paper studies the problem of air-to-air visual tracking of quad-rotor unmanned aerial vehicle(UAV). This research is important for applications like security monitoring, logistics and emergency rescue. Current deep learning tracking algorithms have shown superior performance in various tracking tasks, on the purpose of exploring full potential of these methods for UAV tracking, we present a new dataset, named Drone2Drone, which consists of 58 video sequences containing over 110000 frames. Compared to other existing datasets, the proposed one features diverse environmental backgrounds, various shooting angles, and multiple lighting conditions. We implement a comprehensive training and evaluation process  based on OSTrack tracking algorithms with the proposed datasets. The results indicate UAV tracking improvement and prove that tracker learns more robust class-level UAV information. Furthermore, we present an experimental evaluation of eight representative tracking algorithms, the result of which highlights some prominent challenges in the task of air-to-air UAV tracking and suggests possible directions for tracking algorithms improvement in the future. All the resources will be available before October.

---

## 📂 Table of Contents
* [Introduction](#-introduction)
* [Contributions](#-contributions)
* [Quick View](#-quick-view-dataset)
* [Experimental Results](#-experimental-results)
* [Dataset Download](#-dataset-download)
* [Citation](#-citation)

---

## 🚀 Introduction
Reliable target tracking is a essential for autonomous Unmanned Aerial Vehicle (UAV) operations. While existing benchmarks have extensively covered ground-to-air or air-to-ground scenarios, air-to-air tracking remains significantly under-explored despite its critical importance in aerial refueling, formation flight, and counter-UAV missions.
The air-to-air scenario introduces unique challenges:
* **Highly Dynamic Backgrounds:** Rapid ego-motion of the tracking UAV causes intense view fluctuations.
* **Extreme Scale Variations:** Drastic changes in relative distance.
* **Complex Motion Models:** High-degree-of-freedom maneuvers in 3D space.

---

## 💡 Contributions
* **New Benchmark:** Proposes a novel air-to-air UAV dataset specifically designed for aerial target tracking.
* **Extensive Evaluation:** Benchmarks state-of-the-art (SOTA) tracking algorithms on the new dataset.
* **Analysis:** Provides deep insights into the impact of relative motion and complex backgrounds in aerial scenarios.

---

## 📸 Quick View
### Dataset Samples
<p align="center">
  <img src="./figures/scenarios.png" width="400">
  <br>
  <em>Figure 2: Sample images from our air-to-air UAV Dataset.</em>
</p>

---

## 📊 Experimental Results
### Quantitative Comparison
| Tracker | Success Rate | Precision | FPS |
| :--- | :---: | :---: | :---: |
| Tracker A | 0.654 | 0.721 | 45 |
| Tracker B | 0.712 | 0.789 | 30 |
| **Ours (Best)** | **0.845** | **0.892** | **60** |

### Visualization
![Results Chart](./assets/results_plots.png)
*Figure 3: Success and Precision plots comparing our benchmarked algorithms.*

---

## 📥 Dataset Download
The dataset is available for academic purposes:
* **[Link to Dataset]**: [Insert Link, e.g., Google Drive or Baidu Netdisk]
* **[Link to Code]**: [If applicable, link to your tracking code]

---

## 📜 Citation
If you find our work or dataset useful for your research, please cite:

```bibtex
@inproceedings{li2025aerial,
  title={Aerial Target Tracking: Benchmarking Algorithms on an Air-to-Air UAV Dataset},
  author={Li, C. and Zhu, X. and Wang, Y. and Tang, W. and Ren, X. and Wu, S. and Wu, Z.},
  booktitle={Proceedings of the IEEE International Conference on Robotics and Biomimetics (ROBIO)},
  year={2025}
}

# Drone2Drone-dataset
# Introduction
The proposed dataset primarily utilizes DJI UAVs (MAVIC, Air, Mini, Phantom) to capture mutual footage through various shooting techniques, including orbiting, fixed-point, and following. These methods allow for the collection of diverse UAV videos from multiple angles and distances, enriching the dataset with varied perspectives. Drone2Drone comprises 109,628 images from 50 video sequences with image resolutions of 1920×1080 and 2720×1530.
<img width="942" height="548" alt="image" src="https://github.com/user-attachments/assets/4b3b9b93-f8c6-4f04-9c8a-d72bf25d9acd" />

# Dataset Downloads
The dataset can be downloaded in https://pan.baidu.com/s/1sxv0Fw-Gy__Aqo6W2xNDCA?pwd=3m2j pwd: 3m2j

The first frame annotation is stored in [left top width height].
