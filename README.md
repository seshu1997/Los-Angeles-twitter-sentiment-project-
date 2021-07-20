# Los-Angeles-twitter-sentiment-project


The goal of the project is to investigate the mental well-being (or sentiments) of Los Angeles twitter users in 2019.
More than 1 million geo-tagged tweets were scrapped from twitter for the purpose of the study. 
The tweets were cleaned and organized by week. In addition, crime incidence, arrest incidence, and temperature were collected as potential predictors that might influence the change of  sentiments. 
Various statistical models were implemented to closely examine the predictors' impacts on the sentiments.  

该项目的目的是研究2019年洛杉矶推特用户的心理健康（或情绪）。 出于研究的目的，我从推特上爬取了超过100多万条带有地理标记的推文，并将这些推文以周的单位进行了清理和整理。 
与此同时，我也收集了犯罪率，逮捕率， 和气温等可能影响情绪变化的因素的数据。多种统计模型被用来密切地研究这些因素对情绪的影响。

Where are the tweets? （爬取下来的推文原始数据链接）
- https://drive.google.com/file/d/18mpkkh5WkW5ZLOanDLiFhtukl5g3jhTY/view?usp=sharing

Key Components: 
1. Main.ipynb: 
  
  * Data Cleaning (数据清理）
      
    Tweets were loaded and were sorted by month, and then by week. 

    将推文倒入，先以月为单位分类整理，再以周为单位进行数据清理。 
        
* Sentiment Analysis （情绪分析）
      
  The obtained weekly sentiments were divided into a positivity (polarity > 0) group and a negativity group (polarity <0), with polarity = 0 as the reference point.  

  得到用户每周的情绪值并将情绪值以0为界限分为正面情绪组（情绪值 > 0)和负面情绪组(情绪值 < 0)。
        
* Text Mining/ NLP / Word Cloud （文本挖掘/自然语言处理/词云）
      
  In each sentiment group, high-frequency words were extracted from texts to form word clouds. 

  高频词被从每一个情绪组的文本中提出，并生成词云。
  
  
  
2. Predictors.ipynb:  
  
	Crime incidence, arrest incidence, and temperature were sorted by week. 
    
    犯罪率，逮捕率和气温数据被以周为单位进行归类整理。
      
3. Modeling.ipynb :
	    
     To compensate for the small size of the dataset, a sampling with replacement method was used to increase the validity of the statistical results. 
     Linear regression was used to study the correlation between the predictors and sentiments. 
     Statistical models including linear regression (LR), random forests(RF), and support vector machine (SVM) were implemented and compared to generate the best prediction. 
      
     为了弥补数据集规模较小的不足，重置抽样的方法被用来提高统计结果的有效性。
     线性回归方法被用来研究预测因素与情绪之间的相关性。统计模型，包括线性回归（LR），随机森林（RF）和支持向量机（SVM）被用来比较，以产生最佳预测。
 
 
Packages Involved （用到的包）:

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

