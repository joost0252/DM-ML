<img src="https://camo.githubusercontent.com/197d566e6ccf2e0f8c8f3e6fc1e2269c529674c119bb0d1573eaaa389f0c4ab3/68747470733a2f2f75706c6f61642e77696b696d656469612e6f72672f77696b6970656469612f636f6d6d6f6e732f372f37372f4c6f676f5f4845435f4c617573616e6e652e706e67" width="200" height="90" />

# Tudor Project : Four standard models and Neural Networks ! 
#### Authors: *Elena Martinez Ferradal and Joost Dijkstra*

<!-- TABLE OF CONTENTS -->
<a name="readme-top"></a>
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#functions">Functions</a></li>
      </ul>
      <ul>
        <li><a href="#classes">Classes</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
       <ul>
        <li><a href="#recommendations-for-evaluation">Recommendation</a></li>
      </ul>
    </li>
    <li><a href="#results">Results</a></li>
  </li>
      </li>
    <li><a href="#video">Video</a></li>
  </li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

The purpose of this project is to predit the difficult level of given specific French Texts. Difficulty level is defined in six classes of international langauge levels (A1 to C2). 

These are the models used to classify texts difficulty in  this project. They are divided in 5 sections:
* Logistic Regression 📈
* KNN 📌
* Decision Tree Classifier🌳
* RandomForest Classifer 🌳🌳🌳
* Neural Networks with PCA 🌀

The first four models are done withotut any data cleaning techiniques, the only data preparation is a simple vectorization. 
For Neural Networks, best results werer achieved with PCA (dimensionality reduction) any other complementary techinique was disregarded due to lower the accuracy. 
<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Functions

Here we are going to list the functions used across the colab notebook and explain briefly what they do: 

* Evaluate

The function uses the precision_score, recall_score, f1_score, confusion_matrix, and accuracy_score functions from the sklearn.metrics module to compute these metrics. The average parameter specifies how the scores should be averaged across the different classes, with the 'weighted' option indicating that the scores should be weighted by the number of true samples in each class.

The function prints the computed metrics to the console for easy visualization. You can use this function to evaluate the performance of a classifier on a test set and identify areas for improvement.

* Encode_difficulty

This function encodes the difficulty column of a corpus data frame as ordinal values. It converts categorical variables into numerical values, which can be used as input to models that do not handle categorical data natively. The encoded values retain the ordinal relationships between the categories, meaning that the encoded values can be treated as numerical data in certain contexts (e.g., for comparison purposes).

* Prepare_submission

The purpose of this function is to prepare the data frame in a format that conforms to the submission requirements of the Kaggle competition. The function ensures that the difficulty column has the correct categories and that the data frame does not contain any unnecessary columns.

* Get_prediction_probabilities

This function takes in a pipeline object and a data frame containing a 'sentence' column. It returns an array of the predicted class probabilities for each sentence, as obtained by calling the predict_proba method on the pipeline object and taking the maximum probability along the row-wise dimension of the resulting array. The function also prints the minimum and maximum values of the extracted probabilities.

These funcitons are stored in Functions and explained there in more detail. 

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Classes

Here we are going to list the classes used across the colab notebook and what they do. 

* Net()

The Net class can be used to define a simple feedforward neural network with two hidden layers for binary classification tasks. To use the model, you would first create an object of the Net class, specifying the number of input units (D_in), the number of hidden units (H), and the number of output units (D_out). Then, you would pass an input tensor through the model by calling the forward method on the object, which would return the output of the model.

* Data()

The Data class is useful for creating a dataset object that can be used to train a PyTorch model. The __getitem__ and __len__ methods allow the dataset to be indexed and iterated over in a consistent way, making it easy to use in a PyTorch data loader.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started

The only prerequisities to run the code in the Collab Notebook are:

1. To upload the csv files required to train your models (training data) and do the predicitons (unlabel data).Optionally there is also a sample submission csv file in case you need to uplad your results into Kaggle. 
2. To download all the packages that are at the beginning of the notebook.
3. As explained before, the functions are in a separate file for clarity and will need to be imported. 

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Recommendations for evaluation

1. Read this Readme
2. Open the Google Collab (dont' run the code it will take 20 min)
3. Watch the video with the code on one side


<!-- RESULTS -->
## Results



||Logistic regression|KNN|Decision Tree|Random Forest|Neural Networks|
| :---: | :---: | :---: | :---: | :---: | :---: |
|Precision|0.4667|0.3940|0.3208|0.4208|0.4802
|Recall|0.4667|0.3373|0.3079|0.4084|0.4789
|F1-score|0.4667|0.4111|0.3246|0.4267|0.4844
|Accuracy |0.4667|0.3490|0.3208|0.4180|0.4802



<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- VIDEO -->
## Video



wwww.youtube.com



<p align="right">(<a href="#readme-top">back to top</a>)</p>


