# Agentic AI Learning

My notes and experiments while learning to build AI agents.

Everything here is written as a notebook I can run and re-read later, in plain English, with the reasoning kept next to the code.

## 01 Hugging Face Agents

Agents built with the Hugging Face `smolagents` library.

| Notebook | What it covers |
| --- | --- |
| `01_Music_Search_Agent` | A first agent using a built-in web search tool |
| `02_Custom_Menu_Tool_Agent` | Writing a custom tool with the `@tool` decorator |
| `03_Authorized_Imports_Agent` | Controlling which imports the agent is allowed to use |
| `04_Multi_Tool_Party_Agent` | Combining several tools and letting the agent choose |
| `05_Sharing_and_Importing_Tools` | Pushing tools to the Hub and loading tools from it |
| `06_Retrieval_Agent_With_Custom_Tools` | A retrieval agent over a small local knowledge base |

## Running the notebooks

The notebooks use `InferenceClientModel`, so the language model runs on the Hugging Face Inference API rather than locally.

```bash
pip install smolagents
```

A Hugging Face token is needed for the inference calls:

```bash
export HF_TOKEN="your_token_here"
```
