# 🧠 Agentic RAG Memory Sharing with TiDB Serverless

This project demonstrates how multiple RAG (Retrieval-Augmented Generation) agents can **write, share, and retrieve memory** using [TiDB Serverless](https://tidbcloud.com) as a collaborative memory backend. It supports **short-term and long-term memory**, and uses **vector search** for contextual retrieval.

Built with:
- 🐍 Python + [PyTiDB](https://github.com/pingcap/pytidb)
- 🔍 OpenAI Embeddings (e.g., `text-embedding-ada-002`)
- 🧠 TiDB Vector Search

---

## 📁 Project Structure

- `rag_shared_memory_tidb_pytidb_final.ipynb`  
  → Jupyter Notebook demonstrating full memory flow:
  - Insert memory with OpenAI embedding
  - Store vector in TiDB
  - Perform vector search to retrieve shared memory

- `Bots.sql`  
  → Shared memory in action with multi-agent system.

---

## 🚀 Features

- ✅ Store short/long-term memory with metadata & expiration
- ✅ Use `Vector` column for similarity-based retrieval
- ✅ Memory access control with `private`, `team`, `public` visibility

---

## 📦 Requirements

- Get your TiDB connection string.
- LLM API Key from OpenAI or BedRock.
- To get started, put duplicate an `env` file from `env.template` and put above keys into the file. Then just run the notebooks.

