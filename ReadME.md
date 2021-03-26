# Simple Transfer Learner

An example of transfer learning using [TensorFlow](https://www.tensorflow.org/) and [Keras](https://keras.io/)

For this task, we use a pre-trained model from google: [gnews-swivel-20dim](https://tfhub.dev/google/tf2-preview/gnews-swivel-20dim/1)
The dataset is: [The Internet Movie DataBase (IMDB) reviews data-set](https://colab.research.google.com/github/tensorflow/hub/blob/master/examples/colab/tf2_text_classification.ipynb#scrollTo=2ew7HTbPpCJH)

For each review, the pre-trained model returns a 20-dimensional vector,

We attach 2 layers to the pre-trained model:

* A 16 neuron [relu](https://en.wikipedia.org/wiki/Rectifier_(neural_networks)) layer to learn new data
* A 1 neuron [softmax](https://en.wikipedia.org/wiki/Softmax_function) output layer to classify each review into +ve/-ve class


After finetuning the new model, it can classify movie reviews into +ve/-ve classes,
The loss and accuracy scores are reported in the Jupyter Notebook.
