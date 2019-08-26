# Cats And Dogs Classifier | Convolutional Neural Network with Python and Tensorflow 

Author: Rocky & Sandy

Contact: rockydtk@gmail.com & 

Convolutional Neural Networks are often called ConvNets, which is kind of Neural Network Architecture that are mostly used in Image Classification and ConvNets are very popular when it comes to processin Images. CNN was inspired by the Human Visual Cortex, So now we will use this method and apply to classifying cats and dogs.

![](model_explain.gif)

### EDA:
We are dealing with a train dataset of 25,000 images of dogs and cat. Luckily their names come with a pattern which has already classified them as dog or cat. Therefore, we used simple string slicing to generate label column for the dataset.  

### Model summary:
| Layer (type)                  | Output Shape         | Param   |
|-------------------------------|----------------------|---------|
| conv2d (Conv2D)               | (None, 126, 126, 32) | 896     |
| max_pooling2d (MaxPooling2D)  | (None, 63, 63, 32)   | 0       |
| conv2d_1 (Conv2D)             | (None, 61, 61, 64)   | 18496   |
| max_pooling2d_1 (MaxPooling2) | (None, 30, 30, 64)   | 0       |
| conv2d_2 (Conv2D)             | (None, 28, 28, 64)   | 36928   |
| flatten (Flatten)             | (None, 50176)        | 0       |
| dense (Dense)                 | (None, 64)           | 3211328 |
| dense_1 (Dense)               | (None, 2)            | 130     |

Total params: 3,267,778

Trainable params: 3,267,778

Non-trainable params: 0
