# Not_Hotdog_Model

In this notebook I will try to recreate a curious model used in an App shown in the HBO serie "Sillicon Valley". 

For this model, I will use the hotdog-nothotdog dataset from Kaggle, and to build the model my way to go was to use Tensorflow using Keras layers to build a Convolutional Neural Network and a pre-trained model to make use of transfer learning from the mobileNet v2 model.

Along the notebook and the code blocks, I will try to explain as best as I can what the building process of this model works and at the end obviously the results I got.

Hopefully I can also build the App as in the serie with this model I built, which is the first model I built by my own.

A detailed explanation of how the model was built take a look at the notebook attached in this repo.

You can found the google colab notebook in the following link:
- https://colab.research.google.com/drive/1ScYoJsGa-C5tqyyR5ETeA7pAgXwtwCx1#scrollTo=R0za6i4K4hkg

Here are the results I got.

## Results

### Training

For the training process I run it for 20 epochs, with a batch size of 32 and a learning rate of 0.0001. Using the mobileNet v2 and some more layers including dropout and image augmentation to prevent overfitting. The results I got were the following:

[![training][training-screenshot]]()

### Evaluation

For the evaluation process I used the validation set of the dataset and the results I got were the following:

[![evaluate][evaluate-screenshot]]()

### Predictions

For the predictions I used the test set of the dataset and the results I got were the following:

[![predictions][predictions-screenshot]]()


[training-screenshot]: public/training.png
[evaluate-screenshot]: public/evaluate.png
[predictions-screenshot]: public/predictions.png

