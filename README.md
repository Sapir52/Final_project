# Microtrends in hightech job ads 

# The project's target

The goal of the project is to develop a model for identifying trends in job ads in Israeli high-tech.   
The model will enable the forecasting of the skills required for graduates and professionals to find work in the Israeli high-tech field, 
taking into account the type of job and company.                         
The final result of the process is predicting future values of the words based on previously observed values. 
Another goal is to characterize which words/ terms are similar to each other by using clusters.

# DataSet

The project is based on a database containing job vacancies in the Israeli high-tech field taken from 
four different sites: LinkedIn, Glassdoor, AllJobs, JobMaster. 
The database built lists 11 titles and contains over 1000 job ads in Israeli high-tech. 

# method
The project is based on the NLP method that allows the creation of a prediction model by LSTM.

# Pipeline 
* Arranging the ads by time of publication and division into time windows.  
* Preprocessing of the text which included division into sentences, tokenization, removal of stop words, removal of special characters and creation of multiple-words.                                 
* Words and phrases were represented as vectors by two methods: TF-IDF and Word2Vec.                
* In order to identify the importance  of words and word groups, various algorithms were run from the NetworkX library. In addition, K-means and Text-Rank.   
* Finally, the frequency of word occurrence was predicted using a neural network by creating models for words and clusters.


# results
The results of the model prediction for the different types of vector representation.

The model evaluation is based on the results of various regression-type loss functions.

* Note: Models whose loss function is pink are very flat predicted.

Words prediction:

![TAB11](https://user-images.githubusercontent.com/63209732/123255952-13427600-d4f9-11eb-8692-7fa6b77f2ba1.png)

Clusters prediction:

![TAB22](https://user-images.githubusercontent.com/63209732/123255966-15a4d000-d4f9-11eb-94a1-698cb0ca472b.png)

