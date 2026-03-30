# Satellite Image Classification

This project classifies satellite images into four categories:
- cloudy
- desert
- green_area
- water

Two models are implemented and compared:
1. Custom CNN (built from scratch)
2. MobileNetV2 (transfer learning)

---

## Dataset

The dataset used in this project is from Kaggle:

https://www.kaggle.com/datasets/xxxxx/satellite-image-classification

- Total images: 5631
- Classes: 4

The dataset is not included in this repository.

---

## Methodology

### Custom CNN
- Built using Conv2D and MaxPooling layers
- Includes Dropout to reduce overfitting
- Trained from scratch

### MobileNetV2
- Pretrained on ImageNet
- Frozen base model
- Custom classification head added

---

## Results

| Model | Validation Accuracy |
|------|---------------------|
| Custom CNN | ~90–93% |
| MobileNetV2 | ~98–99% |

---

## Comparison

The custom CNN learns features from scratch and achieves good performance.  
MobileNetV2 leverages pretrained features, resulting in higher accuracy, faster convergence, and more stable performance.

---

## Key Learnings

- Understanding CNN architecture and feature extraction
- Importance of data preprocessing and augmentation
- Transfer learning improves performance significantly
- Model comparison helps evaluate effectiveness

---

## Future Work

- Fine-tuning MobileNetV2
- Testing on unseen real-world images
- Deploying as a web application

---

## Requirements

See `requirements.txt`