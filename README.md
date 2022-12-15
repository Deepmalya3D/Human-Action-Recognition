# Human Action Recognition using CNN and Transfer Learning

Human Action Recognition (HAR) aims to understand human behavior and assign a label to each action. It has a wide range of applications, and therefore has been attracting increasing attention in the field of computer vision. Human actions can be represented using various data modalities, such as RGB, skeleton, depth, infrared, point cloud, event stream, audio, acceleration, radar, and WiFi signal, which encode different sources of useful yet distinct information and have various advantages depending on the application scenarios.

In the project, I have performed image classification of human actions using Convolutional Neural Networks. The dataset features 15 different classes of Human Activities, with 12k+ labelled and 5.4k unlabelled images. Initially, I created a few custom CNNs and fit the training data to the neural networks. I managed to achieve 35% accuracy, which is not much but still better than random guess.

Next, I used transfer learning to increase the accuracy. Transfer learning is a research problem in machine learning that focuses on storing knowledge gained while solving one problem and applying it to a different but related problem. I used EfficientNet-b0 as the starting point of our new model. EfficientNet-b0 is a convolutional neural network that is trained on more than a million images from the ImageNet database. The network can classify images into 1000 object categories, such as keyboard, mouse, pencil, and many animals. I tuned the hyperparameters of this model a bit and added two more dense layers. Finally I managed to reach % accuracy on the validation data.

`DataSet`: [link](https://www.kaggle.com/datasets/meetnagadia/human-action-recognition-har-dataset)
