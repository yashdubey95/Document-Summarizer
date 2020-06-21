# Document-Summarizer

This repository contains the python implementation for an extraction based document summarizer. 

## Introduction:
Document or Text Summarization is a technique that refers to minimizing the contents in the said document with the intention of producing a fluent and logical summary preserving the key informational elements.

In today's era of technological innovation, an explosive amount of data from various sources is circulating the digital space which needs to be summarized efficiently in order to reduce the space it occupies and increase the throughput of data useful for research while maintaining the original meaning of the document. Now, we as humans are extremely efficient in summarizing a piece of information by developing an understanding for the entire content and then writing a summary highlighting its main points; since manual text summarization is a generally laborious and time consuming task, thus automating this task although a difficult and a non-trivial challenge as machines lack the human knowledge and language capability has proven to show promising results with the advances in Natural Language Processing and Machine Learning. There are various approaches used for the automation of text summarization and they are broadly categorized as extraction based approach and abstraction based approach.

### Extraction Based Approach:

The extraction based document summarization approach generally uses a scoring function to identify important sections in the document cropping them and stitching them together with other portions of the content in order to form a coherent summary. This approach is easier and yields summaries that are naturally grammatical and require little or no linguistic analysis. 
Following is the general flow of an extraction based approach:-
  1. Using some metrics like a TF-IDF score for each sentence in the document, construct a representation of the document to highlight its salient features.
  2. Parse the generated representation through a score function to calculate the probability for each sentence to determine whether it will be picked up in the summary or not.
  3. Finally producing a summary based on some threshold like top-k or Latent Semantic Analysis (LSA) to identify important sentences. 
  
### Abstraction Based Approach:

The abstraction based approach is a releatively new approach as compared to extraction based appraoch, as it uses advanced natural language processing and complex machine learning algorithms to produce summary by interpreting the content in the document and generate a newer shorter version of the text parts of which may not even appear in the original document by and yet containing the gist of the content by paraphrasing sentences and semantically mapping it to produce a summaries as opposed to simply selecting and rearranging sentences from the original document. This approach is more closer to how us humans summarize information than the data-driven approach used in extraction based document summarizer; and is thus a challenging task to implement effectively.

## Prerequisites:

Programming Language and Libraries Used:
  1. Python ==> 3.7.6
  2. nltk ==> 3.4.5
  3. bs4 ==> 4.8.2
  4. urllib3 ==> 1.25.8
  
 ## Usage:
 ```bash
 python documentSummarizer.py
 ```
 
 ## Output
 ![alt text](https://github.com/yashdubey95/Document-Summarizer/blob/master/Document%20Summarization/Output.PNG)
