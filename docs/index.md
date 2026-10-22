# Vu Hoang Tue Anh

I am a Computer Science student at VinUniversity. I have built projects spanning backend REST APIs, Kafka message queues, data pipelines and AI/multimodal systems, and I have a foundation in API testing.

I am currently learning test automation with Playwright and Selenium, plus Agile/Scrum.

---

## 📞 Contact Information

- **Phone:** [+84 933 256 166](tel:+84933256166)
- **Email:** [24anh.vht@vinuni.edu.vn](mailto:24anh.vht@vinuni.edu.vn)
- **Location:** Hanoi

---

## 🛠️ Technical Skills

| **Category** | **Skills & Technologies** |
|---|---|
| **Languages** | Python, JavaScript (Node.js), SQL |
| **Backend & APIs** | Node.js, Express, REST APIs, transactional outbox, idempotent consumers |
| **Databases & Search** | PostgreSQL (transactions, row-level locking), Redis, Elasticsearch |
| **Messaging & Streaming** | Apache Kafka, Debezium CDC, Apache Flink SQL |
| **Data Engineering** | PySpark, dbt (star schema, SCD2), Great Expectations, Parquet, S3-compatible object storage, batch and streaming data pipelines |
| **AI / LLMs** | PyTorch, Transformers, TRL, PEFT/LoRA, SFT, GRPO, CoT curation, vLLM, model evaluation |
| **Retrieval & RAG** | Faiss (IVF), BGE-M3, bge-reranker-v2-m3, BM25, e5, VinAI Translate (VI→EN), scikit-learn, LightGBM |
| **Multimodal** | CLIP, Gemini-2.5-Flash image captioning, visual question answering |
| **Testing** | Manual Testing, Postman, Test Execution, Playwright, HTML, XPath locators, Webhooks, unit / integration / end-to-end testing |
| **Tools** | Git, Docker, Docker Compose, Jira |

---

## 🎓 Education

### VinUniversity

**Bachelor's Degree in Computer Science** | *2024 – Present*

- 95% Merit-Based Scholarship; Dean's List, 2024–2025
- Relevant coursework: Object-Oriented Programming, Database Systems, Artificial Intelligence, Machine Learning

---

## 🚀 Featured Projects

### Anhbnb — Lodging Booking Backend

**Backend project** | *Completed · Aug – Sep 2026*

| **Aspect** | **Details** |
|---|---|
| **Project** | Backend for a lodging booking service, built individually. |
| **Booking & Concurrency** | REST APIs with Node.js and Express. PostgreSQL transactions and row-level locking manage concurrent room bookings, with Redis for caching and coordination. |
| **Events & Search** | A transactional outbox with Debezium CDC and Kafka updates Elasticsearch search indexes and invalidates caches through idempotent consumers. |
| **Testing** | APIs tested with Postman; unit, integration and end-to-end tests for booking flows and event processing. |
| **Technologies Used** | Node.js, Express, PostgreSQL, Redis, Kafka, Debezium, Elasticsearch, Docker Compose, Postman |
| **Repository** | [github.com/tertueanhvu/Anhbnb--backend-project](https://github.com/tertueanhvu/Anhbnb--backend-project) |

---

### Divvy Data Platform

**Data pipeline project** | *In progress*

| **Aspect** | **Details** |
|---|---|
| **Project** | Team data engineering project on Divvy, Chicago's bike-share system. |
| **Batch** | Monthly trip files are transformed with Spark into Parquet on an S3-compatible lake, loaded into PostgreSQL and modeled into dbt marts. |
| **Streaming** | Live station status is polled from the public GBFS feed every 2 minutes and published to Kafka; a Flink SQL job over 10-minute sliding windows raises alerts for stations that run out of bikes or docks. |
| **Data Quality** | Each batch is validated with Great Expectations before loading. |
| **Technologies Used** | Python, PySpark, Kafka, Flink SQL, PostgreSQL, dbt, Great Expectations, Docker Compose |
| **Details** | [Description, architecture and status →](projects/divvy.md) |

---

### MEWA — Budgeted Vietnamese–English Legal Evidence Retrieval

**RAG project** | *In progress*

| **Aspect** | **Details** |
|---|---|
| **Project** | Retrieval layer of a cross-lingual legal RAG system for Vietnamese legal questions. |
| **Approach** | Before searching, decides how to split a fixed Faiss IVF search budget between a Vietnamese and an English index, using a gradient-boosted utility model over pre-search signals. |
| **Pipeline** | VI→EN machine translation, BGE-M3 encoding, Faiss IVFFlat indexes and bge-reranker-v2-m3 scoring; evaluation reports recall, regret and budget violations with 95% confidence intervals. |
| **Technologies Used** | Python, Faiss, BGE-M3, bge-reranker-v2-m3, scikit-learn, vLLM |
| **Details** | [Description, architecture and status →](projects/mewa.md) |

---

### MC-GRPO — Mode-Conditioned GRPO for Math Reasoning

**LLM project** | *Completed · individual course project (COMP2050)*

| **Aspect** | **Details** |
|---|---|
| **Project** | Custom GRPO trainer with mode-specific completion-length scaling for Llama 3.2 3B. |
| **Evaluation** | Compared against matched GRPO on GSM8K and MATH500. |
| **Result** | 80.52% GSM8K zero-shot accuracy versus 77.45% for matched GRPO (single-seed experiment). |
| **Repository** | [github.com/tertueanhvu/COMP2050--MC-GRPO](https://github.com/tertueanhvu/COMP2050--MC-GRPO) |

---

### Curating Multi-Mode CoT for Efficient Math Reasoning with GPT-OSS

**Co-first author** | *ICISN 2026*

| **Aspect** | **Details** |
|---|---|
| **Project** | Co-developed a pipeline to curate low-, medium- and high-effort GPT-OSS-20B reasoning traces for GSM8K and MATH using answer verification and mode-specific length filtering; fine-tuned Llama 3.2 3B with LoRA. |
| **Result** | Low-mode SFT followed by GRPO achieved 80.06% GSM8K and 47.60% MATH500 zero-shot accuracy. |
| **Repository** | [github.com/hugebenevolence/LLaMA-OSS](https://github.com/hugebenevolence/LLaMA-OSS) |

---

### Difficulty-Aware Adaptive Reasoning for Vietnamese VQA with GPT-OSS

**Co-author** | *AICI 2026*

| **Aspect** | **Details** |
|---|---|
| **Project** | Co-developed a training-free visual question answering pipeline that combines Gemini-2.5-Flash image captions with CLIP image-caption similarity to route GPT-OSS questions to low, medium or high reasoning modes. |
| **Result** | On ViVQA-X, adaptive reasoning achieved 0.4214 METEOR and reduced inference time by over 75% versus always-high reasoning. |
| **Repository** | [github.com/hugebenevolence/ViVQA-GPT-OSS-DRA](https://github.com/hugebenevolence/ViVQA-GPT-OSS-DRA) |
