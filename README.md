# Traffic Sign Classification with CNN

This project uses a convolutional neural network (CNN) to classify traffic signs into 43 categories based on image data. The model is trained on images of traffic signs and can save the trained model for future use.

## Features

- **Image Classification**: Classifies images of traffic signs into 43 categories.
- **Customizable Model Saving**: Optionally save the trained model as a `.h5` file for later use.

## Requirements

- **Python 3.x**
- **Packages**: `opencv-python`, `tensorflow`, `numpy`, `scikit-learn`
- **Data**: Ensure the data directory contains subdirectories numbered from 0 to 42, each holding images for a specific category.

## Setup

1. **Install dependencies**:
   ```bash
   pip install opencv-python tensorflow numpy scikit-learn
   ```

2. **Data Directory**:
   - Organize the traffic sign images in the `data_directory` as specified: subdirectories `0`, `1`, ..., `42`, each containing images of the corresponding category.

## Usage

1. **Run the script**:
   ```bash
   python traffic.py data_directory [model.h5]
   ```
   - Replace `data_directory` with the path to your image data.
   - Optionally, add `model.h5` to save the trained model.

2. **Output**:
   - The model displays training and testing accuracy after each epoch.
   - Evaluation metrics (accuracy) are shown for the test set.

## Code Overview

- **Functions**:
  - `main()`: Manages data loading, model training, and saving.
  - `load_data(data_dir)`: Loads and processes images into a format suitable for training.
  - `get_model()`: Defines and compiles the CNN architecture for classification.

