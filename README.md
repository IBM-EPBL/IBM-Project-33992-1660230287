# IBM-Project-33992-1660230287
Web Phishing Detection
## Introduction

The Internet has become an indispensable part of our life, However, It also has provided opportunities to anonymously perform malicious activities like Phishing. Phishers try to deceive their victims by social engineering or creating mockup websites to steal information such as account ID, username, password from individuals and organizations. Although many methods have been proposed to detect phishing websites, Phishers have evolved their methods to escape from these detection methods. One of the most successful methods for detecting these malicious activities is Machine Learning. This is because most Phishing attacks have some common characteristics which can be identified by machine learning methods.

## Requirements

The Code is written in Python 3.7.11, make sure you have a python version higher or same as it.The required packages and libraries to run this project on localhost are stated on requirements.txt file. To install the libraries open command prompt and use the command in the project directory after cloning the repository:
```bash
pip install -r requirements.txt
```
After the installation is completed, use the command to activate environment and copy the localhost url on you browser to run the application:
```bash
python app.py
```
## DataSet

Download dataset from [here](https://drive.google.com/file/d/18PuytIZWvNQCnMypKdaQjAqqQ0MRZ0uj/view?usp=sharing).Train it in IBM cloud [click for tutorial](https://youtu.be/TysuP3KgSzc). Then train the dataset to get more accurate detection.

## Web Phishing Detection

![image](https://github.com/IBM-EPBL/IBM-Project-33992-1660230287/blob/main/Project%20Development%20Phase/Sprint%204/Legit%20website.png)

![image](https://github.com/IBM-EPBL/IBM-Project-33992-1660230287/blob/main/Project%20Development%20Phase/Sprint%204/Phishing%20site.png)

## Result

Accuracy of various model used for URL detection
<br>

<br>

||ML Model|	Accuracy|  	f1_score|	Recall|	Precision|
|---|---|---|---|---|---|
0|	Gradient Boosting Classifier|	0.974|	0.977|	0.994|	0.986|
1|	CatBoost Classifier|	        0.972|	0.975|	0.994|	0.989|
2|	XGBoost Classifier| 	        0.969|	0.973|	0.993|	0.984|
3|	Multi-layer Perceptron|	        0.969|	0.973|	0.995|	0.981|
4|	Random Forest|	                0.967|	0.971|	0.993|	0.990|
5|	Support Vector Machine|	        0.964|	0.968|	0.980|	0.965|
6|	Decision Tree|      	        0.960|	0.964|	0.991|	0.993|
7|	K-Nearest Neighbors|        	0.956|	0.961|	0.991|	0.989|
8|	Logistic Regression|        	0.934|	0.941|	0.943|	0.927|
9|	Naive Bayes Classifier|     	0.605|	0.454|	0.292|	0.997|

## Conclusion
1. The final take away form this project is to explore various machine learning models, perform Exploratory Data Analysis on phishing dataset and understanding their features. 
2. Models are trained and tested in IBM cloud and Flask is integrated to it. 
3. The final conclusion on the Phishing dataset is that the some feature like "HTTTPS", "AnchorURL", "WebsiteTraffic" have more importance to classify URL is phishing URL or not. 
4. Gradient Boosting Classifier currectly classify URL upto 97.4% respective classes and hence reduces the chance of malicious attachments.
5. This web application can be further developed to create a chrome extension , so as when ever a user explore a website a notification indicating if the website is safe or malicious can be popped automatically. Thus reducing the fraud effectively.


