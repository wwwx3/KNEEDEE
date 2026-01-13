# KNEEDEE — AI-Based Knee Health Screening System

## Overview
**KNEEDEE** is an AI-powered knee health screening system designed to support early detection of visible knee abnormalities using **non-X-ray camera images**.  
The system was developed using **PictoBlox Machine Learning Environment** and trained on available medical online resources and real-world data collected under hospital supervision in Thailand.

KNEEDEE transforms a simple camera into a **pre-screening medical tool**, enabling wider access to knee health assessment, especially in areas with limited medical resources.

*Note : This project is originally in Thai.*

---

## Problem
Knee conditions such as swelling, deformation, and joint abnormalities are common but often go undetected until they become severe.  
Access to imaging tools like X-ray and MRI is limited and costly, especially for the elderly and people in rural communities.

KNEEDEE addresses this gap by providing:
- A **fast, non-invasive screening method**
- A **low-cost AI-based alternative** for early detection
- A tool that supports, rather than replaces, medical professionals

---

## AI Model & Dataset

The KNEEDEE model was trained on a custom dataset consisting of **five visual knee classes**:

- Normal knees  
- Lateral swelling  
- Frontal (anterior) swelling  
- Deformed knees  
- No knee detected  

Data was collected through:
- **Shadowing orthopedic doctors** at **Police General Hospital**  
- **Prachathipat Hospital**  
- Supplementary publicly available medical images  

The dataset was used both for **training** and for **clinical-style validation**.

---

## Clinical Validation

After training, KNEEDEE was tested by comparing:
- **AI predictions**
vs  
- **Doctor visual assessments and experience**

This allowed us to evaluate not just algorithmic accuracy, but **real-world medical reliability**.

The goal was to ensure KNEEDEE behaves as a **support tool for clinicians**, not just a machine-learning demo.

---

## System Pipeline

1. Camera captures knee image  
2. Image sent to AI model  
3. Model classifies knee condition  
4. Result displayed for screening and further action  

The full training and inference pipeline is stored in the PictoBlox project file.

**System Flowchart**

![Kneedee system flowchart](img/kneedeesysflow.png)

---

## 📂 Project Files

```

KNEEDEE/
├── img/
├── pictoblox_project/
│   └── kneedee.sb3          ← AI training & inference pipeline
├── trained_model/
│   └── kneedee_model.zip    ← exported trained model
├── validation/
│   ├── confusion_matrix.png
│   └── accuracy_results.png
├── demo/
│   └── demo_video.mp4
└── README.md                ← privacy notice

```

---

## Data Privacy

The training dataset contains **real patient knee images** collected under hospital supervision.

Due to **PDPA and medical privacy regulations**, the raw images cannot be publicly released.  
This repository provides:
- The full AI training pipeline (`.sb3`)
- The trained model
- Aggregated validation results

This follows standard practice in **medical AI research**.

---

## My Role

**Chatnatda Ovatanupat (Winnie)**  
Founder & AI Engineer

- Designed the AI pipeline  
- Collected and labeled medical images  
- Coordinated with hospital doctors  
- Trained and validated the model  
- Designed system workflow and user interaction  

---

## Impact

KNEEDEE demonstrates how **AI and computer vision** can be used to:
- Improve early detection of knee conditions  
- Support healthcare professionals  
- Expand access to basic medical screening  

This project combines **medical AI, ethical data handling, and real-world deployment**.

---

## License
Educational & research use. Medical data is protected under PDPA.
```

---
