
# Flight Price Prediction 

Flight prices are soaring high these days and people have started
travelling more and more these days. We might have often that Flight
Prices are so unpredictable. So, I decided to take this challenge and 
predict the prices of flights using Machine Learning.

The main objective of this project is to create an end to end Machine
learning system which predicts the flight of prices based on certain
inputs from user:

1) Airline
2) Arrival Date
3) Departure Date
4) Source
5) Destination
6) No. of Stops
## Screenshots

![App Screenshot](file:///C:/Users/sameer/Downloads/WhatsApp%20Image%202021-11-10%20at%209.00.03%20AM-converted.pdf)


## Roadmap
 Let us first understand the walkthrough of this project in detail.

The dataset originally had 7000 rows and 11 columns where Price was our dependent variables and other features were independent.
1) Importing Libraries and Dataset
2) Exploratory Data Analysis
3) Feature Engineering
4) Feature Selection
5) Hyperparameter tuning
6) Model Building
7) Deployment on Heroku





## Tech Stack

**Programming Language:** Python

**Libraries:** Numpy, Pandas, Seaborn, Matplotlib

**Tools/IDE:** Anaconda navigator, Jupyter Notebook

**Model used:** Random Forest using Randomized Search CV

**Backend:** Flask

**Deployment:** Deployed this model on Heroku
## Documentation

[Documentation](https://medium.com/@sameerkumar21635/flight-price-prediction-with-deployment-7d2f2b151fcc)

I have written a detailed document on entire project from dataset to
the deployment part and published that article on Medium.

Feature Engineering is the most important step in this project as it had many different type of features to play with. One feature was date of journey and I extracted the month and date of journey from that column to create new column using lambda function and datetime. I followed a similar approach for departure time and arrival time and extracted minutes and hours from it.

The features like Airline, Source, Destination and total stops were categorical variables and I applied One Hot encoding (nominal variable) and Label Encoding for ordinal variable(total stops)

I also performed Feature Selection using ExtraTreesRegressor method and correlation matrix using heatmap to visualize the important features which contributed to the target variable.

After building the model using Random Forest, I performed some hyper parameter tuning due to which accuracy got increased by 4%.

The last step was deployment and its steps are as follows:

1) Create model and the pkl file.
2) Create app.py using flask
3) Create templates folder to store your html file.
4) Create requirements.txt file: pip freeze > requirements.txt
5) Create procfile
6) Create account on Heroku and connect with github.
## Lessons Learned

One of the major challenges in this project was during Feature Engineering where I had to work on date time variables and extract date, month from that column and create a new column.

I used lambda function and apply function to extract that datetime functions present in python.


## Acknowledgements

 - [Datetime Python](https://docs.python.org/3/library/datetime.html)
 - [Randomized Search CV](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.RandomizedSearchCV.html)
 - [Feature Selection](https://machinelearningmastery.com/feature-selection-with-real-and-categorical-data/)

