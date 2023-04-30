# langchain-cohere-qdrant-retrieval
This is a template retrieval repo to create a Flask api server using LangChain that takes a PDF file and allows to search in 100+ languages with Cohere embeddings and Qdrant Vector Database.

## Installation

Install all the python dependencies using pip

```bash
pip install -r requirements.txt
```

# Qdrant setup

Please make an account on [Qdrant](https://qdrant.tech/) and create a new cluster. You will then be able to get the qdrant_url and qdrant_api_key used in the section below.

## Environment variables

Please assign environment variables as follows.
```
cohere_api_key="insert here"
openai_api_key="insert here"
qdrant_url="insert here"
qdrant_api_key="insert here"
```

## Run the app

Run the app using Gunicorn command

```bash
gunicorn app:app
```

The app should now be running with an api route ```/embed``` and another api route ```/retrieve```.

Feel free to reach out if any questions on [Twitter](https://twitter.com/MisbahSy)


