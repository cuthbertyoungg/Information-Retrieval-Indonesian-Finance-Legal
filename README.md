# Information-Retrieval-Indonesian-Finance-Legal
A simple Information Retrieval project using Natural Language Processing Techniques like BM25-Okapi, DenseE5 as Bi-Encoder and BGEReranker as Cross-Encoding Reranker

Workflow: Data Scraping ( over 3000 documents ) -> Text Extraction with PdfPlumber -> Pasal ( Article ) Splitting/Chunking with the help of regex -> WER & CER Evaluation ->  Singlehop & Multihop Ground Truth Construction -> Preprocess ( cleaning & normalization ) -> BM25 encoding -> Extract Dense E5 embeddings -> Cosine Similarity -> Top K -> Feed query and candidate passages into BGEReranker ( Cross Encoding ) -> Select TOP K -> Evaluation with Recall, Mrr, Bleu -> Errror Analysis
