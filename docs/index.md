# Vu Hoang Tue Anh

## QA / Software Tester

I am a Computer Science student at VinUniversity with a foundation in **API testing**. I have built projects spanning backend REST APIs, Kafka message queues, data pipelines and AI/multimodal systems.

I am currently learning test automation with Playwright and Selenium, plus Agile/Scrum, and I am eager to learn and grow in **software testing**.

---

## 📞 Contact Information

- **Phone:** [+84 933 256 166](tel:+84933256166)
- **Email:** [24anh.vht@vinuni.edu.vn](mailto:24anh.vht@vinuni.edu.vn)
- **Location:** Gia Lam, Hanoi

---

## 🛠️ Technical Skills

| **Category** | **Skills & Technologies** |
|---|---|
| **Testing** | Manual Testing, Postman, Test Execution, Playwright, HTML, XPath locators, Webhooks |
| **Currently learning** | Playwright and Selenium test automation, Agile/Scrum |
| **Backend** | Python, Node.js, Express, REST APIs, PostgreSQL, Redis, Kafka, Elasticsearch |
| **Data** | SQL queries, data pipelines |
| **Tools** | Jira, Git, Docker |
| **AI / ML** | PyTorch, Transformers, TRL, PEFT/LoRA, Faiss, vLLM |

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
