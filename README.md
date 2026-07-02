# TalentFlowAI

## 🚀 Because Great Talent Should Never Be Lost.

TalentFlowAI is an AI-powered Recruitment Orchestration Platform built using **UiPath Maestro** that intelligently matches candidates to the most suitable job opportunities, automates recruitment workflows, and enables recruiters to hire the right talent faster.

---

# 📐 Solution Architecture

The complete end-to-end UiPath Maestro orchestration flow can be found here:

📄 **[View Maestro Process Flow](Architecture/Maestro_Process_Flow.pdf)**

---

# 🌟 Overview

Traditional recruitment is often focused on filling a single job opening. As a result, highly qualified candidates are frequently rejected simply because they are not the perfect fit for one position.

TalentFlowAI changes this approach by evaluating every candidate against **multiple job opportunities** across the organization. Instead of rejecting great talent, the platform intelligently identifies the best available role using AI-powered reasoning, semantic job matching, and enterprise recruitment data.

Built on **UiPath Maestro**, TalentFlowAI combines AI Agents, Human-in-the-Loop approvals, Data Service, Integration Service, and event-driven workflows to orchestrate the complete recruitment lifecycle—from receiving a candidate application to interview scheduling and HR verification.

---

# 🎯 Problem Statement

Recruitment teams face numerous operational challenges:

- Thousands of recruitment emails every day
- Manual resume screening
- Duplicate candidate applications
- Manual ATS evaluation
- Cooling period verification
- Missing candidate information
- Recruiter follow-ups
- Interview scheduling complexity
- Hiring deadline pressure
- Losing highly qualified candidates due to manual decision making

TalentFlowAI addresses these challenges through intelligent AI-powered orchestration.

---

# ✨ Key Features

- 🤖 AI-powered Resume Understanding
- 🎯 Semantic Multi-Job Matching
- 📊 Multi-Job ATS Scoring
- 👤 Duplicate Candidate Detection
- 📄 Automated Candidate Information Collection
- 🔄 Cooling Period Validation
- 🧠 AI-powered Recruitment Decision Support
- 👥 Human-in-the-Loop Approvals
- 📅 Automated Interview Scheduling with Calendly
- ⚡ Event-driven Long Running Workflows
- 🔍 AI Vector Search using UiPath GenAI Activities
- 📂 Document Collection

---

# 🏗 Technology Stack

| Component | Purpose |
|------------|---------|
| UiPath Maestro | End-to-End Process Orchestration |
| UiPath Agent Builder | AI Agents |
| UiPath Studio | Workflow Development |
| UiPath Data Service | Candidate & Recruitment Data |
| UiPath Apps | Candidate Forms |
| UiPath Integration Service | Gmail, Calendly & Webhooks |
| UiPath Action Center | Human-in-the-Loop Decisions |
| UiPath Orchestrator | Process Execution |
| UiPath GenAI Activities | Semantic Job Search |
| Large Language Models | Resume Analysis & AI Decision Making |

---

# 🔄 High-Level Workflow


Candidate Application Email
          │
          ▼
Resume Understanding
          │
          ▼
Candidate Creation
          │
          ▼
Duplicate Candidate Check
          │
          ▼
Semantic Job Discovery
          │
          ▼
Multi-Job ATS Evaluation
          │
          ▼
Candidate Information Collection
          │
          ▼
Business Context Evaluation
          │
          ▼
AI Decision Making
          │
          ▼
Human Approval (When Required)
          │
          ▼
Interview Scheduling
          │
          ▼
Interview Feedback Collection
          │
          ▼
Document Collection

---

# 📂 Repository Structure

TalentFlowAI
│
├── Architecture
│   ├── Maestro_Process_Flow.pdf
│
├── DataService
│   ├── Schema.json
│
├── Demo
│   ├── 01_Why_TalentFlowAI.mp4
│   ├── 02_TalentFlowAI_Solution_Walkthrough.mp4
│
├── Setup
│   ├── SetupInstructions.md
│   └── Images
│
├── Solutions
│   ├── TalentFlowAI.uis
│   ├── Sync_Job_Vectors_Robot.uis
│
└── README.md

---

# 📦 Repository Contents

This repository includes everything required to deploy and run TalentFlowAI.

- ✅ TalentFlowAI Solution
- ✅ TalentFlowAI-Indexer Solution
- ✅ Complete Setup Guide
- ✅ Data Service Schema
- ✅ Maestro Process Flow
- ✅ Business Demonstration
- ✅ Technical Walkthrough

---

# 🚀 Getting Started

Follow the complete installation guide available in the **Setup** folder.

The guide walks you through:

- Importing UiPath Solutions
- Configuring Gmail Integration
- Configuring UiPath Data Service
- Configuring UiPath GenAI Activities
- Configuring Calendly
- Creating Calendly Webhook
- Importing the Data Service Schema
- Creating the Storage Bucket
- Creating the AI Vector Index
- Running TalentFlowAI-Indexer
- Running TalentFlowAI

📖 **Setup Guide:** `Setup/README.md`

---

# 🎥 Demo

## Business Demonstration

This video explains:

- The recruitment challenges
- Why TalentFlowAI was created
- How it transforms enterprise recruitment

📁 `Demo/01_Why_TalentFlowAI.mp4`

---

## Technical Walkthrough

This video demonstrates:

- Complete UiPath Maestro Workflow
- AI Agents
- Integration Service Connections
- Data Service
- Long Running Workflows
- Human-in-the-Loop
- End-to-End Execution

📁 `Demo/02_TalentFlowAI_Solution_Walkthrough.mp4`

---

# 🤖 AI Vector Index

TalentFlowAI uses **semantic search** to identify the most relevant job opportunities for every candidate.

The **Sync_Job_Vectors_Robot** solution is responsible for keeping the AI Vector Index synchronized with the latest job postings.

The workflow automatically:

- Reads the latest Job Postings from UiPath Data Service.
- Generates a CSV file containing all active job postings.
- Uploads the CSV file to a Storage Bucket.
- Updates the AI Vector Index with the latest data.

To ensure the Vector Index always reflects the current job openings, an **event-driven automation** has been implemented. Whenever a **Job Posting** is created, updated, or deleted in the UiPath Data Service, a Data Service event automatically triggers the **Sync_Job_Vectors_Robot** workflow.

This ensures that:

- Newly created job postings are immediately available for AI-powered matching.
- Updates to existing job postings are reflected in the Vector Index without manual intervention.
- Removed or inactive job postings are no longer considered during candidate evaluation.
- AI Agents always retrieve the most recent and accurate job data while performing semantic search and ATS evaluation.

This automated synchronization eliminates the need for manual index maintenance and ensures TalentFlowAI always uses the latest recruitment data.

---

# 📦 Solutions

## TalentFlowAI

The primary recruitment orchestration workflow responsible for:

- Resume Processing
- Candidate Management
- Job Matching
- ATS Evaluation
- AI Decision Making
- Human Approvals
- Interview Scheduling
- HR Verification

---

## Sync_Job_Vectors_Robot

Keeps the AI Vector Index synchronized with the latest Job Posting data.

Responsibilities include:

- Exporting Job Postings
- Creating CSV Files
- Uploading to Storage Bucket
- Updating the AI Vector Index

---

# 🎯 Future Enhancements

Planned enhancements include:

- LinkedIn Integration
- Naukri Integration
- AI Candidate Ranking Dashboard
- AI Interview Analysis
- Offer Letter Generation
- Background Verification
- Employee Onboarding
- IT Asset Provisioning
- Day-One Automation

---

# 🛠 Built With

- UiPath Maestro
- UiPath Agent Builder
- UiPath Studio
- UiPath Actions
- UiPath Data Service
- UiPath Integration Service
- UiPath Orchestrator
- UiPath GenAI Activities
- Gmail
- Calendly
- Large Language Models (LLMs)

---

# 🙏 Acknowledgements

TalentFlowAI was built as part of the **UiPath AgentHack**, demonstrating how AI Agents, semantic search, intelligent orchestration, and human collaboration can transform enterprise recruitment into a faster, smarter, and more candidate-centric experience.

---

# ❤️ TalentFlowAI

## **Because Great Talent Should Never Be Lost.**
