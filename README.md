# intensity_analysis_capstone_project
Intensity Analysis (Build your own model using NLP and Python) 
The objective of this project is to develop an intelligent system using NLP to predict the intensity in the text reviews. By analyzing various parameters and process data, the system will predict the intensity where its happiness, angriness or sadness. This predictive capability will enable to proactively optimize their processes, and improve overall customer satisfaction.

# Focus Areas:
	**Data Collection:** 
  + Gather all the intensity data, including the text and its intensity, from 3 files and combine together as concatenated_data.csv inside data/processed_data folder.
  + Helper function are written in helper_function.ipynb file and later run in intensity_analysis_capstone_project.ipynb file
	**Data Preprocessing:** Clean, preprocess, and transform the data to make it suitable for machine learning models.
Below are the steps involved in preparing text data for an NLP model using an intensity dataset:
- **Step 1: Remove duplicates**
- **Step 2: Cleaning text :** convert to lowercase, remove symbols, numbers and special character
- **Step 3: Cleaning and preprocessing :** Stop word removal
- **Step 4: Spelling correction:** (continued as NLP data preprocessing in 3rd file)
- **Step 5: Word segmentation :** split the combined words
- **Step 6: Expand contractions :** like dont -> do not and so on
- **Step 7: Spelling correction:** using TextBlob
- **Step 8: Stemming and Lemmatization**

  
	**Exploratory Data Analysis (EDA)** for intensity analysis data involves examining the characteristics and patterns of intensity measurements using below steps

1.	#### Understand the Data
2.	#### Summarize statistic
3.	#### Vizualization of data (Visuals stored in visual folder)
    + Text Review count for each intensity
    + Visualize the distribution of word count for each intensity using a bar chart after stop word removal
    + Bar chart vizualisation of n-gram words for each intensity (n-gram can be choosen dynamically)
    + Word cloud all the words
    + Word cloud for each intensity separately
 
	**Feature Engineering:** Extract relevant features and identify key process variables that impact intensity.
  + Performed CountVectorization, TfidfVectorisation, BOW
    
	**Model Selection:** Choose appropriate machine learning algorithms for intensity classification.
    + Tried logistic regression, RandomForest, Naive Bayers Model, SVM, Kerbas
	**Model Training:** Train the selected models using the preprocessed data.
	**Model Evaluation:** Assess the performance of the trained models using appropriate evaluation metrics.
	**Hyperparameter Tuning:** Optimize model hyperparameters to improve predictive accuracy.










