<!-- PROJECT LOGO -->
<br />
<p align="center">
  <h3 align="center">Satellite Ship Detection using Manifold Learning</h3>

  <p align="center">
    A machine learning pipeline for detecting ships in satellite imagery using manifold learning and ensemble methods
    <br />
  </p>
</p>

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#dependencies">Dependencies</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#methodology">Methodology</a></li>
    <li><a href="#results">Results</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project

This project implements a machine learning pipeline for detecting ships in satellite imagery. The system uses manifold learning techniques (t-SNE, Isomap, LLE) combined with various classifiers to create an effective ship detection model. The pipeline includes data preprocessing, dimensionality reduction, model training, and evaluation components.

### Built With

* Python 3.x
* scikit-learn
* NumPy
* Pandas
* Matplotlib
* PIL (Python Imaging Library)

<!-- GETTING STARTED -->
## Getting Started

To get a local copy up and running, follow these steps.

### Dependencies

The project requires the following main packages:
* scikit-learn
  sh
  pip install scikit-learn
  
* NumPy
  sh
  pip install numpy
  
* Pandas
  sh
  pip install pandas
  
* Matplotlib
  sh
  pip install matplotlib
  
* PIL
  sh
  pip install pillow
  

### Installation

1. Clone the repo
   sh
   git clone [your-repo-link]
   
2. Install the required packages
   sh
   pip install -r requirements.txt
   

<!-- USAGE -->
## Usage

1. Dataset Preparation:
   - Place your satellite images in the scenes folder
   - Ensure images are in RGB format

2. Training the Model:
   python
   python train_model.py
   
   This will:
   - Load and preprocess the training data
   - Train multiple models using different manifold learning techniques
   - Save the best performing model

3. Ship Detection:
   python
   python detect_ships.py --scene_path scenes/your_scene.jpg
   
   This will:
   - Load the specified scene
   - Process it using a sliding window approach
   - Generate a detection map and visualization

## Methodology

The project implements a multi-stage pipeline:

1. *Preprocessing*:
   - Image standardization
   - Sliding window extraction (80x80 pixels)

2. *Feature Learning*:
   - Manifold learning techniques:
     - t-SNE
     - Isomap
     - Local Linear Embedding (LLE)

3. *Classification*:
   - Multiple classifiers evaluated:
     - Support Vector Machines (SVM)
     - Random Forest
     - k-Nearest Neighbors

4. *Detection*:
   - Sliding window approach
   - Prediction aggregation
   - Heat map generation

## Results

The best performing model combination was:
- Manifold Learning: t-SNE
- Classifier: SVM
- Metrics:
  - Accuracy: [Your accuracy score]
  - F1-Score: [Your F1 score]
  - Inference Time: [Your inference time]

The system provides three visualization outputs:
1. Original scene
2. Detection heat map
3. Detection overlay on the original image
