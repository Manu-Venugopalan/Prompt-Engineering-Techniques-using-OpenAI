# 🧠 Prompt Engineering for AI Tasks
![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)
![Model](https://img.shields.io/badge/Model-FinBERT-yellow.svg)
![Model](https://img.shields.io/badge/Model-OpenAI-yellow.svg)
![Tech](https://img.shields.io/badge/Technique-ZeroShot%20|%20FewShot%20|%20CoT-orange.svg)
![Issues](https://img.shields.io/github/issues/your-username/your-repo.svg)
![Stars](https://img.shields.io/github/stars/your-username/your-repo.svg)

Prompt engineering is a core technique in working with modern large language models (LLMs) like GPT, LLaMA, Claude, and FinBERT. It involves crafting the right instructions (prompts) to guide the model toward generating the most accurate and contextually appropriate responses for a given task.

---

### 📘 Prompt Engineering Techniques (With Examples)

| Technique                       | Description                                                                                                                                         | Example                                                                                                                                                                                                         |
| ------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Zero-shot prompting**         | Asking the model to complete a task with no prior examples or context. Useful when the model is already well-trained on a broad range of knowledge. | **Prompt:**<br>“Classify the following sentence as positive, neutral, or negative: ‘The market closed higher today.’”<br>**Expected Output:**<br>Positive                                                       |
| **Few-shot prompting**          | Providing a few annotated examples before asking the model to perform a similar task. Enhances performance when training data is scarce.            | **Prompt:**<br>“Classify the sentiment:<br>1. ‘The stock fell sharply.’ → Negative<br>2. ‘Company revenue grew.’ → Positive<br>3. ‘Dividend remained unchanged.’ →”<br>**Expected Output:** Neutral             |
| **Chain-of-thought prompting**  | Encouraging the model to think step-by-step before providing the final answer. Useful for tasks requiring logical reasoning or calculations.        | **Prompt:**<br>“Is 738 divisible by 3? First, sum the digits: 7+3+8=18. Is 18 divisible by 3?”<br>**Expected Output:** Yes, 738 is divisible by 3.                                                              |
| **Instruction-based prompting** | Giving explicit instructions in natural language. Best for information extraction, summarization, or formatting tasks.                              | **Prompt:**<br>“Extract all financial entities and amounts from the text.”<br>“Barclays invested £50 million in renewable energy.”<br>**Expected Output:**<br>{ "Entity": "Barclays", "Amount": "£50 million" } |
| **Role prompting**              | Assigning a specific role or persona to the model to influence the style or domain knowledge of the response.                                       | **Prompt:**<br>“You are a financial advisor. Recommend an investment plan for a risk-averse client in retirement.”<br>**Expected Output:**<br>A balanced fund or low-risk bond portfolio.                       |
| **Output formatting**           | Asking the model to respond in a particular format (JSON, list, table, etc.) to aid downstream processing.                                          | **Prompt:**<br>“Summarize the key investment risks. Respond in bullet points.”<br>**Expected Output:**<br>- Market volatility<br>- Inflation<br>- Liquidity risk                                                |
| **Prompt tuning (advanced)**    | Optimizing soft prompt tokens using a training dataset. Used in enterprise-level applications to fine-tune model behavior.                          | **Tools Used:** PEFT, LoRA, or SoftPrompting libraries.                                                                                                                                                         |

---

### ✅ Real-World Applications in This Project

This repository demonstrates how prompt engineering is applied to tasks in the financial services domain, using models like FinBERT and GPT:

* **Text Classification (Zero/Few-shot):** Classify financial statements into labels like `ObjectivesAndNeeds`, `Assets`, `Outgoings`, etc.
* **Information Extraction (Instruction-based):** Extract data points like investment amount, institution name, and client goals from conversations.
* **Summarization (Role-based):** Generate personalized meeting summaries from advisor-client interactions.
* **Risk Profiling (Chain-of-thought):** Guide the model to assess financial risk tolerance using reasoning prompts.

---

### 🚀 Technologies Used

* **LLMs:** GPT-4, FinBERT
* **Prompting Frameworks:** LangChain, OpenAI API
* **Data:** Annotated Atlas files and unannotated Arla transcripts from financial conversations
* **Environment:** Python 3.8+, Transformers, Hugging Face Datasets


### 📈 Future Work

* Integrate prompt-based evaluation for performance benchmarking
* Incorporate RAG (Retrieval-Augmented Generation) with prompt verification
* Extend support for multilingual financial datasets

---


