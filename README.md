# intensity_analysis_capstone_project
Intensity Analysis (Build your own model using NLP and Python) 
The objective of this project is to develop an intelligent system using NLP to predict the intensity in the text reviews. By analyzing various parameters and process data, the system will predict the intensity where its happiness, angriness or sadness. This predictive capability will enable to proactively optimize their processes, and improve overall customer satisfaction.

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


### Helper function description:
# Helper functions available in helper_function.ipny


### **Function 1** Visualize the sum of word count per intensity using a countplot
**def vizualize_word_count(dataframe):** Calling the helper function "vizualize_word_count(dataframe)"
  - input parameter : datafram
  - description : displays the countplot of for each intensity in the dataframe : lables each bar with the count
returns back with no return value.

### **Function 2** Visualization of dork count distributiper intensity using bar charton 
**def dist_word_count(data, column):* Calling the helper function "**dist_word_count(data, column)**"
  + input parameter :
       - data -> dataframe,
       - % column -> word_count_column
    + description : displays Bar chart, for the distribution of word_count of each intensity in the dataframe
    + returns back with no return value.
      ****

### **Function 3** cleaning of the review content
**def text_clean(text)
* Calling the helper function "**def text_clean(text)**"
    + input parameter :
        % text -> dataframe['content'],
    + description : for the text in the input parameter, the below cleaning operations are performed- converts to lower case
        - removes punctuations like ()!? and  [.*?\]
        - removes non alphanumeric characters
        - removes @ present in the text
        - removes # from the text
        - also removes http and www. from the text
    + returns cleaned_text.
    + Note: while calling this function iterate through each row of the dataframe or use apply function

**

### **Function 4** check for null content
**def check_null_content(data, count_column)**

* Calling the helper function "**def check_null_content(data, count_column)**"
    + input parameter :
        % data -> dataframe,
        % count_column -> word_count column
    + description : Checks the word_count column for zero value and masked the corresponding rows. And prints if null found or not
    + returns nothing.

### **Function 5** Print the difference in the content column
**def diff_content_column(data, column1, column2)**

### **Function 6** print the mean/average of the word per intensity
**def word_average_per_intensity(data, count_column):**)**
