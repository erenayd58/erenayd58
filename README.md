Eren Aydemir
AI Engineering — LLM Systems, RAG & Agentic AI

I build LLM-powered systems where the model is one component inside a pipeline that can be inspected: deterministic control around model calls, explicit provenance, validated structured outputs, and results reported as they actually ran.

Final-year Mechatronics Engineering student at Yıldız Technical University, focused on applied AI engineering. Open to part-time and long-term opportunities in LLM systems, agentic AI, RAG and applied ML.

📫 erenayd58@gmail.com · LinkedIn · Medium

Focus
LLM systems & RAG — chunking strategies, hybrid retrieval (dense + BM25), citation-grounded answering
Agentic AI — tool-using pipelines with deterministic logic around the model
Evaluation & reliability — structured outputs, schema validation, field-level provenance, failure escalation
Applied ML & intelligent industrial systems — time-series modeling, federated learning, explainable AI, edge inference
Tech
Languages	Python · TypeScript · C/C++ · SQL · Dart
LLM & RAG	OpenAI-compatible APIs (OpenAI, OpenRouter, Azure), Ollama, structured outputs, pgvector, BM25, RRF fusion, cross-encoder reranking, tiktoken
Backend & Data	FastAPI, Pydantic, Flask, Docker, PostgreSQL 16 + pgvector, Supabase, ChromaDB, FAISS, NumPy
ML / DL	TensorFlow/Keras, scikit-learn, SHAP, LIME, Grad-CAM, TFLite, OpenCV
Other	Next.js / React, Linux, Git, pytest, Playwright, Ruff
Featured Projects
Chunk-Viewer — RAG system for comparing chunking strategies
A PDF is parsed once into canonical units, then partitioned by four interchangeable methods under one identical token budget — Markdown (baseline), Standard (structure-aware), Hybrid (embedding-based) and Deep Analysis (LLM proposer → deterministic quality selector → dual-pass validator) — so the only variable is where the boundaries fall. Retrieval fuses pgvector dense search with a deterministic Turkish BM25 via RRF, and answers cite their sources inline ([S1], [S2]). The Viewer shows each method's boundaries on the same text; a new chunking method registers as a single plugin file plus a test.

Python FastAPI PostgreSQL 16 + pgvector Next.js / React Docker — provider-agnostic (OpenAI-compatible endpoints or local Ollama)

areal.ai — Auditable document-AI pipeline (NLP/LLM take-home assignment)
An offline-first pipeline turning mortgage PDFs into loan-level results with source evidence preserved end to end. LLMs are restricted to interpreting unstructured content; deterministic code owns page identity, grouping, normalization, conflict rules and human-review escalation. Strict JSON parsing with Pydantic semantic validation, field-level provenance and audit trails, and a configurable reliability policy with deterministic conflict escalation. The optional OpenAI adapter uses Structured Outputs and sends store=False; tests run with network access blocked. The evaluation section reports the run as it happened, including the document that failed provenance validation.

Python Pydantic PyMuPDF OpenAI Structured Outputs pytest

pq-fedpredict — Federated + explainable predictive maintenance for CNC machines
A CNN-BiLSTM model with temporal attention and three heads — subsystem (6-class), fault (24-class taxonomy across spindle, tool, axis, coolant, hydraulic and power) and RUL regression — trained both centrally and federated (FedAvg / FedProx) across simulated clients with non-IID data. Includes a synthetic data generator for the fault taxonomy, SHAP / LIME / Grad-CAM explainability, TFLite INT8 export for Raspberry Pi 5 edge inference, a Dilithium signature proof-of-concept for model-integrity verification, and Docker + MLflow experiment infrastructure.

Python TensorFlow Federated Learning SHAP / LIME / Grad-CAM TFLite Docker MLflow

pusula — Multi-tenant study-tracking and coaching platform
A platform for 8th-grade LGS students with four roles (institution owner, coach, student, parent). Authorization is enforced in PostgreSQL through row-level security and tested with pgTAP; a custom access-token hook injects the role claim into the JWT for proxy-level routing. Playwright end-to-end tests run against a production build rather than the dev server.

Next.js TypeScript Supabase / PostgreSQL RLS + pgTAP Playwright

Background: Robotics & Embedded Systems
Hardware-in-the-loop work that preceded my focus on AI systems — useful context for industrial and edge AI.

TEKNOFEST — Autonomous Ground Vehicle (Software Team Lead): A* path planning on ROS; fused RPLIDAR, IMU and encoder data for autonomous driving scenarios; real-time monitoring via PyQt5 and a web interface.
YTÜ – BEKO Datathon 2025 — 1st place: predictive maintenance model on real sensor data (cleaning, modeling, validation).
Smart Cargo Box — TÜBİTAK BIGG programme: ESP32 + MQTT remote-controlled cargo box with a Flutter mobile app.
AI-assisted Heart Analysis — TEKNOFEST: ECG acquisition over ESP32 with real-time mobile analysis; signal processing and anomaly detection.
ROS 1/2 Gazebo / RViz / URDF ESP32 STM32 FreeRTOS MQTT Jetson Nano Flutter

Education & Writing
Yıldız Technical University — B.Sc. Mechatronics Engineering (ongoing) · Anadolu University — Computer Programming (on hold)

Certificates: Coderspace AI & Data Science Summer School · Miuul Python for Data Science · Udemy MATLAB Masterclass (in progress)

I write on Medium about NLP, LLMs, transformers and data analysis — plain-language explanations of things I've had to work through myself.
