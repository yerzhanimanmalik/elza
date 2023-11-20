# Elza
### Movie Recommender System - LLM chatbot with RAG
Instructions:
Run Elza.ipynb in Google Colab
Upload dataset data.csv (also called Hydra-Movie-Scrape.csv in Elza notebook) to content
Proceed with running all the cells using GPU 

In order to run notebook you will need to get API key from app.pinecone.io and environment from console
In Pinecone create a new Index to store all the vectors - movie summary embeddings
Embeddings are created using "all-MiniLM-L6-v2" model from Sentence-Transformers library

As LLM we tried two options: LLAMA2-13b-chat (4k) and Openchat (8k), also was thinking to use GPT3.5-Turbo 16k
GPT3.5-Turbo has a 16k context length as opposed to LLAMA2 which gives it a significant advantage, as we need to store history of messages
However, LLAMA2 is free and Open-Source whereas each call to GPT api have some costs 

Final version of Elza is made with Openchat from a library Ollama, note that Openchat is one of the best latest open-source models.
GPT4ALL library is used to create embeddings, however the model used for this purpose is still "all-MiniLM-L6-v2"
I also use Gradio to create a UI experience


