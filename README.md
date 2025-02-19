# Introduction
This project is a collection of LangChain-based implementations designed to demonstrate various functionalities of working with large language models (LLMs). It includes prompt parsing, memory handling, chaining multiple LLM calls, building Q&A systems, evaluating model responses, and using agents for automated tasks.

This project is based on the LangChain course by [DeepLearning.AI](https://learn.deeplearning.ai/courses/langchain/lesson/u9olq/introduction) and expands upon core concepts by demonstrating hands-on examples with different LangChain modules.

## Features
*	Prompt Parsing: Understanding and structuring prompts effectively.
*	Memory Management: Using different types of memory to retain conversation context.
*	Chaining Models: Implementing sequential chains to enhance complex workflows.
*	Question Answering: Using document retrieval to answer user queries.
*	Evaluation: Assessing model outputs through manual and automated evaluations.
*	Agents: Creating dynamic, tool-using AI agents.

## Project Structure
The project is divided into six Jupyter Notebooks, each covering a distinct LangChain concept:
```bash
📂 LangChain-for-LLM-Application-Development
│-- 📂 Codes
    │── 📜 1. Model Prompt Parser.ipynb         # Parsing prompts effectively
    │── 📜 2. Memory.ipynb                      # Memory types for conversations
    │── 📜 3. Chains.ipynb                      # Sequential processing with chains
    │── 📜 4. QnA.ipynb                         # Retrieval-based question answering
    │── 📜 5. Evaluation.ipynb                  # Model evaluation techniques
    │── 📜 6. Agents.ipynb                      # Creating AI agents
│-- 📂 Config
    │── 📜 config.json                          # Contains the OpenAI API key
│── 📜 requirements.txt                         # Required dependencies
│── 📜 README.md                                # Project documentation
│-- 📜 Gitignore                                # Files to be ignored by Git
│-- 📜 LICENSE                                  # Project license
```

## Installation
You need to have the following softwares installed on your machine:
  * [Python](https://www.python.org/downloads/)
  * [Anaconda Navigator](https://www.anaconda.com/products/distribution)
  * [Juypyter notebook](https://jupyter.org/install)

## Setup
1. Clone the repository:
```bash
git clone https://github.com/Akashdip-N/LangChain-for-LLM-Application-Development.git
```

2. Create a virtual environment:
```bash
conda create --name myenv python=3.9.19
conda activate myenv
```
  
  3. Install the required packages:
```bash
pip install -r requirements.txt
```

4. Create a ```config.json``` file in the ```Config``` directory and add your OpenAI API key:
```json
{
    "api_key": "YOUR_OPENAI_API_KEY"
}
```

## OpenAI API Key
Steps to obtain an OpenAI API key:
  1. Go to [OpenAI API keys](https://platform.openai.com/account/api-keys) and sign up for an account.
  2. Generate an API key by clicking on the "API Keys" tab.
  3. Select the "Create new secret key" button and provide a name for the key.
  4. Click on the "Create new secret key" button to finally create the key.
  3. Copy the API key and save it in the `config.json` file in the `Config` directory.

## Note
  * The OpenAI API key is sensitive information and should not be shared publicly. Ensure that the `config.json` file is added to the `.gitignore` file to prevent accidental sharing of the API key.
  * Since you will be requiring an OpenAI API key, it will cost you money to run the code. Ensure that you have the necessary funds in your account to avoid any interruptions.

## Usage
Steps to run the project:
  * Open the `anaconda Navigator`.
  * Activate the virtual environment created earlier.
  * Launch the `Jupyter notebook`.
  * Navigate to the project directory and open the desired notebook.
  * Run the cells in the notebook to execute the code.


## Notebooks Overview

📜 1. Model Prompt Parser.ipynb
*	Parses and structures prompts for better model interactions.
*	Uses LangChain’s PromptTemplate for prompt engineering.

📜 2. Memory.ipynb
*	Implements conversation memory using different memory types:
*	ConversationBufferMemory
*	ConversationBufferWindowMemory
*	ConversationTokenBufferMemory
*	ConversationSummaryMemory

📜 3. Chains.ipynb
*	Uses LLMChain to process inputs in a structured way.
*	Implements SimpleSequentialChain and SequentialChain to automate workflows.
*	Demonstrates a Router Chain for multi-purpose prompts.

📜 4. QnA.ipynb
*	Builds a retrieval-based Q&A system using LangChain.
*	Loads documents into a vector store and queries them dynamically.
*	Utilizes RetrievalQA to enhance question answering.

📜 5. Evaluation.ipynb
*	Evaluates model responses manually and using LangChain’s QAEvalChain.
*	Generates example test cases and assesses model accuracy.

📜 6. Agents.ipynb
*	Implements LangChain Agents to dynamically select tools.
*	Uses built-in tools (Wikipedia, LLM-Math).
*	Creates a custom Python agent for executing code.

## Contributions
Contributions are welcome! For feature requests, bug reports, or questions, please raise an issue on the repository.

# License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

# Acknowledgements
*	[LangChain](https://github.com/langchain-ai/langchain) for providing the framework.
*	[DeepLearning.AI](https://learn.deeplearning.ai/) for the educational material.
*	[OpenAI](https://openai.com/) for powering the underlying language model.