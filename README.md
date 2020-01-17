ALEXNET

This is a simple implementation of Alexnet, a deep convolutional neural network which won the ILSVRC in 2012. The code for model class is same as the official pytorch implementation. 

For better understanding the code and its implemenation refer to the medium articles linked below:
https://medium.com/@vivekvscool/image-classification-cnn-with-pytorch-5b2cb9ef9476

https://medium.com/@kushajreal/training-alexnet-with-tips-and-checks-on-how-to-train-cnns-practical-cnns-in-pytorch-1-61daa679c74a

Official Torchvision implementaion:
https://github.com/pytorch/vision/blob/61763fa955ef74077a1d3e1aa5da36f7c606943a/torchvision/models/alexnet.py#L14

The dataset used to train the model is a Kaggle dataset for classifying cats and dogs:
https://www.kaggle.com/c/dogs-vs-cats/data

The dataset contains 25,000 images of dogs and cats divided equally, 250 images were selected from each of the classes for the validation set. I have written a python script which selects images randomly from each of the classes' train set and puts them in the validation set.

Downloading datasets from Kaggle using the Kaggle api:
https://medium.com/@ankushchoubey/how-to-download-dataset-from-kaggle-7f700d7f9198

The model was trained on a GCP pytorch instance utilizing a Tesla-P4 gpu. You can also use a Google Collab instance and carry out training using the same code, it will be a bit tedious working with the data on the Collab notebook but it is completely doable.

Downloading Kaggle datasets to a Collab instance:
https://medium.com/@opalkabert/downloading-kaggle-datasets-into-google-colab-fb9654c94235
