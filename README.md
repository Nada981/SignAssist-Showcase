# Taraf (SignAssist): Egyptian Sign Language (ESL) Avatar & Accessibility Ecosystem

An end-to-end accessibility platform engineered to bridge communication and structural barriers for individuals with hearing, speech, and motor disabilities. The ecosystem seamlessly integrates an AI-driven video-to-3D sign translation pipeline with an intelligent accessibility geo-assistant and a dedicated social community.

> **Note:** The source code and custom motion dataset are private due to university graduation project policies and intellectual property restrictions. The overall system architecture, conceptual pipeline, and core feature sets are documented below for demonstration purposes.

---

## 🔑 Key Features

- **Speech-to-3D ESL Translation:** Processes uploaded media, transcribes Egyptian Arabic audio, and streams synchronized 3D Egyptian Sign Language avatar animations in real time.
- **Dynamic Multi-Tier Motion Mapping:** A hybrid NLP fallback engine that maps transcribed text to structured 3D skeletal keypoint data (`Pose`, `Face`, `Hands`) using multi-level granularity (Full-Sentence, Word-Level, and Letter Spelling).
- **Asynchronous Chunked Streaming:** A resilient backend architecture designed for long-video processing, featuring video re-encoding, automated chunk segmentation, and asynchronous background worker queues.
- **RAG Accessibility Geo-Assistant:** An intelligent conversational assistant powered by a Multi-LLM fallback mechanism to recommend verified wheelchair-accessible venues and places in Egypt with automatic Google Maps routing.
- **Inclusive Social Community:** A secure, interactive social space supporting custom user profiles, anonymous post sharing, and peer reviews regarding accessibility infrastructure.

---

## 🏗️ High-Level System Architecture

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

## 🛠️ Technology Stack Overview

* **Mobile & Front-End:** Flutter (Cross-platform UI) & Unity 3D Engine (Skeleton Visualizer)
* **AI Core & NLP:** Speech-to-Text Transcriber, Semantic Sentence Transformers (XLM-RoBERTa), Arabic Text Normalization
* **Backend Infrastructure:** Python, FastAPI, Pydantic, Background Tasks Architecture
* **Database & Security:** Supabase Engine (Row-Level Security, Auth, Relational Schema)
* **Language Models (RAG Engine):** Retrieval-Augmented Generation using Multi-LLM Failover Router (Gemini, Grok, Cohere)
* **Containerization & Deployment:** Docker, Hugging Face Spaces

---

## 📄 License & Intellectual Property

© 2025/2026 Taraf Team. All rights reserved.

All codebase components, dataset mappings, and proprietary 3D skeletal motion files remain private and subject to academic IP guidelines.
```
