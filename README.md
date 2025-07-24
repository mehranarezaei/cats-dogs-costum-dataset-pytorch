# CatDogDataset

A simple PyTorch-based custom dataset loader and a project to distinguish cats from dogs using the [Kaggle Dogs vs. Cats dataset](https://www.kaggle.com/c/dogs-vs-cats/data).

## Overview

This repository implements a `CatDogDataset` class built on top of `torch.utils.data.Dataset`, which:

1. Recursively gathers all images from the training folder.  
2. Loads them with Pillow and converts to RGB.  
3. Transforms each image to a PyTorch tensor.  
4. Automatically assigns labels (`0` for cat, `1` for dog) based on parent folder name.  

You can easily plug this into a `DataLoader` and train any CNN model (ResNet, EfficientNet, etc.) for binary classification.

---

## Dataset

We use the Kaggle “Dogs vs. Cats” dataset:

- **Competition page**: https://www.kaggle.com/c/dogs-vs-cats  
- **Direct data**: https://www.kaggle.com/c/dogs-vs-cats/data  
