# DESCRIPTION OF THE PROJECT

YouTube’s recommendation system often prioritizes engagement over viewpoint diversity, which can limit exposure to alternative perspectives. 
Many users seek a broader range of opinions on a topic, but the platform does not consistently support this.

This project addresses the issue by implementing an API-grounded LLM pipeline using n8n to surface YouTube videos that present diverse perspectives for a given search query.

The pipeline first extracts video titles, URLs, and descriptions (when available) using the YouTube Data API.
This metadata is then analyzed by a LLaMA 3 model, running locally via the Ollama API, to identify videos based on perspective diversity rather than popularity.

Multiple open-source language models were evaluated during development. 
Among them, LLaMA 3 demonstrated the most consistent performance in accurately identifying diverse viewpoints and was therefore selected for the final pipeline.
