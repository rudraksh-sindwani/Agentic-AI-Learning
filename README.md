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
| `07_Calculator_And_Converter_Agent` | An agent with a calculator tool and a unit converter tool |
| `08_Text_Stats_And_Formatter_Agent` | An agent with a text stats tool and a text formatter tool |
| `09_Date_And_Time_Helper_Agent` | An agent with a date difference tool and a date formatter tool |
| `10_Prompt_Injection_Detector_Agent` | An agent with a rule-based scanner tool and a redaction tool, plus why keyword matching alone is not a real defense |
| `11_Memory_Tool_Agent` | An agent that stores a fact in one `run()` call and recalls it in a separate one, via a shared memory store |

## 02 AI Ethics Case Studies

Short case studies working through real-world incidents, using small synthetic simulations to make the mechanism concrete.

| Notebook | What it covers |
| --- | --- |
| `01_Tokyo_Medical_University_Scandal` | A group-level score deduction, and how a cutoff learned from its outcomes carries the same bias into fresh, fair data |
| `02_COMPAS_Recidivism_Score_Controversy` | Why a score can be honestly calibrated and still have unequal error rates across groups, and why fixing one breaks the other |
| `03_Amazon_Scrapped_Hiring_Tool` | How a neutral-looking resume feature becomes a proxy for group membership, and why dropping one proxy doesn't guarantee there isn't another |
| `04_Facial_Recognition_Misidentification` | Why an underrepresented group can get a genuinely worse feature representation, and why a per-group threshold can't fix that the way it fixed earlier notebooks |

## Running the notebooks

The notebooks use `InferenceClientModel`, so the language model runs on the Hugging Face Inference API rather than locally.

```bash
pip install smolagents
```

A Hugging Face token is needed for the inference calls:

```bash
export HF_TOKEN="your_token_here"
```
