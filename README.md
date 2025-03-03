# Knowledge Distillation Using Contrastive Learning

## Overview

This project uses contrastive learning to explore knowledge distillation from a large monolingual model to a smaller multilingual one. Specifically, we employ CLIP loss to transfer knowledge effectively.

## Dataset

A small English-Persian paired dataset is used to define the loss pairs for CLIP training. Due to computational limitations, we work with a reduced batch size, focusing on understanding the training process rather than achieving state-of-the-art performance.

## Installation & Dependencies

To set up the environment and download necessary resources, run:

```bash
pip install -q gdown

# Download dataset
!gdown "https://drive.google.com/uc?id=1MVx_gIkX4tQ8ya2OsHt0mqLmw1Pf2CcK"
!gdown "https://drive.google.com/uc?id=1Co-dwJfWw-C_ral0hoAS_X94wN-_vbCj"

# Install necessary libraries
pip install setuptools torch torchvision transformers
```

## Main Components

The project contains the following key parts:

- **Dataset Preparation**: Loading and pre-processing the English-Persian text pairs.
- **Model Setup**: Initializing the student model and defining CLIP loss.
- **Training Procedure**: Training the model using a contrastive learning approach.
- **Evaluation**: Measuring the alignment of multilingual representations.

## How to Run

1. Clone the repository and navigate to the project folder.
2. Install dependencies as mentioned above.
3. Run the Jupyter Notebook (`HW6_401106396.ipynb`) step by step.

## Expected Outcomes

Since the dataset is small, this exercise is primarily focused on learning the training procedure rather than producing real-world results.

