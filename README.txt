Financial Risk Assessment - Machine Learning Project (RStudio + Databricks)


This project implements a financial risk classification model using two environments:
RStudio (for baseline ML model implementation)
Databricks (for High-Performance Computing / parallel model implementation)


RStudio Implementation

Files Included:
financial_risk_assessment.csv  
ML_ImplementationFileBy_2515288.rmd

Description:
This RMarkdown file performs end-to-end machine learning on the `financial_risk_assessment.csv` dataset. It includes:
Data Preprocessing and Cleaning
Exploratory data analysis
Unsupervised Learning
Model training (Random Forest)
Evaluation (confusion matrix, accuracy, etc.)

How to Run:
Open `ML_ImplementationFileBy_2515288.rmd` in RStudio.
Adjust the working directory to the location containing both the dataset and the implementation files.
Press “Knit” to create the report or execute the code step by step.

Required R Packages:
Install.packages(c(“ggplot2”, “validate” “, tidyverse” “, Hmisc” “, psych”, “e1071”, “VIM”, “corrplot”, “RColorBrewer”, ”caret”, “plotly”, “cluster”, ”mclust”, “caret”, “randomForest”, “rpart’ “pROC”, “MLmetrics”))


----------------------------------------------

Databricks Implementation

Files Included:
financial_risk_assessment.csv  
HPC_ImplementationFileBy_2515288.ipynb

Description:
This Jupyter notebook, designed for execution on Databricks, performs the identical machine learning task using PySpark for parallel processing. It encompasses:
Data loading and cleaning using PySpark
Feature engineering and vectorization
Unsupervised Learning 
Model training using RandomForestClassifier from pyspark.ml
Parallel processing on a Spark cluster
Performance evaluation using Spark ML metrics

How to Run:
Log in to your Databricks workspace.
Import HPC_ImplementationFileBy_2515288.ipynb via Workspace > Import.
Upload financial_risk_assessment.csv to the Databricks FileStore or use /dbfs/ path.
Attach the notebook to a running cluster (use Databricks Runtime 12.2 ML or later).
Run all cells from top to bottom.

Required Libraries:
PySpark libraries (included in Databricks runtime)
pandas (for minor data inspection)
imbalanced-learn (To Manage Unbalanced Data)
Seaborn (for data visualization)
Matplotlib (for plotting)
Sklearn (for confusion matrix)