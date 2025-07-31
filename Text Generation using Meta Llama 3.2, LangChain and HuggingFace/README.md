# Text Generation using Meta Llama 3.2, LangChain and HuggingFace

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)

![Libraries](https://img.shields.io/badge/Libraries-MetaLlama3.2%2C%20LangChain%2C%20Transformers-orange.svg)

## 📝 Overview

This project demonstrates a prompt-based Natural Language Processing (NLP) pipeline leveraging [LangChain](https://python.langchain.com/) and [HuggingFace Transformers](https://huggingface.co/). The system enables users to provide a topic and supporting sources, then generates an explanation using the Meta Llama-3.2 language model. This workflow showcases chaining language models and prompt templates for flexible, reference-driven text generation.

## ✨ Features

- **Custom Prompt Generation:** Allows users to input a *topic* and *source references* for context-aware text generation.
- **Meta Llama 3.2 Integration:** Uses the `meta-llama/Llama-3.2-1B` model from HuggingFace for high-quality, reference-guided text outputs.
- **Dynamic User Input:** Accepts varied topics and references, producing tailored explanations.
- **LangChain Pipeline:** Leverages LangChain for creating and managing the NLP pipeline, including a flexible `PromptTemplate` and model chaining.
- **GPU Acceleration:** Includes a CUDA check for leveraging GPU resources to speed up model inference.


## 🛠️ Installation

Install the required dependencies in your Python environment:

```bash
pip install langchain transformers langchain-huggingface
```

> The notebook is developed for Google Colab, though it can also be executed locally (GPU recommended for improved performance).

## 🚀 Usage

1. **Clone or download** this repository and open the notebook: `testing_langchain_using_meta_llama_3_2.ipynb`
2. **Run all cells** in order.
3. **Check GPU availability** (printed in notebook output).
4. **Download and initialize** the Meta Llama 3.2 model.
5. **Enter the topic and sources** when prompted.
6. **View generated explanation**—the model will output an explanation based on your inputs.

### Example

```
What topic would you like know: Machine Learning
Sources: wikipedia

Please explain Machine Learning topic to me. Use wikipedia as reference. And do not copy-paste from the wikipedia.
Machine Learning is a broad area of computer science that deals with the design and development of computational systems that can learn and improve their performance without being explicitly programmed to do so. ...
```


## 🧩 Model Used

This project utilizes the following pre-trained model from the HuggingFace Hub:
- **Text Generation:** [`meta-llama/Llama-3.2-1B`](https://huggingface.co/meta-llama/Llama-3.2-1B)


## 📦 Dependencies

- `Python 3.x`
- `transformers`
- `langchain`
- `langchain-huggingface`
- `torch` (for GPU support)

