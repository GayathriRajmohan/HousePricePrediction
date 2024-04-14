# HousePricePrediction
## HousePricePrediction
Develop a machine learning model to predict the sale price of residential properties based on various features such as location, size, amenities, and other relevant factors. The goal is to create an accurate and reliable predictive model that can assist homeowners, real estate agents, and property investors in estimating the market value of houses, thereby facilitating informed decision-making processes in buying, selling, or investing in residential real estate properties.

##  Generic Flow Of Project
![flow1](https://github.com/GayathriRajmohan/HousePricePrediction/blob/main/HousePricePrediction/output/workflow.png)

## Dataset

[Download the dataset  from here](https://www.kaggle.com/datasets/aariyan101/usa-housingcsv)

## 1. Starting the Project Folder
Installation: Install Django and  install the necessary modules using  this commands:

```

pip install pandas
pip install matplotlib
import os
pip install seaborn
pip install scikit-learn

```
To start the project use this command
```
django-admin startproject HOUSEPREDICTION
cd HOUSEPREDICTION
```
To start the app use this command
```
python manage.py startapp HousePrediction
```

setting.py: In this file, we import ‘os‘ and connect templates to the folder by using the following ‘os.path.join’ code. To connect the ‘templates’ folder with the ‘settings.py’ file, add the following code line to the ‘TEMPLATES’ section of the ‘settings.py’ file, as shown in the image.

![tem1](https://github.com/GayathriRajmohan/HousePricePrediction/blob/main/HousePricePrediction/output/template.png)

view.py: The dataset is read from the ‘USA_Housing.csv’ file, and the ‘Address’ column is dropped.The independent variables (X) and the dependent variable (Y) are separated.The data is split into training and testing sets using train_test_split.A Linear Regression model is created and fitted to the training data.User input values are obtained from the GET request.A prediction is made using the model.The prediction is rounded to an integer.A message containing the predicted rent is created.Finally, the ‘predict.html’ file is rendered with the prediction result.

## 2.Deployement of the Project
Run the server with the help of following command:
```
python3 manage.py runserver
```
## 3.Output
![Output1](https://github.com/GayathriRajmohan/HousePricePrediction/blob/main/HousePricePrediction/output/hs1.png)
![Output2](https://github.com/GayathriRajmohan/HousePricePrediction/blob/main/HousePricePrediction/output/hs2.png)
![Output3](https://github.com/GayathriRajmohan/HousePricePrediction/blob/main/HousePricePrediction/output/Hs3.png)
![Output4](https://github.com/GayathriRajmohan/HousePricePrediction/blob/main/HousePricePrediction/output/hs4.png)
The accuracy of the prediction system is 80% according to the linear regression algorithm.
