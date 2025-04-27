# Breast Arterial Calcification Segmentation using U-Net

This repository contains the code and resources for the project on breast arterial calcification (BAC) segmentation from mammograms using a U-Net model. The project aims to automate the detection and analysis of BAC, which is an important marker for cardiovascular risk.This branch of code is an extended version utilizing patching techniques to improve the outcomes!

## Table of Contents
- [Project Overview](#project-overview)
- [Directory Structure](#directory-structure)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
  - [Preprocessing](#preprocessing)
  - [Training](#training)
  - [Testing](#testing)
  - [Feature Extraction](#feature-extraction)
  - [Inference](#inference)
  - [Self-Supervised Learning](#self-supervised-learning)
- [Configuration](#configuration)
- [Requirements](#requirements)
- [Contributing](#contributing)
- [License](#license)

## Project Overview
The goal of this project is to develop a deep learning-based model for the segmentation of breast arterial calcifications on mammograms. The model is based on the U-Net architecture and can be trained and tested on both GPU and CPU environments. The repository includes notebooks for preprocessing, training, testing, feature extraction, inference, and self-supervised learning.

## Directory Structure
```
.
├── config.yaml
├── requirements.txt
├── preprocess_patches.ipynb
├── train_patches.ipynb
├── test_patches.ipynb
├── self_supervised_patches.ipynb
├── README.md
```

## Setup Instructions
1. **Clone the repository:**
    ```bash
    git clone https://github.com/yourusername/BAC-segmentation.git
    cd BAC-segmentation
    ```

2. **Create and activate the conda environment:**
    ```bash
    conda env create -f config.yaml
    conda activate bac_env
    ```

3. **Install the required packages:**
    ```bash
    pip install -r requirements.txt
    ```

## Usage

### Preprocessing
The preprocessing notebook prepares the data for model training and testing. You need to set up the paths in the notebook.
1. Open `preprocess_patches.ipynb`.
2. Set the appropriate paths for your dataset.
3. Run the cells to preprocess the data.

### Training
The training notebook is used to train the U-Net model.
1. Open `train_patches.ipynb`.
2. Ensure the paths and parameters are correctly set.
3. Run the cells to start training the model.

### Testing
The testing notebook evaluates the model's performance on the test dataset.
1. Open `test_patches.ipynb`.
2. Set the appropriate paths and parameters.
3. Run the cells to test the model.

### Self-Supervised Learning
The self-supervised notebook demonstrates the use of self-supervised learning techniques without labeled data.
1. Open `self_supervised_patches.ipynb`.
2. Set the paths and parameters as needed.
3. Run the cells to train the model using self-supervised learning methods.

## Configuration
The `config.yaml` file contains the configuration for the conda environment. Make sure to update it if you need any additional packages or changes to the environment.

## Requirements
All the required packages are listed in the `requirements.txt` file. Install them using pip:
```bash
pip install -r requirements.txt
```

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request or open an issue to discuss improvements, bug fixes, or new features.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

