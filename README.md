# Image Captioning on Flickr8k

## Overview

This project focuses on developing an image captioning system that generates textual descriptions for images. The system leverages a combination of a pre-trained VGG16 model for feature extraction and an LSTM-based sequence model for caption generation.

## Features

    Data Preprocessing: Cleaning and tokenizing captions to prepare them for model training.
    Feature Extraction: Utilizing the pre-trained VGG16 model to extract features from images.
    Caption Generation: Employing an LSTM-based sequence model to generate textual descriptions of images.
    Model Evaluation: Using BLEU scores to assess the quality of the generated captions against reference descriptions.

## Workflow

    Data Preprocessing:
        Clean the caption data by removing unnecessary characters and handling missing data.
        Tokenize captions to convert them into a format suitable for training.

    Feature Extraction:
        Load the pre-trained VGG16 model and remove the top layers to use it as a feature extractor.
        Pass each image through the VGG16 model to obtain feature vectors.

    Model Training:
        Combine the extracted image features with tokenized captions.
        Train the LSTM-based sequence model to predict the next word in the caption given the current word and image features.

    Model Evaluation:
        Generate captions for a set of test images.
        Calculate BLEU scores to measure how well the generated captions match the reference descriptions.
