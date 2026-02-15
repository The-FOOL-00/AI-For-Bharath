# 🧭 Judge's Evaluation Guide: Flashbook AI

Welcome to the **Flashbook AI** repository. To help you evaluate our "AI for Bharat" submission efficiently, we have mapped our repository structure directly to the judging criteria.

---

## 1. 📋 Documentation & Requirements (Mandatory)
* **Product Requirements (PRD):** [`requirements.md`](./requirements.md)
    * *Look for:* **Requirement 3** (AI Content Gen) and **Requirement 5** (Redis Caching) for technical depth.
    * *Look for:* **"Future Roadmap"** at the bottom for our **multilingual "Digital Bharat" strategy**.
* **System Design:** [`design.md`](./design.md)
    * *Look for:* The **Serverless Architecture** breakdown and **Data Flow** specifics.

## 2. 🏗️ Architecture & Scalability
* **Visual Diagram:** [`diagram-export-15-2-2026-9_25_23-pm.jpg`](./diagram-export-15-2-2026-9_25_23-pm.jpg)
    * *Highlight:* We use a **Microservices** approach (4 distinct Lambdas) rather than a monolith.
    * *Highlight:* **Amazon ElastiCache (Redis)** is implemented to reduce AI costs and latency (<200ms).
    * *Highlight:* **EventBridge & Athena** pipeline included for future analytics.

## 3. 🎨 User Interface (Visuals)
* **Wireframes & Mockups:** See the **`docs/`** folder (or scroll to the bottom of the README).
* **Key Flows:**
    1.  **Onboarding:** Vertical scrolling education concept.
    2.  **Reel Reader:** The core "Instagram-like" interface for books.
    3.  **Smart Notes:** The bottom-sheet annotation tool.

## 4. 🤖 AI & Innovation
* **Models Used:**
    * **Text:** Claude 3.5 Sonnet (via Amazon Bedrock) for summarization.
    * **Images:** Amazon Titan Image Generator for educational illustrations.
* **Code Location:**
    * Backend logic is located in `backend/src/handlers/`.
    * AI Prompt Engineering logic can be found in `backend/src/utils/prompts.py`.

## 5. 🔍 Proof of Process (The `.kiro` Folder)
* **Path:** [`.kiro/`](./.kiro/)
* **What is this?** This folder contains the raw architectural specs and context used by our AI Architect agent. It serves as **traceability** for our design process, proving that our architecture was systematically generated and refined using modern AI-first workflows, rather than being an afterthought.

---

## 🚀 Quick Impact Statement
Flashbook AI solves the "Attention Span Crisis" in education. By converting dense PDF textbooks into vertical, interactive "Knowledge Reels," we make technical education accessible to the mobile-first generation in Tier 2/3 cities.
