# Pediatric Knee Fracture X-Ray Pipeline (CycleGAN)

This repository contains a complete data preprocessing, annotation, and synthetic bias generation pipeline designed to prepare pediatric knee X-ray images for training a CycleGAN model. 

This project is part of the Medical AI research presented at the BRIDGE-AI Summit 2026 (Digital Health Innovation Exhibition).

## Tech Stack
* Language: Python
* Libraries: OpenCV (cv2), Pandas, NumPy
* Core Focus: Computer Vision, Data Preprocessing, Automated Pipeline, Synthetic Data Generation

## Repository Contents

Here is a breakdown of the custom tools built for this data pipeline:

### 1. annotate_physis.py (Custom Annotation Tool)
A custom-built GUI tool using OpenCV designed specifically for medical image annotation.
* Allows manual bounding box drawing for Femur and Tibia bones.
* Supports labeling for different Salter-Harris (SH) fracture classifications.

### 2. augment_data.py (Offline Augmentation)
An automated script to artificially expand the X-Ray dataset to improve CycleGAN training accuracy using flipping, rotations, and contrast adjustments.

### 3. synthetic_damage_generator.py & synthetic_bias_generator.py
Scripts that manage the flow of raw data and generate synthetic clinical biases.
* Automatically splits the dataset into trainA / testA and trainB / testB.
* Integrates with clinical_bias_weights.json to simulate real-world medical data distributions.

### 4. convert_to_json.py
A utility script to convert the annotated CSV bounding box data into JSON format (xray_bounding_boxes.json) for easier integration.

---
Developed by a Computer Engineering & AI Student @PIM, passionate about Data Analytics, AI Innovation, and Process Automation.
---
## 🏆 Certifications & Awards

This project and my core technical skills have been recognized at the following national events:

* **BRIDGE-AI Summit 2026:** Exhibition Participant (Rising Innovator, Medical AI) — Presented this pediatric knee fracture prediction system. [View Certificate](./Bridge_Certificate.pdf)
