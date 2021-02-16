# TextClassification
Applied Natural language processing (NLP) to train and evaluate 7 digital books from NLTK gutenburg.

## Overview
The goal of the project is to classify each word from seven different books from NLTK Gutenburg libraries after training. The code contains two main parts. First, data cleansing and preprocessing are performed to prepare for the training models. The second part includes feature engineering, training, testing and error analysis.

## Environment
Python version: 3.X

Develop platform: Google Colab


## Prerequisite
The libraries we used include: nltk, sklearn, numpy, matplotlib.pyplot, pandas, spacy, seaborn.

If you use Colab to run the code, it is not necessary for you to install the external libraries yourself.

## How to run
The code [TextClassificationNLP.ipynb](https://github.com/damien2012eng/TextClassification/blob/main/TextClassificationNLP.ipynb) was developed on Google Colab, so it is easy to open it through Colab and run the code cell sequently.


Also feel free to open and run the code through jupyter notebook or jupyterLab.


In the function ` main() `, there are several key execute parameters you can modify:
``` Python
    ########### EXECUTE ################
    train_list = ['svm']
    n = nlp_1(documents, shuffle=1)
    n.transform(type='2-gram', tf_idf=False)
```
In the `train_list`, you can add the one or more algorithms you want to play with. The parameters are `'decision tree'`, `'svm'`, `'linear regression'`, `'mlp'`, `'gaussian naive bayes'` and `'knn'`. Decision tree is the defalt algorithm.

In the parameters of `n.transform(type=  , tf_idf=  )`, you can define the type of transform. The parameters of `type` are `'bow'`, `'3-gram'` and `'2-gram'`. The parameter of `'tf_idf` is boolean(True or False), which define whether it will do tf-idf or not. BOW and tf-idf False is the defalt parameter.

## Results

![alt text](https://github.com/damien2012eng/TextClassification/blob/main/src/images/algorithmsComp.png?raw=true)
<p align="center">Fig. 1 Performing algorithms comparison among 5 ML. algorithms and 3 feature learning methods </p>


![alt text](https://github.com/damien2012eng/TextClassification/blob/main/src/images/confusionMatrix.png?raw=true)
<p align="center">Fig. 2 Confusion Matrix with algorithm KNN and TF-IDF </p>
