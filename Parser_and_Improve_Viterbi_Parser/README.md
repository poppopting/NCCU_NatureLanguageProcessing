# Parsing_and_Improve_Viterbi_Parser
Final task: imporve to handle different unknown words

## Processing
First we check each word by runnning "grammar.check_coverage()" , if there is an error(the word is unknown in PCFG):

1. Keep searching hypernyms of the word by wordnet until pass grammar.check_coverage()
2. If the word not in wordnet, we get POS by nltk.pos_tag and then randomly select a word with the same POS in NLTK  words until pass grammar.check_coverage()

When we complete raplacing the unknown words, we store the original word, POS and replaced word and begin parsing the sentence.After pasrsing the sentence, we can use tree.pformat() to replace the original word and POS and complete the task by running "print".
   
## Example:   
Input: 
```
I shot an elephant my pajamas.
```
Ouput: 
```
(S
  (NP-SBJ (PRP I))
  (VP
    (VBD shot)
    (NP (DT an) (NN elephant))
    (NP (PRP$ my) (NN pajamas)))
  (. .))
```
