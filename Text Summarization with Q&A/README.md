# Text Summarization \& Q/A using LangChain and HuggingFace

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)

![Libraries](https://img.shields.io/badge/Libraries-LangChain%2C%20Transformers-orange.svg)


## 📝 Overview

This project demonstrates a multi-stage Natural Language Processing (NLP) pipeline built with [LangChain](https://python.langchain.com/) and [HuggingFace Transformers](https://huggingface.co/). The system takes a block of text from the user, generates a summary, and then allows the user to ask questions about the original text. This showcases how to chain multiple language models together to perform complex tasks like summarization, refinement, and question-answering.

## ✨ Features

*   **Multi-Model Summarization:** Chains two models (`facebook/bart-large-cnn` for initial summarization and `google/pegasus-xsum` for refinement) to produce a concise summary.
*   **Interactive Q&A:** Implements a question-answering system using the `deepset/roberta-base-squad2` model, allowing users to query the source text.
*   **Dynamic User Input:** Accepts any text block and desired summary length (`short`, `medium`, or `long`) from the user at runtime.
*   **LangChain Integration:** Uses LangChain to create and manage the NLP pipeline, including prompt templating and model chaining.
*   **GPU Acceleration:** Includes a check for CUDA availability to leverage GPU for faster model inference.


## 🛠️ Installation

Install the required dependencies in your Python environment:

```bash
pip install transformers langchain langchain_huggingface
```

> The notebook was developed in Google Colab, but can be run locally if you have a GPU (recommended for faster processing).

## 🚀 Usage

1. **Clone or download** this repository and open the notebook: `summaization-q-a_using_langchain.ipynb`
2. **Run all cells** in order.
3. **Enter the text to summarize** when prompted.
4. **Select summary length**: short, medium, or long.
5. **View the generated summary**.
6. **Engage in an interactive Q/A session**—ask questions based on the provided content or type `exit` to finish.

### Example

```
Enter the text to summarize:
Artificial intelligence (AI) is the capability of computational systems...
Enter the length (short/medium/long):
short

Generated Summary:-
Artificial intelligence (AI) is the capability of computational systems to perform tasks typically associated with human intelligence.

Ask a question (or type 'exit' to stop):
what is artificial intelligence

ANSWER: the capability of computational systems to perform tasks typically associated with human intelligence
```


## 🧩 Models Used

- **Summarization:** [`facebook/bart-large-cnn`](https://huggingface.co/facebook/bart-large-cnn)
- **Refinement:** [`google/pegasus-xsum`](https://huggingface.co/google/pegasus-xsum)
- **Q\&A:** [`deepset/roberta-base-squad2`](https://huggingface.co/deepset/roberta-base-squad2)


## 📦 Dependencies

- Python 3.x
- transformers
- langchain
- langchain_huggingface
- torch (for GPU support)

