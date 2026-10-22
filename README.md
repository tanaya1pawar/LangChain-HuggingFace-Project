# LangChain-HuggingFace-Project
A local NLP and vector search pipeline built using LangChain, Hugging Face Transformers (gpt2), Sentence-Transformers embeddings (all-mpnet-base-v2), and FAISS vector database in Google Colab.
# 🚀 Local LLM & Vector Search Pipeline (LangChain & Hugging Face)

An end-to-end local machine learning project implemented in Google Colab[cite: 10] that demonstrates local text generation, recursive text chunking, dense vector embeddings, and similarity search indexing using **FAISS** and **LangChain**.

---

## 🛠️ Tech Stack & Components

* **Framework:** LangChain (`langchain-core`, `langchain-huggingface`, `langchain-community`)[cite: 10]
* **Local LLM:** Hugging Face Transformers Pipeline using `gpt2` (Causal Language Model)[cite: 10]
* **Embeddings Model:** `sentence-transformers/all-mpnet-base-v2` (768-dimensional vector embeddings)[cite: 10]
* **Vector Store:** Facebook AI Similarity Search (**FAISS**)[cite: 10]
* **Environment:** Google Colab (Python 3.13)[cite: 10]

---

## 📌 Core Features Implemented in the Notebook

1. **Local Text Generation:** Initialized Hugging Face causal language models (`gpt2`) and wrapped them inside LangChain's pipeline integration for prompt chaining[cite: 10].
2. **Text Splitting:** Configured `RecursiveCharacterTextSplitter` with customized chunk sizes and overlaps for processing large text data[cite: 10].
3. **Dense Embeddings:** Generated 768-dimensional vector embeddings using pre-trained sentence transformer models (`all-mpnet-base-v2`)[cite: 10].
4. **FAISS Vector Indexing & Local Persistence:** Indexed document embeddings locally using FAISS, performed similarity searches with distance scores, and saved/reloaded index files (`faiss_index`)[cite: 10].

---

## 💻 Sample Code Workflow
* **Text Generation Chain Example:**
  ```python
  from langchain_core.prompts import PromptTemplate

  template = "Question: {question}\nAnswer: Let's think step by step."
  prompt = PromptTemplate(template=template, input_variables=["question"])
  chain = prompt | local_llm
  response = chain.invoke({"question": "What is machine learning?"})
  print(response)


  FAISS Similarity Search Example:
  query = "What is FAISS used for?"
results = db.similarity_search(query, k=1)
print(results[0].page_content)


Here are tailored descriptions, a complete `README.md` template, and a quick explanation in a Marathi-English mix for your **`Langchain_and_Huggingface1.ipynb`** project notebook!

---

### 📝 Short GitHub Bio / Repository Description

*Paste this into the **About** section of your GitHub repository:*

> A local NLP and vector search pipeline built using LangChain, Hugging Face Transformers (`gpt2`), Sentence-Transformers embeddings (`all-mpnet-base-v2`), and FAISS vector database in Google Colab.

---

### 📄 Complete `README.md` Template

*Create a file named `README.md` in your GitHub repository and paste this:*

```markdown
# 🚀 Local LLM & Vector Search Pipeline (LangChain & Hugging Face)

An end-to-end local machine learning project implemented in Google Colab[cite: 10] that demonstrates local text generation, recursive text chunking, dense vector embeddings, and similarity search indexing using **FAISS** and **LangChain**.

---

## 🛠️ Tech Stack & Components

* **Framework:** LangChain (`langchain-core`, `langchain-huggingface`, `langchain-community`)[cite: 10]
* **Local LLM:** Hugging Face Transformers Pipeline using `gpt2` (Causal Language Model)[cite: 10]
* **Embeddings Model:** `sentence-transformers/all-mpnet-base-v2` (768-dimensional vector embeddings)[cite: 10]
* **Vector Store:** Facebook AI Similarity Search (**FAISS**)[cite: 10]
* **Environment:** Google Colab (Python 3.13)[cite: 10]

---

## 📌 Core Features Implemented in the Notebook

1. **Local Text Generation:** Initialized Hugging Face causal language models (`gpt2`) and wrapped them inside LangChain's pipeline integration for prompt chaining[cite: 10].
2. **Text Splitting:** Configured `RecursiveCharacterTextSplitter` with customized chunk sizes and overlaps for processing large text data[cite: 10].
3. **Dense Embeddings:** Generated 768-dimensional vector embeddings using pre-trained sentence transformer models (`all-mpnet-base-v2`)[cite: 10].
4. **FAISS Vector Indexing & Local Persistence:** Indexed document embeddings locally using FAISS, performed similarity searches with distance scores, and saved/reloaded index files (`faiss_index`)[cite: 10].

---

## 💻 Sample Code Workflow
* **Text Generation Chain Example:**
  ```python
  from langchain_core.prompts import PromptTemplate

  template = "Question: {question}\nAnswer: Let's think step by step."
  prompt = PromptTemplate(template=template, input_variables=["question"])
  chain = prompt | local_llm
  response = chain.invoke({"question": "What is machine learning?"})
  print(response)

```

* **FAISS Similarity Search Example:**
```python
query = "What is FAISS used for?"
results = db.similarity_search(query, k=1)
print(results[0].page_content)

```



```



---

<ElicitationsGroup>
  <Elicitation label="Explain more code blocks" query="Can you walk me through specific code blocks inside my Langchain_and_Huggingface1.ipynb file?"/>
  <Elicitation label="Add project license" query="How do I add an open-source MIT license to my GitHub repository?"/>
</ElicitationsGroup>

```
