# Practicallab3
 Vanilla CNN and Fine-Tune VGG16 - for Dogs and Cats Classification

# The notebook includes:
- Data loading from 5000 image subset
- Data augmentation and preprocessing
- CNN model training and evaluation
- VGG16 base model training and fine-tuning
- Evaluation using accuracy, confusion matrix, precision, recall, F1-score
- Visualization of precision-recall curves
- Misclassification sample inspection

# This subset should include *2500 images of cats* and *2500 images of dogs*, evenly distributed.

---

## Models Used

### 1. Custom CNN
- Simple convolutional network
- Data augmentation
- Binary classification using sigmoid

### 2. VGG16 Fine-Tuning
- Pretrained VGG16 (ImageNet)
- Custom top classifier head
- Phase 1: Feature extraction (frozen base)
- Phase 2: Fine-tuning last layers (block5)

---

##  Evaluation

Each model is evaluated using:
- Accuracy
- Confusion Matrix
- Classification Report (Precision, Recall, F1)
- Precision-Recall Curve
- Misclassified Image Examples

---

##  Observations
- VGG16 fine-tuning outperforms basic CNN
- Model performance is visualized via training/validation graphs
- Overfitting monitored using validation loss
- Sample misclassifications help understand weaknesses

---

##  Requirements

```bash
tensorflow
matplotlib
numpy
scikit-learn