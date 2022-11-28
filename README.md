# AutoML_TFIDF

## Automated tf-idf Vector Space Model Recommendation System    

Recommendation systems are one of the major usage of machine learning nowdays.    

This open source library is built to utilize process of building    

### content based filtering recommendation system using tf-idf vector space model

Provided by Team Memebers: Kim Juhyeong, Lee JunHyeok, Seo JiWon and Park YeJin    
From Term Project of 2022-2 Machine Learning Lectures, Prof. Won Kim    
Gachon Univ. School of Computing

## Requirements

Pandas

NumPy

Scikit-Learn

nltk     

For nltk download requirements: 'stopwords', 'punkt', 'averaged_perceptron_tagger', 'wordnet', 'omw-1.4' 
These can be easily installed by 

<code>download_nltk_requirements()</code>

# Function Definition & Description 

## recommend_by_name (...)

![image](https://user-images.githubusercontent.com/90828283/204347044-f3a2cc2a-3655-40a5-b151-78eb0042f64b.png)

recommendation 

<code>recommend_by_name(df,name, target_col, N, columns,do_ascending=False, rating="rating", name_col="name")</code>

df: input data (DataFrame)   
name: name of the item to be base of the recommendation. Recommendation will be made with comparing bag of words of the item with this name    
target_col:  target column to be set as bag of words    
N: N elements to be returned (recommended)
columns: columns of N elements to be returned with (recommendation)    
     
## recommend_by_description (...)

![image](https://user-images.githubusercontent.com/90828283/204347320-4f2c667f-84d7-4f72-ac78-f2d1a03ac41b.png)

<code>recommend_by_description(df, description ,N, target_columns, columns, do_ascending=False)</code>

df: input data (DataFrame)   
name: name of the item to be base of the recommendation. Recommendation will be made with comparing bag of words of the item with this name    
target_columns:  target columns to be set as bag of words    
N: N elements to be returned (recommended)
columns: columns of N elements to be returned with (recommendation)    

# References

Notebook of Zomato dataset analysis from Kaggle :  https://www.kaggle.com/code/chirag9073/zomato-recommendation-system


