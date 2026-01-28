# Vehicle Detection Comparison: CNN vs Vision Transformers

This project provides a fast experimental benchmark comparing **CNN-based** and **Transformer-based** object detectors on the **UA-DETRAC vehicle dataset**.

The goal is to evaluate how well different detection architectures identify vehicles in traffic surveillance frames, using standard COCO evaluation metrics.

---

## 📌 Models Compared

We compare three pretrained object detection models:

| Model | Architecture Type | Description |
|------|------------------|-------------|
| YOLOv8n | CNN-based detector | Fast one-stage convolutional vehicle detector |
| DETR (ResNet-50) | Vision Transformer detector | Transformer-based global attention detector |
| RF-DETR Nano | Lightweight Transformer detector | Real-time transformer variant (single-class vehicle detection) |

---

## 📂 Dataset Used

**UA-DETRAC Vehicle Detection Benchmark**

- Traffic surveillance dataset with bounding-box annotations  
- Vehicle categories: **car, bus, van, others**
- Original annotation format: XML
- Converted into COCO format for evaluation

### Dataset statistics (Test split)

- Total test frames: **56,167**
- Total bounding boxes: **675,774**

For fast evaluation, experiments were run on a random subset:

- Evaluation subset size: **1000 images**
- Random seed: **123**

---


