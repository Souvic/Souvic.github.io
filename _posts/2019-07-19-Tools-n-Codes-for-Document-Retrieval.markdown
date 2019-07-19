---
layout: default
title:  "Tools and Codes for Document Retrieval"
date:   2019-07-19 17:15:00
categories: teaching
---
**Date: 19th July 2019** <br>
**Course: INFORMATION RETRIEVAL** 

Today's class included discussions on the following
* Recap of previous class (keyword matching method, inverted index, inverted positional index)
* Few more examples to understand all the three methods (discussed in class, not in slides)
* Keyword matching using "grep" UNIX command
* Inverted index method codes
* Inverted positional index using lucene
* Using "grep", lucene to search queries in small set of documents
* Running "grep", inverted index, and lucene bigger datasets
* Analysis of the Performance (Recall, and Time to search)

You can find the materials below.
* ["grep" manual](http://man7.org/linux/man-pages/man1/grep.1.html)<br>
Here a manual for "grep" command can be found which includes different options, patterns for different requirements. 
* [Dataset](https://drive.google.com/drive/folders/1pogGFFrn_WjIKn5uTKQ_mw4N4CIhalQF?usp=sharing)<br>
The dataset contains the following 
  1. "query.txt": List of <query_ids, queries>
  2. "alldocs.rar": Around 5800 text documents
  3. "output.txt": List of relevant document for each query or the true answers for each of the queries<br>
Task: For each query find the relevant documents out of all the 5800 documents.
* [Codes](https://github.com/gourabkumarpatro/RelevantDocumentSearch-GREP-vs-INDEX-vs-PYLUCENE-)<br>
This contains the following
  1. "grep_code.py": Finds the relevant documents using "grep" command
  2. "nltk_index_code.py": Creates a simple inverted index and then uses it to finds relevant docs for each query
  3. "pylucene_code.py": Creates a more sophisticated form of inverted positional index and then uses it to finds relevant docs for each query<br>
(Don't forget to extract all the files from the rar folder before running the codes. All these implementations prints the average recall and average time required for each query. All these codes can be executed on a system with atleast 2GB_RAM-n-DualCore ,and their performances can compared as done in class.)
  4. "Python_Lucene_Installation_Steps.txt" : Steps to install lucene


