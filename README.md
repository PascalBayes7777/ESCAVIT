## ESCAViT: EEG Spectrogram Convolutional Audio Vision Transformer

This repository contains the implementation of ESCAViT for IIIC pattern classification, including:

Domain_Specific_Mixup.py: Implementation of Domain-Specific Mixup strategy
-> Adaptive EEG Spectrogram Mixup (AES-Mix)

Symmetry_Aware_Contrastive_Learning_Loss.py: Symmetry-Aware Contrastive Learning Loss
-> Lead Interrelation-Guided Contrastive Learning (LIGCL)

ESCAViT.py: ESCAViT model architecture


## Overview
Domain-Specific Mixup: Custom mixup strategy for handling EEG data ambiguity
-> Adaptive EEG Spectrogram Mixup (AES-Mix)

Symmetry-Aware Contrastive Learning: Loss function designed for lead symmetry learning
-> Lead Interrelation-Guided Contrastive Learning (LIGCL)

ESCAViT: Multi-stream architecture combining ViViT with lead attention mechanisms


## Dataset
This study used data from the "HMS - Harmful Brain Activity Classification" competition on Kaggle (https://www.kaggle.com/competitions/hms-harmful-brain-activity-classification). The dataset is licensed under CC BY-NC 4.0.


## Training Setting
All models were trained/tested on one NVIDIA GeForce RTX A6000 48GB GPU. Training is facilitated by the AdamW optimizer, with a learning rate of 1e-4, weight decay of 1e-3, and is conducted over 50 epochs with a batch size of 8.
