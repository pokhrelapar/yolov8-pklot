# YOLOv8-PKLOT: Parking Space Occupancy Detection

This project presents a comparative analysis of different YOLOv8 backbone architectures for parking space occupancy detection using the **PKLot** dataset. Each folder contains a specific YOLOv8 variant trained and evaluated independently. Results are visualized and compared to highlight performance differences in terms of accuracy, generalization, and robustness.

## 📁 Project Structure

### `comparison-plots/`
Contains visualization artifacts, such as:
- Confusion matrices
- Performance comparison plots (e.g., Precision, Recall, mAP)
- Training and validation loss curves

Used for analyzing and reporting the performance of all model variants side-by-side.

---

### `yolov8n/`
Baseline YOLOv8n model with default backbone. Includes:
- Training notebook/scripts
- Evaluation metrics
- Exported model weights (if saved)

---

### `yolov8n-efficeint-net-v2/`
YOLOv8n modified with an **EfficientNetV2** backbone. Includes:
- `yolov8n-efficient-netv-2.ipynb`: Training and evaluation notebook
- `runs/`: Auto-generated training logs, metrics, and best weights

Designed to evaluate the impact of a lightweight but powerful backbone on parking detection.

---

### `yolov8n-ghostp2/`
YOLOv8n with a **GhostNet-P2** backbone, designed for efficiency on edge devices. Contains:
- Training notebook and evaluation results
- All metrics recorded during training

---

### `yolov8n-resnet18/`
YOLOv8n variant using a **ResNet-18** backbone. Offers a balance between depth and speed.
- Useful for comparing traditional CNN backbones to modern efficient architectures

---

### `yolov8n-vgg16/`
YOLOv8n with **VGG-16** backbone integration.
- Known for simplicity and strong feature extraction in image classification tasks
- Benchmark for performance comparison

---


### `README.md`
This documentation file, summarizing the purpose and structure of the project.

---

## 🚀 Getting Started

To run any of the models:
1. Navigate to the corresponding folder.
2. Open the training notebook (e.g., `yolov8n-efficient-netv-2.ipynb`).
3. Install dependencies and run all cells.

Each notebook is self-contained and processes training, validation, and metric visualization.

---

## 📊 Evaluation Metrics

All models are evaluated using:
- **Precision**
- **Recall**
- **mAP@50**
- **mAP@50:95**
- **Confusion Matrix**

Results are visualized in `comparison-plots/` for easy comparison.

---

## 📌 Dataset

All models are trained on the **PKLot** dataset, a public benchmark for parking space occupancy detection. Ensure the dataset is properly formatted and located in your working directory before training.

---

## 📬 Contact

For questions or contributions, feel free to open an issue or contact the author.

---
