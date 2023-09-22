# Face Mask Detection using YOLOv5

## Overview

This project aims to detect the usage of face masks in images using object detection models. It categorizes each face into one of the three types:

1. Wearing a mask correctly
2. Wearing a mask incorrectly
3. Not wearing a mask at all

The dataset for this project is sourced from Kaggle, and YOLOv5 is utilized for object identification. A custom YAML model is also implemented to optimize efficiency.

![Training Dataset Image](<images/Screenshot 2023-09-21 at 3.40.48 PM.png>)

## Dataset

The dataset consists of images segregated into three categories: 'Correct', 'Incorrect', and 'No Mask'. The distribution of these categories is visualized below:

![Dataset Histogram](link-to-histogram-image)

## Model Training

### Architecture

The YOLOv5 model is used for object identification, optimized with a custom YAML model for better performance.

### Training Details

- **Epochs**: 50
- **Metrics**:
     - Box Loss
     - Object Loss (obj_loss)
     - Classification Loss (cls_loss)

![Metrics Graphs](link-to-graphs)

### Validation Losses

- Validation Box Loss
- Validation Object Loss
- Validation Classification Loss

![Validation Losses Graphs](link-to-validation-losses-graphs)

### Evaluation Metrics

- Precision
- Recall
- mAP at IoU=0.5
- mAP at IoU=0.5:0.95

![Evaluation Metrics Graphs](link-to-evaluation-metrics-graphs)

### Learning Rate Graphs

- lr1
- lr2
- lr3

![Learning Rate Graphs](link-to-learning-rate-graphs)

## Testing

A set of randomly picked images were used for testing the model. Results are showcased before and after the object detection task.

![Testing Images](link-to-testing-images)

## Setup and Run

1. Clone the repository
      ```
      git clone [your-repository-link]
      ```
2. Install dependencies
      ```
      pip install -r requirements.txt
      ```
3. Run the Jupyter Notebook
      ```
      jupyter notebook Face_Mask_Detection.ipynb
      ```

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

---

Remember to replace the placeholders such as `link-to-your-example-image` with the actual URLs or relative paths of your images. This should provide a comprehensive view of your project, its functionality, and performance metrics.
