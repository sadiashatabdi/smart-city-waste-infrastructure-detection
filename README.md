# Smart City Waste and Infrastructure Detection

Smart City Waste and Infrastructure Monitoring using YOLOv11s.

This repository contains a notebook-based object detection workflow for monitoring waste and infrastructure conditions in urban environments using YOLOv11s. The project is designed to help detect waste-related objects and support smart city monitoring through computer vision.

## Project Overview

The goal of this project is to build an intelligent vision system to identify and monitor waste and related urban infrastructure conditions from images. Using YOLOv11s, the model can be trained, validated, and tested on custom datasets to support city maintenance and environmental monitoring tasks.

## Key Use Cases

- Waste bin and litter detection
- Urban garbage monitoring
- Infrastructure condition inspection
- Smart city environmental analysis
- Vision-based monitoring for municipal services

## Repository Structure

```text
bangladeshi-fish-detection-yolo11/
│
├── README.md
├── .gitignore
├── requirements.txt
│
├── notebooks/
│   └── fish-detection-yolo11s.ipynb
│
└── assets/
    ├── prediction-examples.png
    ├── confusion-matrix.png
    ├── confusion-matrix-normalized.png
    └── train-validation-loss.png
```
## Tech Stack

- Python
- OpenCV
- Ultralytics YOLOv11
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
## How to Run

1. Clone this repository.
2. Install the required Python libraries.
3. Open the notebook in Kaggle or Jupyter Notebook.
4. Download or connect the dataset from Roboflow.
5. Configure the dataset path and `data.yaml`.
6. Run the notebook cells in sequence to train and evaluate the model.

## Example Inference

```python
from ultralytics import YOLO

model = YOLO('yolo11s.pt')
results = model('sample.jpg')
results[0].show()
```

## Typical Workflow

1. Prepare and label the dataset
2. Train the YOLOv11s model
3. Validate the model on test data
4. Run prediction on new images or videos
5. Analyze model output and improve dataset quality

## Notes

This project is intended for experimentation and development around smart city waste and infrastructure analysis. It can be extended with custom classes, different datasets, and deployment workflows depending on project requirements.

## License

This project currently does not specify a license file. If you plan to distribute or publish it publicly, you may want to add a license such as MIT.

## Contribution

Contributions are welcome. If you want to improve the dataset, add new notebooks, or refine the detection pipeline, feel free to submit a pull request.

## Repository

- GitHub: https://github.com/sadiashatabdi/smart-city-waste-infrastructure-detection
