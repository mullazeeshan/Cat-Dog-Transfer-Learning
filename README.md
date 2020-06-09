# Cat-Dog-Transfer-Learning
VGG on Cat Dog dataset using Transfer Learning. Model trained on Imagenet dataset

[Google Colab Notebook](https://drive.google.com/drive/u/1/folders/1X7PDVFYoXIVrVssLcImvcHVHlPGGkz1-)

## References:

[A Concise Brief to Transfer Learning](https://medium.com/@14prakash/transfer-learning-using-keras-d804b2e04ef8)|

[45 min read Transfer Learning with Real-World Applications in Deep Learning](https://towardsdatascience.com/a-comprehensive-hands-on-guide-to-transfer-learning-with-real-world-applications-in-deep-learning-212bf3b2f27a)|

# Basic CNN Performance 
![11](https://user-images.githubusercontent.com/29397302/84140465-4c838180-aa6f-11ea-93ac-2e891d509d61.png)

# VGG Transfer Learning
![12](https://user-images.githubusercontent.com/29397302/84140920-fc58ef00-aa6f-11ea-9869-84a270597d62.png)


## Getting Started:
Here I will explain how to get the data and run the notebook in your own environment. Also I will try to explain basics of Transfer Learning.

### Prerequisites
You will need Python 3.X.X with some packages which you can install direclty using requirements.txt.
> pip install -r requirements.txt

## Getting the Data
Run the notebook named Using_VGG_Transfer_Learning.ipynb which will download and extract the data in the first cell only. You can also run the Using_CNN_from_Scratch.ipynb notebook to compare performace with basic cnn model.

## Transfer Learning
In practice a very few people train a Convolution network from scratch (random initialisation) because it is rare to get enough dataset. So, using pre-trained network weights as initialisations or a fixed feature extractor helps in solving most of the problems in hand. Very Deep Networks are expensive to train. The most complex models take weeks to train using hundreds of machines equipped with expensive GPUs.

Transfer learning is a machine learning method where a model developed for a task is reused as the starting point for a model on a second task.

This form of transfer learning used in deep learning is called inductive transfer. This is where the scope of possible models (model bias) is narrowed in a beneficial way by using a model fit on a different but related task. The general idea is to use knowledge, that a model has learned from a task where a lot of labeled training data is available, in a new task where we don’t have a lot of data. Instead of starting the learning process from scratch, you start from patterns that have been learned from solving a related task.

For example, in computer vision, Neural Networks usually try to detect edges in their earlier layers, shapes in their middle layer and some task-specific features in the later layers. With transfer learning, you use the early and middle layers and only re-train the latter layers. It helps us to leverage the labeled data of the task it was initially trained on.

According to Demis Hassabis, the CEO of DeepMind Technologies, Transfer is also one of the most promising techniques that could someday lead us to Artificial General Intelligence (AGI).

## License
This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/mullazeeshan/Cat-Dog-Transfer-Learning/blob/master/LICENSE) file for details
