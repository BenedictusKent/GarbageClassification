# Garbage Classification

Using deep learning to classify garbage.  
Classification:
- Recycle
  - Plastic
  - Paper
  - Metal
  - Glass
- Trash   

Data used in this project is taken by ourselves.

## Installation

To clone this repo, use git command:

```bash
git clone https://github.com/BenedictusKent/GarbageClassification.git
```

## Steps
1. Load all images under ```img/own``` with size (220x220) and color.
2. Label images with the respective label by using integer or one-hot index provided by NumPy.
3. Take 10% of the images of every classes as test images and the rest for training and validation ```(TRAINVAL)```.
4. Every image is augmented using the function provided by TensorFlow and added to ```(TRAINVAL)```.
5. 10% of ```(TRAINVAL)``` is taken as validation data and the rest as training data.
6. Fit the data using the ```MobileNet``` neural network architecture [```ResNet50``` also provides similar accuracy of around 91%, though model saved is almost 5x bigger than ```MobileNet```. Purpose: to hopefully be able to put model on phone directly.]

## Future Update
1. Improve accuracy by increasing image augmentation.
2. Increase data set count.
3. Basic mobile app.