**AI Resume Auditor & ATS Optimizer (n8n + Gemini)**

**📋 Project Overview**

This project is an automated AI-driven "Agent" built using n8n that audits resumes. It doesn't just look for keywords; it uses Google Gemini 1.5 Flash to perform a semantic analysis of a candidate's experience against modern recruitment standards.

**🛠️ The Tech Stack**

Workflow Orchestration: n8n (Self-hosted/Cloud)

AI Engine: Google Gemini 2.5 Flash (via API)

Data Extraction: PDF Parser (n8n Binary Tool)

Trigger: [e.g., Webhook / Google Drive / Email]

Notification: [e.g., Gmail / Slack / Discord]

**🧠 Logic & Workflow Architecture**

The system follows a 4-stage "Agentic" workflow:

Ingestion: A PDF resume is uploaded/received via the trigger node.

Extraction: n8n converts the binary PDF data into clean text strings.

Analysis (The Brain): The text is sent to Gemini with a multi-step prompt:

Step A: Identify core skills and years of experience.

Step B: Compare against industry-standard ATS (Applicant Tracking System) benchmarks.

Step C: Generate a "SWOT" analysis (Strengths, Weaknesses, Opportunities, Threats).

Delivery: The final audit is formatted into a readable report and sent automatically to the user.

**📂 How to Use**

Blueprint: The resume_auditor_workflow.json file contains the exported n8n workflow.

Setup: Import the JSON into your n8n instance, add your Gemini API key, and activate the nodes.

Created as part of my GenAI & Automation Mentorship (December 2025)
