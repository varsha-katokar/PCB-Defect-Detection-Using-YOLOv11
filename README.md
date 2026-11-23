# PCB Defect Detection Using YOLOv11

## Project Overview

This project focuses on automated multiclass surface defect detection in Printed Circuit Boards (PCBs) using deep learning and the YOLO object detection framework.

The implementation uses the **SolDef AI dataset**, which contains PCB images with polygon-based annotations. The project explores annotation conversion, dataset preprocessing, segmentation, bounding-box generation and YOLO-based model training.

## Objectives

- Automate the detection of PCB surface defects.
- Convert polygon-based annotations into YOLO-compatible formats.
- Prepare and organize datasets for model training and validation.
- Explore bounding-box, oriented bounding-box (OBB) and segmentation approaches.
- Evaluate model performance and visualize defect predictions.

## Technologies Used

- Python
- YOLOv11 / Ultralytics
- OpenCV
- PyTorch
- NumPy
- Pandas
- Matplotlib
- Google Colab

## Dataset

The project uses the SolDef AI PCB Dataset for PCB surface defect detection.

The dataset contains PCB images and polygon-based JSON annotations.

Dataset Link: SolDef AI PCB Dataset – Kaggle

The dataset is not included in this repository due to its size. Download it separately and configure the dataset paths in the notebook before running the project.

## Defect Categories

The multiclass implementation explores the following categories:

| Class ID | Defect Category   |
| -------- | ----------------- |
| 0        | Good              |
| 1        | Excess Solder     |
| 2        | Poor Solder Joint |
| 3        | Spikey Solder     |

## Implementation Workflow

1. **Dataset Preparation:** Load PCB images and JSON annotation files.
2. **Annotation Processing:** Extract polygon coordinates and convert annotations into YOLO-compatible formats.
3. **Dataset Organization:** Create training and validation directories.
4. **Bounding Box Generation:** Explore axis-aligned and oriented bounding-box generation.
5. **Segmentation:** Generate polygon-based YOLO segmentation labels.
6. **Model Training:** Experiment with Ultralytics YOLO models.
7. **Inference and Visualization:** Generate predictions and visualize detected defects.

## Repository Structure

```text
PCB-Defect-Detection-Using-YOLOv11/
│
├── pcb_defect_detection.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## Installation

Clone the repository:

```bash
git clone https://github.com/varsha-katоkar/PCB-Defect-Detection-Using-YOLOv11.git
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

## Running the Project

1. Open the notebook in Google Colab.
2. Download and extract the SolDef AI dataset.
3. Upload or mount the dataset in Google Drive.
4. Update the dataset paths in the notebook according to your directory structure.
5. Execute the notebook cells to perform preprocessing, annotation conversion, model training and inference.

## Note

The dataset and trained model weights are not included in this repository. Download the dataset using the link provided above and configure the paths in the notebook before running it.
