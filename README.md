# LangChain Exploration Notebooks

This repository contains a collection of Jupyter notebooks for experimenting with the [LangChain](https://www.langchain.com/) framework. It covers various features, from basic model interaction and prompt templating to more advanced topics like agents and tools, using both OpenAI and Google Gemini models.

## Notebooks Overview

*   **[main.ipynb](main.ipynb)**: The primary notebook for exploring core LangChain concepts using OpenAI. It covers:
    *   Basic `ChatOpenAI` instantiation and invocation.
    *   Prompt Templates.
    *   Response Caching (In-memory).
    *   Streaming responses.
    *   Chaining runnables.

*   **[main-gemini.ipynb](main-gemini.ipynb)**: Focuses on integrating and using Google's Gemini models through the `langchain-google-genai` package.

*   **[langchain-tools.ipynb](langchain-tools.ipynb)**: Demonstrates how to use pre-built LangChain tools like `DuckDuckGoSearchResults` and `WikipediaQueryRun` to give language models access to external information.

*   **[react.ipynb](react.ipynb)**: Explores the implementation of a ReAct (Reasoning and Acting) agent, which can use tools to answer questions that require external knowledge.

*   **[embeddings.ipynb](embeddings.ipynb)**: Covers the creation and use of text embeddings for semantic search. It demonstrates how to:
    *   Generate embeddings for a list of words from [words.csv](words.csv).
    *   Save the embeddings to [words-embeddings.csv](words-embeddings.csv).
    *   Perform similarity searches to find semantically related terms.

## Setup and Installation

1.  **Clone the repository:**
    ```bash
    git clone <your-repository-url>
    cd <repository-directory>
    ```

2.  **Create and activate a virtual environment:**
    ```bash
    python -m venv venv
    source venv/bin/activate 
    ```

3.  **Install dependencies:**
    The project dependencies are listed in [requirements.txt](requirements.txt).
    ```bash
    pip install -r requirements.txt
    ```

4.  **Set up environment variables:**
    Create a `.env` file in the root directory. Add your API keys to this file.
    ```env
    # .env
    OPENAI_API_KEY="your-openai-api-key"
    GOOGLE_API_KEY="your-google-api-key"
    ```
    The `.env` file is included in the [.gitignore](.gitignore) to prevent accidental sharing of your keys.

## Usage

Once the setup is complete, you can run the Jupyter notebooks to explore the different LangChain features. Launch Jupyter Lab or Jupyter Notebook from your activated virtual environment:

```bash
jupyter lab
```

Then, navigate to the notebook file you wish to view.