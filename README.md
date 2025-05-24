# LangChain-Agents-with-Tools
This project showcases LangChain agents dynamically selecting and utilizing various tools (Wikipedia, ArXiv, custom RAG) powered by different LLMs (OpenAI, Ollama Mistral) to answer diverse queries.


## Features

* **Tool Integration**: Utilizes Wikipedia, ArXiv, and a custom retriever tool for diverse information access.
* **Flexible LLMs**: Works with OpenAI's `gpt-3.5-turbo-0125` and local models like `Mistral` via Ollama.
* **Agentic Behavior**: Agents intelligently select and use the most appropriate tool for a given query.

## Setup

1.  **Install dependencies:**
    ```bash
    pip install -U langchain langchain-community langchain-core langchain-huggingface sentence_transformers faiss-cpu arxiv wikipedia pydantic>=2.0,<3.0 python-dotenv llama-cpp-python langchain-ollama
    ```

2.  **Set your OpenAI API Key:**
    Create a `.env` file in the project root and add:
    ```
    OPENAI_API_KEY="YOUR_OPENAI_API_KEY"
    ```
    If using LangSmith, also set `LANGCHAIN_API_KEY`.

3.  **For Ollama (optional):**
    Download and install Ollama from [ollama.com](https://ollama.com/).
    Pull the Mistral model: `ollama pull mistral`

## Usage

1.  Open the `Agents.ipynb` Jupyter Notebook.
2.  Run through the cells to see how tools are defined, combined into an agent, and then used to answer questions by leveraging the appropriate tool.

   ![image](https://github.com/user-attachments/assets/2246eddc-8ee5-414f-a298-9643cef4beff)

   ![image](https://github.com/user-attachments/assets/d184ff22-310d-4bce-b4ad-ee3b7cdc862c)


