# nlp
This repository is for small projects in natural language processing and sentiment analysis

3. TF-IDF model (from GeeksforGeeks)
tf-idf stands for Term frequency-inverse document frequency. The tf-idf weight is a weight often used in information retrieval and text mining. Variations of the tf-idf weighting scheme are often used by search engines in scoring and ranking a document’s relevance given a query. This weight is a statistical measure used to evaluate how important a word is to a document in a collection or corpus. The importance increases proportionally to the number of times a word appears in the document but is offset by the frequency of the word in the corpus (data-set).

How to Compute:
tf-idf is a weighting scheme that assigns each term in a document a weight based on its term frequency (tf) and inverse document frequency (idf). The terms with higher weight scores are considered to be more important.

Typically, the tf-idf weight is composed by two terms-

Normalized Term Frequency (tf)
Inverse Document Frequency (idf)

Step 1: Computing the Term Frequency(tf)
Frequency indicates the number of occurences of a particular term t in document d. Therefore,

tf(t, d) = N(t, d), wherein tf(t, d) = term frequency for a term t in document d.

N(t, d)  = number of times a term t occurs in document d
We can see that as a term appears more in the document it becomes more important, which is logical.We can use a vector to represent the document in bag of words model, since the ordering of terms is not important. There is an entry for each unique term in the document with the value being its term frequency.

Given below are the terms and their frequency on each of the document. [N(t, d)]

tf for document 1:

DOC 1	BEN	STUDIES	COMPUTER	LAB
tf	1	1	2	1
Vector Space Representation for Doc 1 : [1, 1, 2, 1]

Vector Space Representation for Doc 2 : [1, 1, 1, 1]

tf for document 3:
 

DOC 3	DATA	SCIENTISTS	WORK	LARGE	DATASETS
tf	1	1	1	1	1
Vector Space Representation for Doc 3 : [1, 1, 1, 1, 1]

Thus, the representation of documents as vectors in a common vector space is known as Vector Space Model and it’s very fundamental to information retrieval.

Since we are dealing with the term frequency which rely on the occurrence counts, thus, longer documents will be favored more. To avoid this, normalize the term frequency
