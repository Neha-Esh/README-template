<!-- PROJECT LOGO --> <br /> <p align="center"> <a href="https://github.com/your_username/ship-classification"> <img src="images/ship_logo.png" alt="Logo" width="150" height="150"> </a> <h3 align="center">Ship Image Classification and Analysis</h3> <p align="center"> A pipeline for classifying ship images using traditional machine learning techniques. <br /> <a href="https://github.com/your_username/ship-classification/blob/main/docs/documentation.md"><strong>Explore the docs »</strong></a> <br /> <br /> <a href="#usage">View Demo</a> · <a href="https://github.com/your_username/ship-classification/issues">Report Bug</a> · <a href="https://github.com/your_username/ship-classification/issues">Request Feature</a> </p> </p>
<!-- TABLE OF CONTENTS --> <details open="open"> <summary>Table of Contents</summary> <ol> <li> <a href="#about-the-project">About The Project</a> <ul> <li><a href="#built-with">Built With</a></li> </ul> </li> <li> <a href="#getting-started">Getting Started</a> <ul> <li><a href="#dependencies">Dependencies</a></li> <li><a href="#installation">Installation</a></li> </ul> </li> <li><a href="#usage">Usage</a></li> <li><a href="#roadmap">Roadmap</a></li> <li><a href="#contributing">Contributing</a></li> <li><a href="#license">License</a></li> <li><a href="#authors">Authors</a></li> <li><a href="#acknowledgements">Acknowledgements</a></li> </ol> </details>
<!-- ABOUT THE PROJECT -->
About The Project
This project implements a machine learning pipeline to classify ship images as either "Ship" or "No Ship." It includes visualization tools, dimensionality reduction techniques, and supervised learning models for accurate and efficient classification.

Key features of the pipeline:

Data Visualization: Display samples of ship and no-ship images for exploratory analysis.
Dimensionality Reduction: Use Principal Component Analysis (PCA) to optimize computational efficiency and reconstruct images.
Supervised Learning: Train and evaluate models like Random Forest and SVM.
Manifold Learning: Apply t-SNE, Isomap, and LLE for advanced visualization and classification.
Built With
NumPy
Matplotlib
Seaborn
scikit-learn
Visit the project repository

<!-- GETTING STARTED -->
Getting Started
To get a local copy up and running, follow these steps.

Dependencies
Ensure the following libraries are installed:

NumPy 1.22.3

pip install numpy
Matplotlib 3.5.1

pip install matplotlib
Seaborn 0.11.2

pip install seaborn
scikit-learn 1.0.2

pip install scikit-learn
Alternative: Export Your Environment
To export your Python environment:

conda env export > environment.yml
Users can recreate the environment with:

conda env create -f environment.yml
Installation
Clone the repository:

git clone https://github.com/Neha-Esh/ship-classification.git
Set up the environment:

conda env create -f environment.yml
conda activate ship-classification-env
Add the dataset (ship_data.npy and ship_labels.npy) to the root directory.
<!-- USAGE -->
Usage
This project is modular. You can execute individual scripts for specific tasks.

Visualize Data

python visualize_data.py
This script displays random samples of ship and no-ship images, along with geographic data from specific regions.

Train Classifiers
Random Forest

python train_random_forest.py
This script trains a Random Forest model and evaluates its performance on the test set.

Dimensionality Reduction

python pca_reconstruction.py
This script reduces dimensionality using PCA and visualizes reconstructed images.

Manifold Learning

python manifold_learning.py
This script reduces image features to 2D and trains models using t-SNE, Isomap, and LLE.

For more examples, see the documentation

<!-- ROADMAP -->
Roadmap
 Integrate CNN-based classification models.
 Extend to multi-class classification for different ship types.
 Automate data preprocessing.
 Include larger datasets with distributed training support.
See the open issues for a full list of proposed features and known issues.

<!-- CONTRIBUTING -->
Contributing
Contributions are what make the open-source community such an amazing place to learn and create. Any contributions you make are greatly appreciated.

Fork the project.
Create your feature branch:

git checkout -b feature/AmazingFeature
Commit your changes:

git commit -m "Add AmazingFeature"
Push to the branch:

git push origin feature/AmazingFeature
Open a pull request.
<!-- LICENSE -->
License
Distributed under the MIT License. See LICENSE for more information.

<!-- AUTHORS -->
Authors
Your Name
GitHub: @Neha-Esh
Email: neha.eshwaragari@ufl.edu

<!-- ACKNOWLEDGEMENTS -->
Acknowledgements
This project uses:

NumPy for numerical computations.
Matplotlib and Seaborn for visualization.
scikit-learn for machine learning algorithms.
t-SNE for manifold learning.
Thank you for your support and contributions!
