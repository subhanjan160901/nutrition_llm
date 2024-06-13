# Nutrition QnA Chatbot
I have built a web application that allows users to ask anything about everyday nutrition, dietary guidelines, impact of various foods on our health system, etc. The data has been collected from the manual "DIETARY GUIDELINES FOR INDIANS" which is available on the official website of National Institute of Nutrition (https://www.nin.res.in). 

In this document, food-related approaches, both in qualitative and quantitative terms, have been incorporated. The guidelines are consistent with the goals set in national policies on Agriculture, Health and Nutrition. Emphasis is on positive recommendations which can maximize protective effects through use of a variety of foods in tune with traditional habits. This can help to formulate health promoting recipes and diets which are region- and culture- specific. 

Our application leverages OpenAI's GPT-3.5-turbo model for natural language processing and the Llamaindex framework for indexing and querying document contents.

## Features

The chatbot employs a Retrieval-Augmented Generation (RAG) pipeline, which involves the following steps:

1. **Document Loading**: Documents are loaded from a specified directory and processed.
2. **Indexing**: The contents of the documents are indexed. This step creates a searchable index that maps relevant sections of the documents to key terms and phrases.
3. **Retrieval**: When a user asks a question, the query is first used to retrieve relevant document sections from the index.
4. **Generation**: The retrieved document sections are then passed to the OpenAI GPT-3.5-turbo model, which generates a context-aware response based on the retrieved information.

## Architecture

The "llama_index" library is central to building this chatbot, providing the necessary tools for indexing and querying document contents. LlamaIndex is a framework that allows us to ingest custom content/data and allows us to query that content. The following picture shows a high level approach of how LlamaIndex works :
![image](https://github.com/subhanjan160901/nutrition_llm/assets/55011614/10bef7a6-7522-4c83-b9f3-de4d2a5d7541)
