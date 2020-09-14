# NLP_Polority_Classification
To predict a reviews is positive or negative
## Data : 
movie reviews
## Processing : 
1. Remove stopword and words with POS like conjunction and prepositions which uncorrelated to our goal --classify the polority of th review
2. Stemming the word --- removing the suffix from a word and reduce it to its root word. 
   Ex: plays --> play, played --> play
3. Extract features by fitting CountVectorizer
## Model : 
1. LightGBM (F-socre 0.88)
2. Logistic Regression (F-socre 0.83)
      
