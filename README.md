# 📊 LangSmith QA Dataset: DBRX Model Evaluation

## 🧾 Project Overview

In this project, we set up a complete workflow to evaluate a question-answering (QA) system using [LangSmith](https://smith.langchain.com), LangChain’s tracing and evaluation platform.

We began by installing essential Python libraries including:
- `langsmith` — to interact with the LangSmith API
- `openai` — for model integration if using OpenAI LLMs
- `ollama` — to support local LLM inference via the Ollama runtime
- `pandas` — for dataset creation, manipulation, and CSV handling

We then configured environment variables like `LANGCHAIN_API_KEY`, `LANGCHAIN_PROJECT`, and `LANGCHAIN_TRACING_V2` to authenticate and enable advanced tracing capabilities in LangSmith.

Next, we used `pandas` to construct a structured QA dataset centered on the DBRX model. The dataset included questions related to its architecture, pretraining data, GPU infrastructure, and context window size. This data was then saved as a CSV file for recordkeeping and uploading.

Using the LangSmith Python SDK, we initialized a `Client`, created a dataset named `"DBRX"`, and uploaded the question-answer pairs as examples. Additionally, we demonstrated how to incrementally add new QA entries to the same dataset, illustrating LangSmith’s support for iterative and evolving evaluation pipelines.

This setup enables robust model evaluation, debugging, and benchmarking using either LangSmith's visual interface or programmatic automation.

---
