# SignAssist AI: Video-to-Sign Language Avatar & Accessibility Platform

An end-to-end accessibility solution designed to empower people with disabilities through AI-driven assistive tools. The platform enables users to upload video content, which is processed asynchronously through a computer vision and sequence translation pipeline to generate a synchronized sign language avatar translation, accompanied by an AI assistant for accessible locations.

> **Note:** The source code is private due to graduation project policies and intellectual property. The system architecture, features, and pipeline overview are documented below.

Key Features
Automated Video-to-Sign Translation: Users upload standard videos; the platform extracts audio/visual cues, processes the content through a translation model, and delivers the video accompanied by an animated sign language avatar.

Asynchronous Processing Pipeline: Efficient handling of video ingestion, sequence parsing, and avatar rendering workflows.

Accessibility Geo-Assistant: Intelligent assistant helping users identify wheelchair-accessible venues and ramps.

Inclusive Community: Dedicated platform for peer connection and sharing accessible location reviews.


Pipeline Overview

Plaintext
[ User Video Upload ]
         │
         ▼
[ Video & Audio Ingestion / Extraction ]
         │
         ▼
[ NLP & Sign Gloss Sequence Mapping ]
         │
         ▼
[ 3D Avatar Translation & Rendering ]
         │
         ▼
[ Processed Video Delivery to User ]

Tech Stack
Core & AI Processing: Python, OpenCV, MediaPipe / PyTorch

API Framework: FastAPI, Pydantic

Containerization & Version Control: Docker, Git

Author
Developed with a focus on Applied AI Engineering and Assistive Technologies.