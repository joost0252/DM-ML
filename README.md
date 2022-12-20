<img src="https://camo.githubusercontent.com/197d566e6ccf2e0f8c8f3e6fc1e2269c529674c119bb0d1573eaaa389f0c4ab3/68747470733a2f2f75706c6f61642e77696b696d656469612e6f72672f77696b6970656469612f636f6d6d6f6e732f372f37372f4c6f676f5f4845435f4c617573616e6e652e706e67" width="200" height="90" />

# Tudor Project : Four standard models and Neural Networks ! 
#### Authors: *Elena Martinez Ferradal and Joost Dijkstra*

<!-- TABLE OF CONTENTS -->
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
    </li>
    <li><a href="#results">Results</a></li>
  </li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

The purpose of this project is to predit the difficult level of given specific French Texts. Difficulty level is defined in six classes of international langauge levels (A1 to C2). 

These are the models used to classify texts difficulty in  this project. They are divided in 5 sections:
* Logistic Regression
* KNN 
* Decision Tree Classifier
* RandomForest Classifer 
* Neural Networks with PCA
The first four models are done withotut any data cleaning techiniques, the only data preparation is a simple vectorization. 
For Neural Networks, best results werer achieved with PCA (dimensionality reduction) any other complementary techinique was disregarded due to lower the accuracy. 
<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Functions

Here we are going to list the functions used across the colab notebook and explain briefly what they do: 

* One hote Encoding
* Evaluate
* DataLoader
* Losses

These funcitons are stored in Functions and explained there in more detail. 

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Classes

Here we are going to list the classes used across the colab notebook and what they do. 

* Net nn


<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started

The only prerequisities to run the code in the Collab Notebook are:

1. To upload the csv files required to train your models (training data) and do the predicitons (unlabel data).Optionally there is also a sample submission csv file in case you need to uplad your results into Kaggle. 
2. To download all the packages that are at the beginning of the notebook.
3. As explained before, the functions are in a separate file for clarity and will need to be imported. 

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- RESULTS -->
## Results



||Logistic regression|KNN|Decision Tree|Random Forest|Neural Networks|
| :---: | :---: | :---: | :---: | :---: | :---: |
|Precision|0.43||||
|Recall|||||
|F1-score|||||
|Accuracy |||||



<p align="right">(<a href="#readme-top">back to top</a>)</p>



