# DESCRIPTION OF THE PROJECT

ViewPoints addresses the lack of viewpoint diversity in YouTube’s recommendation system, which often prioritizes engagement over exposure to alternative perspectives. 
As a result, users seeking a broader range of opinions on a topic are not consistently supported by the platform.

This project implements an API-grounded LLM pipeline using n8n to surface YouTube videos that present diverse perspectives for a given search query. 
The pipeline extracts video titles, URLs, and descriptions (when available) via the YouTube Data API, and processes this metadata using a LLaMA 3 model running locally through the Ollama API.

Multiple open-source language models were evaluated during development. 
Among them, LLaMA 3 demonstrated the most consistent performance in identifying diverse viewpoints and was therefore selected for the final implementation.
