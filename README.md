# AI Agents Portfolio (n8n)

> A collection of production-style AI agents built with n8n, showcasing agentic thinking, real integrations, human-in-the-loop workflows, and system-level reasoning.

---

## 📌 Overview

This repository contains **real-world AI agents**, not prompt demos.

Each agent is designed to demonstrate how **AI systems actually operate in production** — interacting with tools, managing state, handling human feedback, and executing multi-step workflows reliably.

The focus is on:
- End-to-end automation
- Agentic workflows
- Real integrations
- Deterministic logic + LLM reasoning
- Production-oriented design

---

## 🔹 Agent 1: LinkedIn Post Generator Agent

📁 **`linkedin-post-generator/`**

### What It Does

An AI agent that automates **LinkedIn content creation** with a **human approval loop**.

### Key Capabilities

- Accepts structured input via webhook (topic, audience, email)
- Generates LinkedIn post content using an LLM
- Optionally generates image prompts and images
- Stores generated content and metadata in Google Sheets
- Stores assets in Google Drive
- Sends approval emails (Approve / Reject)
- Regenerates content using human feedback if rejected

### Why It Matters

This agent demonstrates:

- Human-in-the-loop AI design
- Stateful workflows across executions
- Real-world integrations (Email, Sheets, Drive)
- Multi-step agent behavior instead of single prompts

This mirrors how **AI agents are used in marketing and growth automation teams**.

---

## 🔹 Agent 2: Website Analytics – AI Explainer

📁 **`website-analytics-ai-explainer/`**

### What It Does

An AI agent that turns **Google Analytics data** into **plain-English insights**.

### Key Capabilities

- Accepts natural-language questions via webhook
- Fetches current vs previous period data from GA4
- Computes trends and percentage changes
- Explains traffic changes using an LLM
- Returns insights via API response (webhook)

### Why It Matters

Most analytics tools show numbers but don’t explain **why** changes happened.

This agent demonstrates:

- Data-grounded AI reasoning
- Time-window comparison logic
- Deterministic preprocessing + LLM explanation
- Building AI agents that explain, not hallucinate

This reflects real use cases in **analytics, ops, and decision-support systems**.

---

## 🛠 Tech Stack (Across Agents)

- **n8n** — Workflow orchestration
- **LLMs (OpenAI compatible)** — Reasoning & generation
- **Google Analytics 4** — Analytics data source
- **Google Sheets** — Lightweight state storage
- **Google Drive** — Asset storage
- **Email (SMTP / Gmail)** — Approval workflows
- **Webhooks** — API-style triggering

---

## 📂 Repository Structure

```plaintext
.
├── linkedin-post-generator/
│   ├── post-generator.json
│   └── README.md
├── website-analytics-ai-explainer/
│   ├── website-analytics-explainer.json
│   └── README.md
└── README.md
