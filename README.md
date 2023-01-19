# Implementing-Image-Recognition-for-Forest-Fire-Detections

With the use of convolutional neural networks (CNN), this study aims to identify the beginning or presence of a forest fire in a picture. The theory behind this model is that it might be used to analyse (aerial) surveillance footage of a forest in order to spot a fire or the beginning of a fire. Given that flames don't spread quickly, the model might be used in real-time to monitor low-framerate surveillance footage and inform users in the event of a fire.

# About Data
I added pictures from this category to the dataset by removing frames from films that depict the beginning of a fire since our tests indicated that the network had difficulty classifying'start fire' images. We used data augmentation tools offered by Keras to apply a number of random transformations (zooms, shifts, cropping, and rotations) on photos before they are fed to the network in order to train a network that extrapolates well to new images.

# Usage
Utilizing the routines defined in setup datasets.py, the datasets may be set up. Transfer learning.py, a module that has a function that specifies a batch generator that does data augmentation, contains the definition of the model we used to execute transfer learning from InceptionV3. The training procedure is also covered in this file, with the option to adjust the learning rate for fine-tuning and to freeze layers. The Python modules video annotation.py and evaluate model.py allow us to evaluate our model and mine challenging cases for the network, respectively.
