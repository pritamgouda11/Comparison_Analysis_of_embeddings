# Comparison_Analysis_of_embeddings

## Part I Text Classification
### **Approach 1:** Rule based classification
The rule-based classification works using a few hand-crafted rules. In sentiment classification, few words are associated with positive sentiment and few others with negative sentiment. 
```
EVALUATION of rule-based classifier with learnable weights is: 70.975
```
### **Approach 2:** Bag-of-Words (BoW)
The bag-of-words model is a model of text which uses a representation of text that is based on an unordered collection (or "bag") of words. It is used in natural language processing and information retrieval (IR). It disregards word order (and thus any non-trivial notion of grammar[clarification needed]) but captures multiplicity. 

![image](https://github.com/pritamgouda11/Comparison_Analysis_of_embeddings/assets/46958858/aed89113-d3f1-47c1-a1e8-572eccf6e31b)

```
EVALUATION of BoW classifier is: 80.675
```
## Part II Word2Vec
Word2vec is one of the most popular techniques to learn word embeddings. The idea behind word2vec was that the meaning of a word is determined by the context in which it occurs. A word embedding is a learned representation for text where words that have the same meaning have a similar representation.
Word2vec model has 2 architectures:

### **Continuous bag of word (CBOW):**

![image](https://github.com/pritamgouda11/Comparison_Analysis_of_embeddings/assets/46958858/0830706c-e5f3-446e-bf7e-ebbf0b819ef6)

The continuous bag-of-words (CBOW) model is a neural network for natural language processing tasks such as language translation and text classification. It is based on predicting a target word given the context of the surrounding words. The CBOW model takes a window of surrounding words as input and tries to predict the target word in the center of the window. The model is trained on a large text dataset and learns to predict the target word based on the patterns it observes in the input data. The CBOW model is often combined with other natural language processing techniques and models, such as the skip-gram model, to improve the performance of natural language processing tasks.

### **Skip-gram:**

![image](https://github.com/pritamgouda11/Comparison_Analysis_of_embeddings/assets/46958858/4d6c5101-5503-45e5-825b-46d7461564a1)

Skip-gram is one of the unsupervised learning techniques used to find the most related words for a given word. Skip-gram is used to predict the context word for a given target word. It's reverse of CBOW algorithm. Here, target word is input while context words are output.
```
EVALUATION: Precision at 5 for the analogy test is 0.1111111111111111
EVALUATION: Precision at 5 for the analogy test with Google skip-gram model is 0.0034
```
