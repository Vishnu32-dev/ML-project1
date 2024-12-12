# ML-project1
image classification
# Emotion Detector in Art

## Project Overview
The **Emotion Detector in Art** is a machine learning project designed to analyze and interpret emotions conveyed by artworks. Leveraging the WikiArt dataset and advanced neural networks, the project aims to bridge the gap between the emotions intended by the artist and those perceived by the audience. This repository contains the code, data processing pipelines, and model training scripts required for the project.

---

## Features
- **Dataset:** Utilizes the WikiArt dataset and a complementary emotion-labeled dataset.
- **Model Architecture:** Fine-tuned VGG16 model with additional dense layers.
- **Augmentation:** Extensive data augmentation using `ImageDataGenerator` for robust training.
- **Emotion Mapping:** Maps artworks to their corresponding emotions for insightful analysis.
- **Performance Tracking:** Includes training logs, model checkpoints, and metrics evaluation.

---

## Prerequisites
### Software Requirements
- Python 3.10+
- Google Colab (for GPU acceleration)
- Libraries:
  - TensorFlow
  - NumPy
  - Pandas
  - scikit-learn
  - Matplotlib

### Hardware Requirements
- Access to GPU (e.g., Google Colab or a local GPU-enabled environment)

---

## Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/emotion-detector-art.git
   cd emotion-detector-art
   ```
2. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```

---

## Usage
### Data Preparation
1. Download the WikiArt dataset and ensure it follows this structure:
   ```
   p1/
   └── archive/
       └── <class folders containing images>
   ```
2. Place the emotion-labeled `.csv` file in the `p1` directory.

### Training the Model
1. Mount Google Drive in Colab:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```
2. Run the training script provided in `emotiondetector.py`.
3. Monitor training with model checkpoints and early stopping.

### Model Evaluation
1. Evaluate the model on validation data to track accuracy and loss.
2. Generate a classification report to assess emotion predictions.

---

## File Structure
```
project-folder/
|── emotiondetector.py      # Main script for model training and evaluation
|── p1/
    |── archive/         # Contains WikiArt dataset
    |── Contrastive.csv  # Emotion-labeled dataset
|── README.md           # Project documentation (this file)
```

---

## Model Details
- **Base Model:** Pretrained VGG16 (ImageNet weights)
- **Input Shape:** 224x224x3
- **Output:** Softmax layer with classes corresponding to emotions

---

## Results
- **Training Accuracy:** TBD
- **Validation Accuracy:** TBD
- **Classification Report:** Pending completion of analysis.

---

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes and open a pull request.

---

## License
This project is licensed under the MIT License.

---

## Contact
For inquiries or collaborations, feel free to reach out:
- **Name:** [Vishnu Prakash Singh]
- **Email:** [vishnuprakashsingh32@gmail.com]
- **GitHub:** [Vishnu32]

---
