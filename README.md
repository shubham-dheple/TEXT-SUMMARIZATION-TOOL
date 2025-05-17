# TEXT-SUMMARIZATION-TOOL

*Company*:CODETECH IT SOLUTION

*NAME*:Shubham Dheple

*Intern ID *:C0DF277

*DOMAIN*:AIML

*DURATION*:4 weeks

*Mentor*:NEELA SANTOSH

The provided Python code demonstrates how to summarize a block of text using the Latent Semantic Analysis (LSA) technique from the sumy library. This script takes a longer input passage and extracts the most relevant sentences to generate a concise summary. Here’s a detailed breakdown of the code and its functionality:

1. Purpose of the Code
The primary objective of this script is to reduce a lengthy paragraph into a smaller number of representative sentences that convey the core message. It does this using natural language processing (NLP) techniques available in the sumy library, specifically the LsaSummarizer, which uses Latent Semantic Analysis to determine the most important sentences in a given text.

2. Required Libraries
sumy.parsers.plaintext.PlaintextParser: This module is used to convert raw input text into a format that the summarization algorithm can understand.

sumy.nlp.tokenizers.Tokenizer: This is used to split the input text into sentences and words.

sumy.summarizers.lsa.LsaSummarizer: Implements the LSA technique to perform the actual summarization.

These modules together allow for tokenization, parsing, and summarizing of textual content.

3. Function Definition: summarize_text()
The core logic resides in a function called summarize_text() which takes two parameters:

text: The input paragraph that needs to be summarized.

sentence_count: The number of sentences you want in the summary (default is 3).

Steps Inside the Function:
The PlaintextParser.from_string() method is used to parse the raw input text. This converts the string into a document object which can be processed.

A Tokenizer is applied to break down the text into meaningful linguistic units (e.g., words and sentences).

An instance of LsaSummarizer is created.

The summarizer is applied to the parsed document, generating a list of the top-ranked sentences based on semantic similarity.

These sentences are then converted to strings and joined together to form the final summary output.

4. Example Input
The input_text variable contains a short article about Artificial Intelligence (AI), its uses, and associated ethical concerns. The text discusses the growing role of AI in various industries and the importance of responsible development.

5. Execution and Output
Finally, the function is called with the sample input text, and the number of summary sentences is set to 2. The result is printed to the console using print(). This produces a condensed version of the input, extracting the two most relevant sentences that best represent the original content.

6. Summary and Applications
This script is an excellent example of how you can perform automatic summarization of texts using Python. It is particularly useful for:

Condensing lengthy documents into shorter forms for quicker reading.

Extracting key information from news articles, reports, or research papers.

Creating preview summaries for content in applications like news aggregators, educational tools, and more.

The summarization approach using LSA is unsupervised and does not require training data, making it ideal for quick and domain-independent applications. However, it’s worth noting that it may not capture nuanced meanings or emotional tones as well as more advanced transformer-based models like BERT or GPT.
