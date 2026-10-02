# Real vs AI-Generated Image Classifier

**Problem:** Classify whether an image is real or AI-generated.

**Dataset:** CIFAKE (100,000 training and 20,000 test images, from Kaggle).

**Method:** Transfer learning with MobileNetV2 (pretrained on ImageNet) + a new classification layer.

**Result:** 88.3% test accuracy after 3 epochs.

**Tools:** Python, TensorFlow/Keras, matplotlib.

## Limitations

The model was trained only on CIFAKE, which contains small 32x32 images from one source. Because of this, it may misclassify high-resolution photos or images from other AI generators.
