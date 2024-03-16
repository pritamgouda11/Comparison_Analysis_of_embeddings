# Comparison_Analysis_of_embeddings

## Part I Text Classification
**Approach 1:** Rule based classification
The rule-based classification works using a few hand-crafted rules. In sentiment classification, few words are associated with positive sentiment and few others with negative sentiment. 

EVALUATION of rule-based classifier with learnable weights is: 70.975

**Approach 2:** Bag-of-Words (BoW)
The BoW vector representations is based on the unordered counts of words piece of text (similar to a "bag" of words).

EVALUATION of BoW classifier is: 80.675

## Part II Word2Vec
Word2vec is one of the most popular techniques to learn word embeddings. The idea behind word2vec was that the meaning of a word is determined by the context in which it occurs. A word embedding is a learned representation for text where words that have the same meaning have a similar representation.

Word2vec model has 2 architectures:

**Continuous bag of word (CBOW):**
CBOW predicts the center word from the surrounding context words.

**Skip-gram:**
Skip-gram predicts surrounding context words from the center word.

EVALUATION: Precision at 5 for the analogy test is 0.1111111111111111

EVALUATION: Precision at 5 for the analogy test with Google skip-gram model is 0.0034
