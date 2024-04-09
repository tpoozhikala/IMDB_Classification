# IMDB_Classification
![IMDB-Logo](https://github.com/tpoozhikala/IMDB_Classification/blob/main/Assests/IMDb_Logo.wine.png)

Provide a quick and accurate deep learning neural network image classification model for Family Friendly Productions, movie production company, to predict the movie genre based on IMDB poster image data before their upcoming movies hit the market. This is to give the Marketing team more focused insights to tune their respective marketing methods(Facebook and Instagram Advertising) to target their specific audience members so that Family Friendly Productions will be positive by the end of 2024 financial year. 

## Data Wrangling
In order to begin steps of model development, an intial dataset was retrived throguh a paid IMDb API to get PG and G movie data from 1990 to 2023 with json loads and python get requets. The dataset was then assessed and filtered out for null values within the 'image' and 'genre' columns as values are needed in both columns for the image classificaiton model.  

|         | count_missing     |
| ------- | --- |
| image | 86 | 
| genre | 45 | 

Further steps detailed in the [Data Wrangling Notebook] 

## Exploratory Data Analysis
A comprehensive breakdown between the different genre class representation of movies provided within [EDA Notebook](https://github.com/tpoozhikala/Bank-Churnrate/blob/main/3_EDA/03_EDA_Bank_Churnrate.ipynb).

## Pre-Processing
Method to generate 80/20 train test splits for the datasets of numpy RGB values for movie poster image array and a genre label dataframe given within [Preprocessing Notebook](https://github.com/tpoozhikala/Bank-Churnrate/blob/main/4_Preprocess_and_Training/04_Preprocess_and_Training_Bank_Churnrate.ipynb).

## Training and Modeling
Keras Image Classificaiton model development and training steps detailed in [Training_and_Modeling Notebook](https://github.com/tpoozhikala/Bank-Churnrate/blob/main/5_Modeling/05_Modeling_Bank_Churnrate.ipynb)

Results regarding best model performer and correspdoing ROC AUC values for few genres were: 
| Model Name | f1_score | ROC_AUC_Comedy  | ROC_AUC_Adventure | ROC_AUC_Drama | ROC_AUC_Documentary |
| ------- | --- | --- | --- | --- | --- | 
| Keras Image Classification Model | 	0.25258895 |	0.4978308 |	0.49173069 | 	0.49308443 | 	0.503067484 |	

## Results/Conclusion
Improvements will need to be implemented before model can be delployed to production such as increasing sample size of genres and performing 5-fold cross validation instead of 3-fold. 
Further remarks detailed in [Final Project Report](https://github.com/tpoozhikala/Bank-Churnrate/blob/main/6_Documentation/Bank_Churn_Rate_Final_Project_Report.pdf)

## Future Work
Future work will be not only increasing the sample size of genres and performing 5-fold cross validation instead of 3-fold, but also to further fine tune the Image Classification model by finding optimal layers, as well as expanding GridSearchCV parameters.
Again further remarks found in [Final Project Report](https://github.com/tpoozhikala/Bank-Churnrate/blob/main/6_Documentation/Bank_Churn_Rate_Final_Project_Report.pdf)

## Acknowledgments
The author would personally like to thank Springboard Mentor [Eric Callahan](https://www.linkedin.com/in/ericcallahan/) for his guidance and support throughout this project development.