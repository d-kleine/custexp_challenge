# Fashion Shop Gender Prediction Model
## Introduction

This GitHub repository contains the code and files necessary to build a gender prediction model for an e-Commerce Fashion Shop. The goal is to create a model that can predict the gender of customers based on their browsing behavior, enabling the shop owner to dynamically customize the webpage layout to provide the best possible shopping experience for each customer.

## Task description

The task is to build a machine learning model using the data provided in *train.csv* to predict the gender of registered customers. The data in *train.csv* contains the following columns:

* `user_id`: Unique identifier for each customer.
* `path`: The URL path visited by the customer, which represents the product category.
* `timestamp`: The timestamp of the page visit, indicating the time of page load.
* `gender`: The gender of the customer (the target variable).

The path column corresponds to the URL path visited by the user. After training the model, the model will be used for *test.csv* to predict the gender of registered or non-registered customers.


## Approach

To build the gender prediction model, it will follow these steps:
* **Data Preprocessing**: 
    * Clean and preprocess the data, handle missing values, and convert categorical features into numerical representations suitable for machine learning algorithms.
* **Feature Engineering**: 
    * Extract relevant features from the timestamp and path columns to enhance the model's predictive power.
* **Model Selection**: 
    * Choose a suitable machine learning algorithm (e.g., logistic regression, random forest, or neural network) to train the model.
* **Model Training**: 
    * Train the selected model on the preprocessed training data to learn the patterns in the customer's browsing behavior and their associated gender.
* **Model Evaluation**: 
    * Evaluate the trained model's performance using appropriate metrics to ensure it provides accurate gender predictions.
* **Prediction**: 
    * Once the model is trained and evaluated, it will be used to predict the gender of customers in the *test.csv* dataset.

## Files in the Repository
* *train.csv*: The training dataset containing `user_id`, `path`, `timestamp`, and `gender`.
* *test.csv*: The test dataset containing `user_id`, `path`, and `timestamp` for which we need to predict the gender.

## Instructions

To replicate the model training and make predictions, follow these steps:

1. Clone this repository to your local machine.
2. Install the required dependencies as mentioned in *requirements.txt*.
3. Open the Jupyter Notebook *gender_prediction.ipynb*.
4. Execute the notebook cells sequentially to perform data preprocessing, train the model, and make predictions on the test data.
5. The predictions for the test dataset will be stored in a file named *predictions.csv*.

## Conclusion

With this gender prediction model, the Fashion Shop owner can predicted gender of the customers, providing them with a personalized and enjoyable shopping experience.