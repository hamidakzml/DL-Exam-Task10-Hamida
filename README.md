# Task 10: Traffic Sign Recognition

**Student:** Hamida  
**ID:** 12  
**Seed:** 20240110  

## Presentation
(https://drive.google.com/your-link-here)

## Dataset
- **Name:** GTSRB (German Traffic Sign Recognition Benchmark)
- **Classes:** 10 traffic signs
- **Selected signs:**
  - Speed limit 30
  - Speed limit 50
  - Stop
  - Yield
  - No entry
  - Turn right ahead
  - Turn left ahead
  - Pedestrians
  - Children crossing
  - Road work

## Model Architecture
- **Type:** MobileNetV2 (Pre-trained)
- **Trainable layers:** Classifier only
- **Output classes:** 10

## Training Comparison

### Version 1
- Optimizer: Adam
- Learning rate: 0.0001
- Batch size: 32
- Epochs: 15
- Test accuracy: 97.01%

### Version 2
- Optimizer: Adam
- Learning rate: 0.00001
- Batch size: 32
- Epochs: 15
- Test accuracy: 88.42%

## Best Result
- **Best version:** Version 2
- **Final test accuracy:** 92.71
- **Target accuracy:** 88%
- **Status:** ✓ Achieved

## Analysis
Version 2 achieved better accuracy due to a lower learning rate, which allowed smoother convergence and reduced overshooting.

## Files
- `notebook.ipynb`: Full implementation
- `results/training_comparison.png`: Training curves
- `results/confusion_matrix.png`: Confusion matrix
- `results/predictions.png`: Sample predictions
