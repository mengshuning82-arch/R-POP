# R-POP: A Benchmark Dataset for UAV Infrared Human Detection in Jungle Environments

This repository contains the official release of the **Robust-POP (R-POP)** dataset, a specialized infrared benchmark designed for Unmanned Aerial Vehicle (UAV) jungle search and rescue (SAR) missions. 

To bridge the gap between laboratory environments and complex real-world rescue scenarios, the R-POP dataset features a **vertical altitude gradient** and high-density foliage occlusions, providing a challenging benchmark for advanced object detection algorithms (such as YOLO series, RT-DETR, etc.).

---

## 📦 Dataset Download & Extraction

Due to file size constraints, the dataset is hosted in the **[Releases](../../releases)** section and split into multiple 1900MB volumes.

### Extraction Instructions:
1. Download all split parts (`R-POP.zip`, `R-POP.z01`, `R-POP`, etc.) into the **same directory**.
2. Use an advanced compression tool (e.g., **Bandizip**).
3. Right-click **only** the main file `R-POP.zip` and select **"Extract Here"**. The software will automatically merge and extract the full dataset.

---

## 🌟 Dataset Features

- **Modality:** Thermal Infrared (TIR) images capturing human signatures.
- **Environment:** Dense, complex jungle and forest environments with varying illumination.
- **Vertical Gradient:** Images captured across a wide altitude range (from **30 meters to 100 meters**), capturing multi-scale target variations.
- **Annotation Format:** Available in **YOLO text format** .

---

## 📂 Directory Structure

After successful extraction, organize the dataset directory as follows:

```text
R-POP_dataset/
├── images/
│   ├── train/       # Training images
│   ├── val/         # Validation images
│   └── test/        # Test images (stratified by altitudes: 30m, 50m, 80m, 100m)
└── labels/
    ├── train/       # YOLO format text labels
    ├── val/         # Validation labels
    └── test/        # Test labels
