# Improve_word_segmentation
Improve word segmentation with CRF
## Data : 
source: http://sighan.cs.uchicago.edu/bakeoff2005/
## Processing : 
1. Add word position information and bigram trigram features
2. Collect surround word and add above features
## Model : 
   CRF (F-socre 0.93)
## Compare with jieba
   jieba (F-socre 0.82)
      
