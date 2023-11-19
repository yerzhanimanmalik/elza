# Elza
### Movie Recommender System - LLM chatbot with RAG
Instructions:
Run Elza.ipynb in Google Colab
Upload dataset Hydra-Movie-Scrape.csv to content
Proceed with running all the cells using GPU (preferably A100)

In order to run notebook you will need to get API key from app.pinecone.io and environment from console
In Pinecone create a new Index to store all the vectors - movie summary embeddings
Embeddings are created using "all-MiniLM-L6-v2" model from Sentence-Transformers library

As LLM we tried two options: LLAMA2-13b-chat and GPT3.5-Turbo 16k
GPT3.5-Turbo has a 16k context length as opposed to LLAMA2 which gives it a significant advantage
However, LLAMA2 is free and Open-Source whereas each call to GPT api have some costs 


