AARY TAGARE

AI Engineer | Applied AI / ML | Generative AI | RAG | NLP

Kolhapur, Maharashtra, India  •  tagareaary@gmail.com  •  +91-9175498114
LinkedIn: linkedin.com/in/aary-tagare14  •  GitHub: github.com/aarya008


## 1. Personal & Professional Overview

Aary Tagare is an Electrical Engineering graduate who transitioned toward Artificial Intelligence and Machine Learning after developing a strong interest in AI during research for a review paper on AI-enabled home automation. His current direction is applied AI engineering: building practical systems that combine Python, NLP, machine learning, generative AI, retrieval-augmented generation, vector databases, and APIs.

The strongest evidence of this transition is a progression from electrical/embedded engineering into document intelligence, RAG systems, computer vision, and conversational AI. His work emphasizes end-to-end pipelines rather than isolated model experiments.


## 2. Education


## 3. Transition from Electrical Engineering to AI/ML

During the B.Tech period, Aary developed an interest in Artificial Intelligence and Machine Learning while researching the review paper “A Review on IoT-Enabled Smart Homes Using AI.” The research exposed him to AI-driven automation and motivated a deliberate career shift toward AI/ML.

Rather than abandoning his engineering background, his trajectory combines it with software and AI. This is visible in both the embedded/automotive work completed during his internship and the later development of RAG, NLP, computer-vision, and conversational-AI systems.


## 4. Professional Experience


### Koptotech LLP — AI Engineer Intern

Jan 2026 – Present | Kolhapur

- Built a production-oriented face recognition system using InsightFace (RetinaFace + ArcFace) and ChromaDB vector search.

- Implemented cosine-similarity matching across multi-album image collections with O(1) deduplication using in-memory ID sets.

- Developed a closed-eye detection pipeline using 106-point facial landmarks, affine-aligned eye crops, and batch ViT inference with Hugging Face Transformers and PyTorch.

- Reduced per-photo model calls by approximately 60% through single-forward-pass batching.

- Work demonstrates practical experience taking computer-vision models beyond experimentation into scalable processing pipelines.


### Elmos Semiconductor — Project Intern

Sep 2024 – Mar 2025 | Kolhapur

- Designed PCB schematics for microcontroller-based motor-control systems using the M53306B driver for automotive cooling-fan applications.

- Worked with embedded C firmware for BLDC motor control.

- Processed temperature and Hall-sensor inputs to regulate motor speed and coil energization.

- Gained hands-on experience in embedded systems, hardware interfacing, technical documentation, and structured engineering workflows.


## 5. Major AI / ML Projects


### Automotive Manual Intelligence System — RAG

Technologies: Python, LangChain, ChromaDB, vector embeddings, semantic search, Streamlit, FastAPI

- Built an end-to-end RAG-based AI assistant capable of answering natural-language questions over 1,000+ pages of automotive manuals.

- Developed TOC-aware parsing and semantic chunking to improve retrieval quality.

- A later benchmark of the hybrid retrieval pipeline reported 89% retrieval accuracy, compared with 72% for basic RAG and 65% for keyword search.

- Implemented per-chunk metadata including vehicle-system detection, safety-level classification, and content-type identification.

- Added multi-manual indexing, conversational memory, PDF upload, real-time vector indexing, and source citations.

- Deployed the application on Streamlit Community Cloud and designed the system around practical document-intelligence workflows.


### NLP-Based Resume Screening System

Technologies: Python, NLP, TF-IDF, cosine similarity, PDF parsing, scikit-learn

- Designed an end-to-end system to evaluate and rank resumes against job descriptions for automated shortlisting.

- Built a modular PDF parsing and text-preprocessing pipeline.

- Used TF-IDF vectorization and cosine similarity to calculate candidate–job relevance.

- Created a scoring and ranking engine that exports structured, sortable results in CSV format.

- Designed the architecture to support future ATS/CRM integration and extension toward semantic or embedding-based matching.


### Personal AI Voice Assistant — Ongoing

Technologies explored: Python, Qwen 3.5 4B, Whisper, Windows-native Edge TTS

- Developing a personal voice-assistant pipeline around speech-to-text, an LLM reasoning layer, and text-to-speech.

- Using Qwen 3.5 4B as the local language model component.

- Evaluating Whisper Medium for CPU-based speech recognition so GPU resources can remain available for the local LLM.

- Using Windows-native Edge TTS for speech synthesis.

- The project reflects an interest in practical local AI systems, latency/resource trade-offs, and multimodal conversational interfaces.


### AI-Powered Educational Visualization — Exploration

- Explored generating HTML5-based visual explanations for educational questions such as free fall.

- Focuses on converting natural-language concepts into interactive visual explanations rather than only returning text.

- Represents an interest in AI-assisted educational interfaces and explainable/visual learning experiences.


### Customer Dish Preference Predictor & Data Pipeline

Technologies: Python, Pandas, NumPy, LightGBM, Optuna, SQL, data engineering, feature engineering, data validation, time-aware validation, predictive modeling

- Built an end-to-end data pipeline for customer purchasing and dish-preference analytics using more than 1.5 million records spanning 22 food categories.

- Designed the pipeline to handle data sourcing, cleansing, transformation, mapping, feature construction, validation, and preparation of production-ready analytical datasets.

- Engineered 150+ temporal, behavioral, and demographic features to capture customer purchasing patterns and improve prediction quality.

- Implemented data-quality validation before modeling, checking missing values, inconsistent records, mappings, and feature integrity.

- Developed and trained a LightGBM classification model to predict customer dish preferences and support campaign-oriented consumer analytics.

- Used Optuna for automated hyperparameter optimization to systematically improve model configuration.

- Applied time-aware validation to reduce temporal leakage and provide a more realistic estimate of performance on future customer behavior.

- Trained and evaluated the model on datasets containing more than 1 million records, achieving 65.9% Top-3 accuracy and 83.2% Top-5 accuracy.

- Built reusable data-processing and feature-engineering stages so the pipeline could support downstream analytics, reporting, and model inference.

- Automated parts of the data-sourcing and preparation workflow, reducing manual data-handling effort by more than 40%.

- Complete ML workflow: raw data → cleaning → validation → feature engineering → model training → hyperparameter tuning → time-aware evaluation → prediction and analytics.


### AI Face Search & Recognition System — Wedding Album Intelligence

Technologies: Python, RetinaFace, ArcFace, QdrantDB, FastAPI, Celery/Redis, OpenCV, PyTorch, Hugging Face Transformers, ViT, facial landmarks, vector embeddings

- Built an end-to-end computer-vision system for searching and identifying people across large wedding-photo collections.

- Used RetinaFace for face detection and alignment, followed by ArcFace to generate discriminative facial embeddings for identity matching.

- Stored and searched face embeddings with QdrantDB vector search, enabling fast similarity-based retrieval across multi-album collections.

- Implemented cosine-similarity matching and in-memory ID-set deduplication to avoid repeated identities while processing large numbers of images.

- Built backend APIs with FastAPI and asynchronous batch processing with Celery/Redis; AWS Transfer Family was used in the broader ingestion workflow.

- Engineered closed-eye detection using 106-point facial landmark extraction and ViT-based classification, with affine-aligned eye crops.

- Optimized inference by batching eye crops into a single forward pass, reducing model inference calls by approximately 60%.

- Achieved approximately 90% production recognition accuracy; the closed-eye detection component achieved about 80% accuracy.

- The project demonstrates practical experience with the complete vision pipeline: image ingestion → face detection → embedding generation → vector indexing → similarity search → deduplication → structured results.


### AI Data Analyst Agent — Conversational Analytics Platform

Technologies: Python, FastAPI, Streamlit, LangChain, Groq, SQL, Pandas, NumPy, CSV, Excel, PostgreSQL, data profiling, NL-to-SQL, Python code generation

- Developed an agentic AI data-analysis platform that allows users to explore datasets through natural-language conversation instead of manually writing SQL or Python.

- Designed the system to work with CSV, Excel, and PostgreSQL sources, including datasets exceeding 1 million rows.

- Implemented a multi-agent workflow using LangChain and Groq to route analytical tasks and generate the appropriate SQL, Python analysis, or visualization logic.

- Built an NL-to-SQL workflow that translates natural-language questions into executable database queries for structured analytical retrieval.

- Added Python code-generation capabilities for data transformation, statistical analysis, calculations, and visualization tasks that are better handled outside SQL.

- Implemented automated data profiling and ingestion-time data-quality checks to identify missing values, anomalies, schema issues, and other problems before analysis.

- Added sandboxed execution for generated analytical code, along with retry/error-handling logic to improve robustness when generated queries or code fail.

- Produced structured analytical outputs, reporting summaries, and visualization-ready results through a conversational interface.

- Exposed the core functionality through a RESTful FastAPI backend while using Streamlit for an interactive user-facing analytics experience.

- Designed the system around non-technical users: the goal is to turn a business question into data retrieval, analysis, visualization, and an understandable answer with minimal manual intervention.

- Current performance target/benchmark: average response times below 3 seconds for supported analytical workflows.


## Data Engineering & Predictive Modeling Capability

- Large-scale structured-data processing: 1.5M+ records across 22 food categories.

- Feature engineering: 150+ temporal, behavioral, and demographic features.

- Predictive model: LightGBM classification.

- Optimization: Optuna hyperparameter optimization.

- Validation: time-aware validation to reduce temporal leakage.

- Measured performance: 65.9% Top-3 and 83.2% Top-5 accuracy.

- Pipeline automation: reduced manual data handling by 40%+.

- Business objective: customer purchasing behavior, dish-preference prediction, and campaign analytics.


## 13. Project Architecture & Engineering Themes

Across these projects, Aary has repeatedly worked on end-to-end AI pipelines rather than isolated models. Common architecture patterns include ingestion → preprocessing → model/LLM processing → vector/database layer → API/application layer → evaluation and monitoring.

- RAG / Document Intelligence: document ingestion, TOC-aware parsing, semantic chunking, metadata enrichment, embeddings, ChromaDB, retrieval, LLM generation, citations and conversational memory.

- Computer Vision: image ingestion, face detection/alignment, embedding generation, vector search, similarity scoring, deduplication, batch inference and API serving.

- AI Analytics: structured data ingestion, profiling and quality validation, NL-to-SQL/code generation, sandboxed execution, visualization, reporting and conversational delivery.

- ML Prediction: large-scale feature engineering, time-aware validation, hyperparameter optimization, model evaluation and production-oriented data pipelines.

- Engineering: modular Python architecture, REST APIs with FastAPI, asynchronous processing, vector databases, Git, Docker/cloud-oriented deployment, and performance optimization.


## 6. Research & Publication


### A Review on IoT-Enabled Smart Homes Using AI

Published in the 15th International Conference on Computing, Communication and Networking Technologies (ICCCNT), IIT Mandi, 2024.

Author: Aary Tagare, et al.

DOI: 10.1109/ICCCNT61001.2024.10723321

This research was an important turning point in Aary’s career direction: research into AI-enabled home automation helped develop the interest that ultimately led to pursuing AI/ML engineering.


## 7. Technical Skill Set

Programming: Python, Java, SQL, Embedded C

AI / ML: Machine Learning, NLP, PyTorch, scikit-learn, computer vision

Generative AI: LLMs, RAG, vector embeddings, semantic search, prompt engineering

Frameworks & Libraries: LangChain, Hugging Face Transformers, Pandas, NumPy, Matplotlib, Seaborn

Vector / Data Systems: ChromaDB, document ingestion pipelines, PDF processing, data pipelines

Backend / Deployment: FastAPI, Docker, Streamlit, Git

Engineering Fundamentals: OOP, data structures, algorithms, SDLC, computer networks, operating systems

Embedded / Hardware: PCB schematic design, microcontrollers, BLDC motor control, Hall sensors, motor drivers


## 8. Certifications & Learning

- IBM Generative AI Engineering Professional Certificate

- Google Cybersecurity Professional Certificate


## 9. Achievements

- Project-Based Learning (PBL) Competition — Runner-Up, 2022 and 2024.


## 10. Interests & Direction

- Applied Artificial Intelligence and Machine Learning

- Generative AI and LLM applications

- Retrieval-Augmented Generation and document intelligence

- NLP and semantic search

- Computer vision and AI-powered image processing

- Conversational AI and local AI assistants

- Automation and intelligent software systems

- Nature photography and videography


## 11. Career Profile

Aary’s profile is best characterized as an early-career Applied AI Engineer with an Electrical Engineering foundation. The differentiator is not the degree itself, but the ability to bridge engineering systems with modern AI software: embedded/automotive exposure, followed by hands-on work in NLP, RAG, vector databases, computer vision, and local conversational AI.

Current career direction: AI Engineer / ML Engineer / Generative AI Engineer, with particular strength in RAG systems, NLP, document intelligence, computer vision, and end-to-end AI application development.


## 12. Source & Accuracy Notes

This profile consolidates information supplied in the current conversation and information available from the user's previous career/resume materials and project discussions. Where earlier resume versions contained different diploma-score figures, the current user-provided figure of 76.94% is used here.


### Education

| Period | Institution | Qualification | Result |

| --- | --- | --- | --- |

| 2018–2019 | Sau. S. M. Lohia High School, Kolhapur | 10th / SSC Board | 86.20% |

| 2019–2022 | Government Polytechnic, Kolhapur | Diploma in Electrical Engineering | 76.94% |

| 2022–2025 | Kolhapur Institute of Technology, Kolhapur | B.Tech in Electrical Engineering | CGPA 8.1 |
