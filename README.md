# RFP-Management-System
An end-to-end AI-powered platform that automates the entire Request for Proposal (RFP) creation, evaluation, and lifecycle management process. This system reduces manual effort, improves accuracy, and speeds up decision-making using LLMs, ML-based scoring, and workflow automation.

## Overview
The **AI-RFP-System** consists of two major components:

- *Backend* (Python/FastAPI)
  - Handles authentication, RFP ingestion, AI scoring, versioning, workflows, and database management.

- *Frontend* (React + Tailwind)
  - A clean UI for creating RFPs, reviewing AI-generated scores, managing proposals, and tracking status.

This project is designed to resemble real enterprise RFP automation software used in procurement, enterprise sales, and vendor management.

## Project Structure
```pgsql
ai-rfp-system/
│
├── backend/
│   ├── app/
│   │   ├── api/
│   │   ├── core/
│   │   ├── models/
│   │   ├── schemas/
│   │   ├── services/
│   │   └── utils/
│   ├── requirements.txt
│   └── README.md
│
├── frontend/
│   ├── src/
│   ├── public/
│   └── README.md
│
└── README.md   ← (This file)
```

## Features

1. **AI-based Proposal Scoring**
    - LLM-based semantic similarity scoring
    - Weighted scoring by category (tech, pricing, compliance, SLA, etc.)
    - Custom business-logic scoring models
2. **RFP Creation & Management**
    - Create structured RFPs (sections, questions, scoring)
    - Upload PDFs/Docs → Extract requirements using AI
    - Automatic version history
3. **Vendor Proposal Evaluation**
    - Upload vendor responses
    - AI auto-maps answers to RFP questions
    - Generates:
        - Scores
        - Strengths & weaknesses
        - Risk flags
        - Summary report
4. **Workflow Automation**(Future Goal)
    - Status tracking: Draft → Published → Under Review → Awarded
    - Role-based access (Admin, Reviewer, Vendor)
5. **Dashboards & Analytics**(Future Goal)
    - Proposal comparison
    - Heatmaps
    - Time taken to evaluate
    - Category-weight analytics





