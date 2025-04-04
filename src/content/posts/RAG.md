---
title: RAG introduction
published: 2025-04-04
tags: [RAG, LLM]
category: LLM
draft: false
description: Fudamental knowledge about RAG
image: https://i.pximg.net/img-original/img/2022/09/04/18/40/36/100994095_p0.png
---

## What is and Role ?
A technology that use external knowledge repository to reduce hallucination of LLM.

## How does it works ?
1. Split the **Knowledge Base**(PDF、Word,Wiki,video,audio,PDF,etc... generally, un-structured data) into **Text Chunk** 
2. **Text Chunk** will be converted into **vector** (High dimension to Low dimension, capture the semantic relation) by **Embedding Model** (eg. OpenAI: text-embedding-3-large etc..) Note: different Embeddig Model will create differnt vector values. 
3. **Vector Base** is formed by these vector embeddings. It can be used as a Long-term Memory for AI.
4. Combine the **User Query**(will be converted into vector by embedding model too) and the **Vector Base**, doing the similarity search. (Retrieve part)
5. Select **top-k chunks**.
6. **Top-k chunks** will be sent into **Reranking model** to select **top-n chunks** among them. (improve search relevance)
7. **Top-n chunks** will be sent to LLM as context(combined with user query)

## How to measure if the vector embeddings are similar ?
- Euclidean Distance
- Cosine Similarity(usually used in text-based data,NLP. Because: Even if two document are stronly different in length,which will lead to long euclidean distance, they still have the possibility to have high cosine similarity)
- Dot Product Similarity






