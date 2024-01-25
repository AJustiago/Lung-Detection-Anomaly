 **# Lung Anomaly Detection with Detectron**

**## Overview**

This project demonstrates how to detect lung anomalies in chest X-ray images using Detectron2 and PyTorch. It utilizes the VinBigData Chest X-ray Resized PNG (256x256) dataset available on Kaggle.

**## Dataset**

- **Source:** [https://www.kaggle.com/datasets/xhlulu/vinbigdata-chest-xray-resized-png-256x256](https://www.kaggle.com/datasets/xhlulu/vinbigdata-chest-xray-resized-png-256x256)
- **Description:** Contains resized chest X-ray images with annotations for lung anomalies.
- **Structure:**
    - `train` folder: Contains training images.
    - `test` folder: Contains test images.
    - `train_meta.csv`: Contains metadata for training images (image IDs, original sizes).
    - `test_meta.csv`: Contains metadata for test images (image IDs, original sizes).
    - `train.csv`: Contains bounding box annotations for lung anomalies in training images.

**## Installation**

1. Create a virtual environment (recommended):
```bash
conda create -n lung-anomaly-detection python=3.8
conda activate lung-anomaly-detection
```
2. Install dependencies:
```bash
pip install -r requirements.txt
```

**## Usage**

1. Download the dataset from Kaggle and extract it into the project directory.
2. Run the training script:
```bash
python train.py
```
3. Run the inference script on a test image:
```bash
python inference.py --image_path path/to/test_image.png
```

**## Further Information**

- Detectron2 documentation: [https://detectron2.readthedocs.io/](https://detectron2.readthedocs.io/)
- VinBigData Chest X-ray Abnormalities Detection competition: [https://www.kaggle.com/c/vinbigdata-chest-xray-abnormalities-detection](https://www.kaggle.com/c/vinbigdata-chest-xray-abnormalities-detection)

**## Disclaimer**

This project is for educational and research purposes only. It is not intended for clinical use.
