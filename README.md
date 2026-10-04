# SignAssist AI: Egyptian Sign Language (ESL) Avatar & Accessibility Platform

An end-to-end accessibility solution designed to empower people with hearing and speech disabilities through AI-driven assistive tools. The platform enables users to upload video content, extracts spoken audio, and asynchronously translates Egyptian Arabic speech into synchronized 3D Egyptian Sign Language (ESL) avatar animations using predefined skeletal motion keypoints (JSON mapping).

> **Note:** The source code is private due to graduation project policies and intellectual property. The system architecture, animation pipeline, and features are documented below.


---

## Key Features

* **Speech-to-ESL Translation:** Extracts spoken Egyptian Arabic dialogue from uploaded videos and transcribes it via Speech-to-Text (STT).
* **JSON Skeletal Motion Mapping:** Matches recognized terms to corresponding 3D skeleton keypoint coordinates stored in structured JSON dictionaries to drive realistic avatar gestures.
* **Asynchronous Video Processing:** Efficient queue and processing pipeline handling video ingestion, audio extraction, sign gloss mapping, and avatar rendering.
* **Accessibility Geo-Assistant:** Intelligent assistant helping users identify wheelchair-accessible venues and ramps.
* **Inclusive Community:** Dedicated platform for peer connection and sharing accessible location reviews.

---

## Pipeline Overview

```text
[ User Video Upload ]
         │
         ▼
[ Audio Extraction & Egyptian Arabic STT ]
         │
         ▼
[ NLP Text Parsing & Word Alignment ]
         │
         ▼
[ JSON Skeleton Coordinates Retrieval ]
         │
         ▼
[ 3D Avatar Motion Animation & Rendering ]
         │
         ▼
[ Final Synchronized Video Delivery ]

```

---

## Tech Stack

* **Audio & Speech Processing:** Python, Speech-to-Text (STT) Pipelines
* **Animation & Data Structure:** JSON (3D Skeletal Motion Keypoints), Blender / 3D Avatar Engine
* **API Framework:** FastAPI, Pydantic
* **Containerization & Version Control:** Docker, Git

---

## Author

Developed with a focus on Applied AI Engineering and Assistive Technologies.
