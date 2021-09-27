# Los-Angeles-twitter-sentiment-project


The goal of the project is to investigate the mental well-being (or sentiments) of Los Angeles twitter users in 2019.
More than 1 million geo-tagged tweets were scrapped from twitter for the purpose of the study. 
The tweets were cleaned and organized by week. In addition, crime incidence, arrest incidence, and temperature were collected as potential predictors that might influence the change of  sentiments. 
Various statistical models were implemented to closely examine the predictors' impacts on the sentiments.  



Where are the tweets? 
- https://drive.google.com/file/d/18mpkkh5WkW5ZLOanDLiFhtukl5g3jhTY/view?usp=sharing

Key Components: 
1. Main.ipynb: 
  
  * Data Cleaning 
      
    Tweets were loaded and were sorted by month, and then by week. 

    
        
* Sentiment Analysis 
      
  The obtained weekly sentiments were divided into a positivity (polarity > 0) group and a negativity group (polarity <0), with polarity = 0 as the reference point.  

  
        
* Text Mining/ NLP / Word Cloud 
      
  In each sentiment group, high-frequency words were extracted from texts to form word clouds. 

  
  
  
  
2. Predictors.ipynb:  
  
	Crime incidence, arrest incidence, and temperature were sorted by week. 
    
    
      
3. Modeling.ipynb:
	    
     To compensate for the small size of the dataset, a sampling with replacement method was used to increase the validity of the statistical results. 
     Linear regression was used to study the correlation between the predictors and sentiments. 
     Statistical models including linear regression (LR), random forests(RF), and support vector machine (SVM) were implemented and compared to generate the best prediction. 
      
 
 
Packages Involved:

  json
  
  matplotlib
  
  numpy
  
  nltk
  
  panda
  
  re
  
  requests
  
  ssl
  
  seaborn
  
  sklearn
  
  statsmodels
  
  textblob
  
  wordcloud

