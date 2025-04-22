# Gen-AI-Intensive-Course-Capstone-2025Q1
## Monopoly rules assistant using RAG
### Project Overview
In this example, we’ll build a Board Game Rules Assistant that lets users ask questions about the rules of a board game (for example, from a PDF rulebook).
**Goal**: Create an interactive Jupyter Notebook that can read a board game rule document (e.g., in PDF form), index its contents with embeddings, and answer user queries in a structured JSON format using few-shot prompting in a RAG framework.

Generative AI capabilities demonstrated:

**Retrieval Augmented Generation (RAG)**: The notebook ingests the document, splits it into chunks, computes embeddings, and stores these in a vector index . When a user asks a question, the notebook retrieves the most relevant text passages for context.

**Few-shot Prompting**: The prompt fed into the language model includes a couple of examples (a few-shot setup), instructing the system on how to answer questions based solely on the retrieved context. We guide the large language model with a few example question–answer pairs, which helps steer the generation in a specific style.

**Structured Output/JSON Mode**: The language model is explicitly instructed to output its answer in JSON format (e.g., with keys "answer", and "sources"), ensuring that its responses are controlled and easy to postprocess.
