# Simple Agents using OpenAI(API) + LangGraph

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)

![Libraries](https://img.shields.io/badge/Libraries-OpenAI%2C%20LangGraph%2C%20LangChain-orange.svg)

## 📝 Overview

This project demonstrates how to build **simple interactive AI agents** using [LangChain](https://python.langchain.com/), [LangGraph](https://github.com/langchain-ai/langgraph), and [OpenAI](https://platform.openai.com/). The agents are created using LangGraph's pre-built ReAct (Reasoning and Acting) framework, which allows it to intelligently choose between using a language model for conversation or calling predefined tools for specific tasks.

The assistant is equipped with two basic tools: a greeting tool and a calculator, and can dynamically switch between them based on user input.

## ✨ Features

* **ReAct Agent Framework:** Utilizes `langgraph.prebuilt.create_react_agent` to create a robust agent that can reason about which tool to use.
* **Custom Tool Integration:** Defines and integrates two custom tools:
    * `greeting(name)`: To provide a personalized greeting.
    * `calculator(a, b)`: To perform simple arithmetic addition.
* **Interactive Chat Loop:** Provides a command-line interface for users to interact with the assistant continuously.
* **OpenAI Integration:** Uses `langchain_openai.ChatOpenAI` as the core language model to drive the conversation and reasoning.
* **Environment-Friendly:** Securely loads API keys using `dotenv`.


## 🛠️ Installation

To set up the project, install the required Python packages using pip:

```bash
pip install langchain-core langchain-openai langgraph python-dotenv
```

> **Note:** This project requires an OpenAI API key.

## 🚀 Usage

1. **Set up your environment:** Create a `.env` file in the root directory and add your OpenAI API key:

```
OPENAI_API_KEY="your-api-key-here"
```

2. **Open the notebook:** `simple_agents_using_langgraph.ipynb`.
3. **Run all cells** in sequential order.
4. **Interact with the assistant** in the input prompt. You can either chat or ask it to perform a calculation.
5. Type `quit` to exit the application.

### Example

```
Welcome! I'm your AI assistant. Type 'quit' to exit
You can ask me to perform calculations or chat with me

You: hi there, my name is Alex

Assistant: greeting tool has been called
Hello Alex, Hope you are doing well

You: what is 12 + 5

Assistant: calculator tool has been called
The sum of 12.0 and 5.0 is 17.0
```


## 🧩 Models \& Tools Used

* **LLM:** `langchain_openai.ChatOpenAI` (OpenAI's chat models)
* **Tools:**
    * `greeting`: A custom tool for personalized greetings.
    * `calculator`: A custom tool for arithmetic calculations.
* **Agent Framework:** `langgraph.prebuilt.create_react_agent`


## 📦 Dependencies

* `Python 3.x`
* `langchain`
* `langchain_openai`
* `langgraph`
* `python-dotenv`