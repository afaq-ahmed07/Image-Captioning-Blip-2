# Image Captioning Blip 2

This repository demonstrates the fine-tuning of **BLIP-2** (Bootstrapping Language-Image Pretraining) for image captioning using the **Flickr8k dataset**. The model has been fine-tuned to generate human-like descriptions of images, and the training process leverages **LoRA (Low-Rank Adaptation)** for parameter-efficient fine-tuning.

## Overview

The project uses the BLIP-2 model from Salesforce, a vision-language transformer that can understand and describe images in natural language. The **Flickr8k dataset** was used for training the model, and LoRA was applied to efficiently fine-tune the model while reducing memory and computational requirements.

### Key Components:
- **BLIP-2 Model**: A state-of-the-art image captioning model.
- **LoRA (Low-Rank Adaptation)**: A technique for efficient fine-tuning of large models.
- **Flickr8k Dataset**: A dataset consisting of 8,000 images, each paired with 5 human-generated captions.
- **IPython Notebook**: The notebook contains the complete code for loading the dataset, fine-tuning the model, and evaluating the results.

## Files & Directories

- **flickr8k.zip**: Contains the images from the Flickr8k dataset.
- **flickr8k_captions.csv**: A CSV file containing the captions for the images in the dataset.
- **blip2-flickr8k.ipynb**: Jupyter notebook that contains the entire process of fine-tuning and evaluating the BLIP-2 model.
- **model**: The fine-tuned model saved for inference and further use.

## Requirements

To run this project, ensure you have the following libraries installed:

```bash
pip install -q peft transformers bitsandbytes datasets fsspec==2025.3.0 evaluate pycocoevalcap
