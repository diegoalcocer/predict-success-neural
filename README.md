# Machine Learning | Predict Success Neural
Binary classification models using deep neural networks to predict whether Alphabet Soup funding applicants will be successful

---

## Summary

It is very important to predict whether Alphabet Soup funding applicants will be successful, and to achieve this, I created a binary classification model using a deep neural network using the following these steps:

* Preprocess data for a neural network model: 
    * Encode the `categorical_variables` using the `OneHotEncoder()`
    * Concatenate the encoded categorical variables with the numerical variables using the Pandas `concat()` function
    * Ceate the features X and target y (column `IS_SUCCESSFUL`) datasets
* Use the model-fit-predict pattern to compile and evaluate a binary classification model
    * Output Neurons: 1
    * Hidden Nodes Layer 1: 58
    * Hidden Nodes Layer 2: 29
    * Epochs: 50
* Optimize the model.
    * First alternative Model *A1*: 
        * 3 layers and 50 epochs
        * 58, 29 and 14 neurons for each hidden layer respectively
    * Second alternative Model *A2*: 
        * 3 layers and 60 epochs
        * 60, 40 and 30 neurons for each hidden layer respectively  

After finishing the different models, the following are the accuracy scores achieved by each model.

```
Original Model Results
268/268 - 0s - loss: 0.5526 - accuracy: 0.7291 - 305ms/epoch - 1ms/step
Loss: 0.5525816082954407, Accuracy: 0.7290962338447571
``` 

```
Alternative Model 1 Results
268/268 - 0s - loss: 0.5532 - accuracy: 0.7305 - 344ms/epoch - 1ms/step
Loss: 0.5532207489013672, Accuracy: 0.7304956316947937
```

```
Alternative Model 2 Results
268/268 - 0s - loss: 0.5617 - accuracy: 0.7311 - 369ms/epoch - 1ms/step
Loss: 0.5617035627365112, Accuracy: 0.7310787439346313
```
As you can observe in the previous statistics, there is a slight improvement in the accuracy after each Model. The Model A2 has the higer accuracy. 

---
## Installation and Usage

```sh
git clone https://github.com/diegoalcocer/predict-success-neural
cd predict-success-neural/
```
To start the Jupyther Notebook you could launch the jupyter lab:

```sh
jupyter lab
```

### 📚 resources/

This project uses the following resources required for analysis 

* applicants_data.csv:  Contains a variety of information about each organization that have received funding from Alphabet Soup over the years, including whether or not it ultimately became successful 
* The Models saved as HDF5 files

---

## License

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
