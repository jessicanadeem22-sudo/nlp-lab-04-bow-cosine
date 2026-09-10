

# NLP Lab Exercise 04
## Vector Space Model (BoW) & Cosine Similarity

### Course
Natural Language Processing

### Task 1: Bag of Words Matrix

This task implements the Bag of Words model using CountVectorizer.

### Output

Vocabulary:

['amazing' 'bad' 'customer' 'fast' 'great' 'performance' 'product' 'service' 'terrible']

Bag of Words Matrix:

[[1 0 0 1 0 1 1 0 0]
 [0 0 0 1 1 1 0 1 0]
 [0 1 1 0 0 1 0 1 1]]

### Task 1 Screenshot

<img width="631" height="223" alt="image" src="https://github.com/user-attachments/assets/f32a469d-9baf-4ad5-92a6-fad9cfa21d08" />

---

## Task 2: Document Search Engine

This task uses Cosine Similarity to find the most relevant document for a given query.

### Query

machine learning algorithms for data

### Similarity Scores

Document 1: 0.7559
Document 2: 0.3536
Document 3: 0.0000
Document 4: 0.5669

### Most Relevant Document

Machine learning algorithms analyze structured data effectively.

### Task 2 Screenshot

<img width="471" height="130" alt="image" src="https://github.com/user-attachments/assets/dfd8c4ef-b141-4599-9907-3d68243e7650" />

---

# Lab Viva & Reflection Questions

## 1. Word Order Invariance

Bag of Words ignores the order of words and only counts how many times each word occurs. Therefore, "Dog bites man" and "Man bites dog" have the same Bag of Words representation because they contain the same words.

This can affect sentiment analysis because word order can change the meaning of a sentence. BoW may not understand the difference when the same words are arranged differently.

## 2. Sparsity Issue

When the corpus contains 100,000 unique vocabulary words, the Bag of Words matrix becomes very large and requires more memory. However, most documents contain only a small number of these words, so most entries in the matrix are 0. Therefore, the matrix becomes sparse.

## 3. Zero Similarity

Document 3 receives a Cosine Similarity score of 0.0000 because it does not contain overlapping terms with the query "machine learning algorithms for data". Therefore, their Bag of Words vectors have no common terms, resulting in zero similarity.

---

## Conclusion

This lab demonstrated how text can be converted into numerical vectors using the Bag of Words model and how Cosine Similarity can be used to measure the similarity between a search query and documents.

