# CS-210-Project-Repository
CS 210 Term Project Repository (Databees)


Jupyter Notebooks:

ExtractingWebsite.jpynb: This notebook converts the 2 COVID-19 tables (one weekly, one daily) in the Ministry of Health's website to excel files. 

ExtractingLabDataset.jpynb: This notebook converts the authorized laboratory table in the Ministry of Health's website to an excel file. 

Analysis_Of_Lab_Dataset.jpynb: This notebook changes the language of the extracted excel file from Turkish to English. Also, additional "Region" column is added. Then, there are 2 graphs (1 for distribution of labs by province, 1 for distribution of labs by region).

Analysis_Of_COVID19_Dataset.jpnyb: This notebook changes the language of the extracted excel file (Daily Covid 19 Dataset) from Turkish to English. Missing cells are filled as much as possible. Also 3 new columns are added : Month, Year, Season. Correlation analysis were done on specifically 3 columns: "# Daily Deaths", "# Heavy Patients" and "Flu Percentage". "Flu Percentage" and "# Heavy Patients" were not correlated with anything enough to fill their missing values. Because of that we dropped those columns. The cleaned dataset will be used for Machine Learning.

Using_Machine_Learning.jpnyb: This notebook uses the cleaned dataset from "Analysis_Of_COVID19_Dataset.jpynb" to train Machine Learning models. "Year", "Month", "Season" columns are converted to numbers with .getdummies() method. Columns that contain Total values are dropped since this model works on daily data. Linear Regression, KNN, Polynomial Regression, Decision Tree and Random Forest models were trained with the dataset. The best performing model was Random Forest. Each models's error rates are printed in the notebook and their performances are plotted as well.

Data_Visualization.jpynb: This notebook contains many graphs from the cleaned dataset. These graphs provides insights to understand the data. 

