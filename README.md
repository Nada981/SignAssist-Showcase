# Taraf (SignAssist): Egyptian Sign Language (ESL) Platform

Taraf is an advanced end-to-end accessibility platform designed to bridge communication and structural barriers for individuals with hearing, speech, and motor disabilities. The system integrates an AI-driven video-to-3D sign translation pipeline, an intelligent accessibility geo-assistant, and a secure social community hub.

> **Note:** The source code and custom motion dataset are kept private to protect proprietary implementation details. This repository serves as a high-level technical documentation and system architecture showcase.

---

## 🚀 Core Features & Technical Highlights

- **Speech-to-3D ESL Translation Pipeline:** Processes media inputs, extracts Egyptian Arabic speech via Speech-to-Text, and streams synchronized 3D Egyptian Sign Language avatar animations in real time.
- **Dynamic Multi-Tier Motion Mapping:** Engineered a hybrid NLP fallback engine mapping transcribed text to structured 3D skeletal keypoint data (`Pose`, `Face`, `Hands`) with multi-level granularity (Full-Sentence, Word-Level, and Letter Spelling).
- **Asynchronous Chunked Backend:** Built a resilient backend architecture for heavy video processing, featuring automated FFmpeg re-encoding, chunk segmentation, and asynchronous background worker queues.
- **RAG Accessibility Geo-Assistant:** Implemented an intelligent conversational assistant powered by a Multi-LLM fallback mechanism to recommend verified wheelchair-accessible venues with automatic routing.
- **Secure Community Platform:** Developed a robust social hub supporting custom user profiles, anonymous posting, and peer-reviewed infrastructure accessibility ratings.

---

## 🏗️ System Architecture Workflow

```text
[ User Video Upload / Media Ingestion ]
                 │
                 ▼
[ Background Processing & Chunking Pipeline ]
                 │
                 ▼
[ Egyptian Arabic Speech-to-Text Transcriber ]
                 │
                 ▼
[ Semantic Text Normalization & Hybrid NLP Matcher ]
                 │
                 ▼
[ Skeletal Motion Coordinate Resolver (JSON Timeline) ]
                 │
                 ▼
[ 3D Avatar Rendering Engine & Real-Time Sync ]

```

---

## 🛠️ Technology Stack

* **Mobile & Frontend:** Flutter (Cross-Platform UI), Unity 3D Engine (Skeleton Visualizer)
* **AI & NLP Core:** Speech-to-Text (STT), Sentence Transformers (XLM-RoBERTa), Arabic Text Normalization
* **Backend & API:** Python, FastAPI, Pydantic, Background Tasks
* **Database & Security:** Supabase (Row-Level Security, Auth, Relational Schema)
* **RAG Engine & LLMs:** Retrieval-Augmented Generation, Multi-LLM Failover Router (Gemini, Grok, Cohere)
* **Deployment & Containerization:** Docker, Dockerfile, Hugging Face Spaces

---

## 📄 License & Intellectual Property

© 2025/2026 Taraf Development. All rights reserved.

*All codebase components, proprietary dataset mappings, and 3D skeletal motion files remain private.*
