# SkimLit NLP 📄🔥

SkimLit NLP aims to simplify reading medical abstracts by leveraging Natural Language Processing (NLP). This project replicates and expands upon the research architecture from the paper [PubMed 200k RCT](https://arxiv.org/abs/1710.06071).

## Overview

This repository includes:

-   A machine learning pipeline for classifying medical abstract sentences.
-   Pretrained models using the Universal Sentence Encoder.
-   Experimentation with multiple model architectures, including hybrid embeddings and tribrid models.

## Features

-   **Multi-input architectures**: Token, character, and positional embeddings.
-   **Reproducibility**: All experiments are included in the notebook.
-   **Pretrained embeddings**: Universal Sentence Encoder for semantic similarity.

## Project Structure

skimlit-nlp/
├── notebooks/ # Jupyter notebooks for experimentation
│ └── skimlit-nlp.ipynb # Main notebook
├── utils/ # Utility functions for preprocessing and visualization
│ └── helper_functions.py # Functions used throughout the project
├── README.md # Project documentation
└── requirements.txt # Python dependencies

## Setup Instructions

1. Clone the repository and navigate to the project directory:

`git clone https://github.com/aiwkz/skimlit-nlp.git`
`cd skimlit-nlp`

2. Install the necessary packages:

`pip install -r requirements.txt`

3. Download the helper functions script if not included:

`!wget https://raw.githubusercontent.com/aiwkz/skimlit-nlp/refs/heads/main/utils/helper_functions.py`

4. (Optional) If running in Google Colab, mount Google Drive to access the saved model.

## Usage

1. Run the notebook:

-   Open `skimlit-nlp.ipynb` in a Jupyter notebook environment or Google Colab.
-   Ensure you have access to the Food101 dataset through TensorFlow Datasets.

2. The notebook includes the following steps:

-   Loading and preparing the data.
-   Building and fine-tuning the EfficientNetV2 model.
-   Training and evaluating the model.
-   Saving and loading the model for reuse.

3. (Optional) Save the model in your Google Drive for future use.

## Requirements

-   Python 3.7+
-   TensorFlow 2.0+
-   TensorFlow Datasets
-   NumPy
-   Matplotlib

A `requirements.txt` file is included in the repository with the necessary dependencies.

## Results

The model achieves competitive performance compared to the original paper, demonstrating its ability to classify medical abstracts effectively.

## License

This project is created for educational purposes as part of a course and is not intended for commercial use.
