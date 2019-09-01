# Spam-Classifier-using-Naive-Bayes

1. The SMS Spam Collection is a set of SMS tagged messages that have been collected for SMS Spam research. 
2. It contains one set of SMS messages in English of 5,574 messages, tagged according being ham (legitimate) or spam.
3. The files contain one message per line. Each line is composed by two columns: v1 contains the label (ham or spam) and v2 contains the      raw text.

#Addition of Additional Feature TF–IDF

1. Tf–idf stands for "Term Frequency–Inverse Document Frequency" is a numerical statistic used to reflect how important a word is to a        document in a collection or corpus of documents.
2. TFIDF is used as a weighting factor during text search processes and text mining.
3. The intuition behing the TFIDF is as follows: if a word appears several times in a given document, this word might be meaningful (more    important) than other words that appeared fewer times in the same document. However, if a given word appeared several times in a given    document but also appeared many times in other documents, there is a probability that this word might be common frequent word such as      'I' 'am'..etc. (not really important or meaningful!).
4. TF: Term Frequency is used to measure the frequency of term occurrence in a document:
5. TF(word) = Number of times the 'word' appears in a document / Total number of terms in the document
6. IDF: Inverse Document Frequency is used to measure how important a term is:
7. IDF(word) = log_e(Total number of documents / Number of documents with the term 'word' in it).
8. Example: Let's assume we have a document that contains 1000 words and the term “John” appeared 20 times, the Term-Frequency for the        word 'John' can be calculated as follows:
   TF|john = 20/1000 = 0.02
9. Let's calculate the IDF (inverse document frequency) of the word 'john' assuming that it appears 50,000 times in a 1,000,000 million      documents (corpus).
   IDF|john = log (1,000,000/50,000) = 1.3
   Therefore the overall weight of the word 'john' is as follows
   TF-IDF|john = 0.02 * 1.3 = 0.026
