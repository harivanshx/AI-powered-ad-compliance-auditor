# AI Video Advertisement Compliance Auditor

## Overview

This project is an AI-powered compliance auditing system for YouTube video advertisements. It automatically analyzes ad content, compares claims against regulatory rulebooks, and generates a pass/fail compliance report.

The system combines video indexing, semantic search, and LLM reasoning to simulate a regulatory audit workflow.

---

## How It Works

1. A user submits a YouTube video URL via FastAPI.
2. The video is downloaded and processed using Azure Video Indexer.
3. Transcript and OCR text are extracted from the video.
4. Regulatory PDFs are indexed in Azure AI Search.
5. Relevant legal sections are retrieved using vector search.
6. An LLM evaluates claims vs regulations.
7. A structured compliance report is generated.

---

## Architecture Flow


YouTube URL
   ↓
FastAPI Backend
   ↓
Video Download
   ↓
Azure Video Indexer
   ↓
Transcript + OCR Extraction
   ↓
Azure AI Search (Law Retrieval)
   ↓
LangGraph + LLM Reasoning
   ↓
Compliance Report (Pass / Fail)

---

## Core Components

* **FastAPI** — API gateway and orchestration trigger
* **Azure Video Indexer** — Transcript + OCR extraction
* **Azure AI Search** — Regulatory document retrieval
* **LangGraph** — Agentic reasoning workflow
* **LLM (GPT)** — Compliance analysis
* **Azure Application Insights** — Monitoring
* **LangSmith** — Observability and tracing

---

## Output

The system produces:

* Compliance verdict (Pass / Fail)
* Detected violations
* Supporting evidence
* Referenced regulations

---

## Use Cases

* Ad compliance verification
* Regulatory auditing automation
* Brand claim validation
* Pre-publication review pipelines

---

## Future Enhancements

* Multi-region regulatory support
* Human-in-the-loop review
* Confidence scoring
* Dashboard analytics

---
