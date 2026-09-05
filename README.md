<!-- Header -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0ea5e9,100:a855f7&height=120&section=header&animation=twinkling" alt="" />
</p>

<h1 align="center">Hi 👋 — I'm <strong>Dhanush G</strong></h1>

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=JetBrains+Mono&weight=600&size=26&duration=2600&pause=1000&color=38BDF8&center=true&vCenter=true&width=560&lines=AI+Engineer;Production+GenAI+Systems;LLM+Fine-Tuning+%C2%B7+Agentic+RAG+%C2%B7+MLOps" alt="AI Engineer · Production GenAI · LLM Fine-Tuning · Agentic RAG · MLOps" />
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/d0801" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="mailto:dhanushgd0801@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-Contact-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail" />
  </a>
  <a href="https://github.com/DhanushGD/Portfolio" target="_blank">
    <img src="https://img.shields.io/badge/Portfolio-View-a855f7?style=for-the-badge&logo=githubpages&logoColor=white" alt="Portfolio" />
  </a>
</p>

<p align="center"><sub>✦ ✧ ✦</sub></p>

## 🌟 About Me

AI Engineer at **Automation Anywhere** (2.5+ yrs), where I own the support-AI stack end to end: a multi-tenant **Vespa**-backed enterprise search platform, a **Hybrid Agentic RAG** layer on top of it, and an in-house **fine-tuned LLM on AWS SageMaker** with a drift-triggered self-healing retraining loop. It's used daily by 25+ support engineers and embedded by external customers over 150K+ documents.

I care about the parts that make AI trustworthy in production — grounding, evaluation, drift monitoring, and human-in-the-loop safety. My open-source work pushes the same themes: LLM alignment (DAPT → SFT → DPO), agent interoperability (MCP / A2A), and closed-loop MLOps.

### 📈 Things I've shipped at work

| Area | What | Result |
|---|---|---|
| 🔎 Enterprise Search | Multi-tenant Vespa hybrid search (BM25 + vector) with pluggable ETL from Salesforce, Jira, Fluid Topics & web crawl | **+22% NDCG@10**, replaced a licensed third-party tool |
| 🤖 Agentic RAG | LangGraph + MCP retrieval / reasoning / validation agents with HITL guardrails | **−60% hallucinations** (RAGAS), latency **8s → 3.2s** |
| 🧪 LLM Evaluation | CI-gated RAGAS + LangSmith eval pipeline on every release | **−75%** eval turnaround |
| 🧠 Fine-tuned LLM | TinyLlama QLoRA (Unsloth) on 100K+ resolved-case dataset, served on SageMaker | **83% → 87%** golden-set accuracy, **−70%** inference cost |
| 🔁 Self-healing MLOps | Evidently drift triggers → retrain → golden-set gate → blue/green deploy → auto-rollback | Retrain-to-deploy **~2 days → ~4 hours**, unattended |

<p align="center"><sub>✦ ✧ ✦</sub></p>

## 🚀 Featured Projects

> The ones that best show how I think. Each has a full README with architecture, eval results, and how to run it.

| Project | What it is | Stack |
|---|---|---|
| 🦙 **[BioLLama-R](https://github.com/DhanushGD/BioLLama-R)** | Full three-stage LLM alignment pipeline for healthcare — **DAPT → SFT → RLHF (DPO)** — with the aligned model wired into a Groq-powered agentic pipeline for patient intake, clinical reasoning, and safety validation | Unsloth · TRL · Hugging Face · Groq · LangGraph |
| 🔗 **[InterAgentX 4](https://github.com/DhanushGD/InterAgentX-4)** | Cross-language multi-agent system — three Python agents (RAG Analyst, Web Researcher, Evidence Verifier) and a JavaScript Summarizer collaborating over **A2A (JSON-RPC streaming)** with a shared **MCP** tool layer consumed identically from both runtimes | A2A · MCP · LlamaIndex · ChromaDB · Streamlit |
| 🛡️ **[AegisML](https://github.com/DhanushGD/AegisML)** | Self-healing production MLOps for content moderation — fine-tuned multi-label DistilBERT with **Evidently drift detection → Ollama-assisted HITL re-labeling → DVC lineage → Great Expectations gate → zero-downtime CI/CD** | DistilBERT · FastAPI · Evidently · DVC · GitHub Actions |
| 🤖 **[SupportSage](https://github.com/DhanushGD/SupportSage)** | TinyLlama fine-tuned on support tickets with **LoRA/QLoRA**, W&B tracking, and SageMaker deployment via S3 — the open-source sibling of my production fine-tuning pipeline | Unsloth · W&B · SageMaker |
| 🏦 **[RiskGraph AI](https://github.com/DhanushGD/RiskGraph-AI)** | Autonomous credit-model auditor — XGBoost + SHAP explanations fed into a LangGraph agent over a Neo4j **GraphRAG** knowledge base | XGBoost · SHAP · LangGraph · Neo4j · Ollama |
| 🩺 **[Medical-RAG](https://github.com/DhanushGD/Medical-RAG)** | Domain-specific **embedding fine-tuning** for hallucination reduction in medical retrieval, benchmarked against base embeddings with RAGAS | Sentence-Transformers · RAGAS · FAISS |

<details>
<summary><b>🧪 More fine-tuning & alignment experiments</b></summary>
<br>

- 🎯 **LlamaRefine** — Aligning TinyLlama via SFT + DPO
- 🧩 **RLHF-PPO** — Fine-tuning with Proximal Policy Optimization
- 🔍 **Gemma-3n Fine-Tuning**
- 🩺 **LLM Doctor** — TinyLlama fine-tuned on MedQuAD with Ollama integration
- 🦙 **BioLLama** — DAPT → SFT for healthcare LLMs (predecessor to BioLLama-R)

</details>

<details>
<summary><b>🤖 More agents & RAG</b></summary>
<br>

- 🧠 **SupportMind** — Stateful multi-agent IT support on a LoRA/QLoRA fine-tuned model
- 🤝 **InterAgentX** — RAG + CrewAI + MCP + ADK-compatible A2A agent
- 📊 **ChartInsight AI** — Multi-agent chart analyzer with Azure OCR + LangGraph
- 🔍 **AI IT Assistant** — Hybrid-search RAG + multi-agent system with CrewAI
- 📄 [Conversational RAG for PDFs](https://github.com/DhanushGD/Conversational-RAG-System-for-PDF-Documents-) — PDF upload + chat history
- 🤖 [GenAI Code Review Bot](https://github.com/DhanushGD/Generative-AI-Code-Review-and-Assistance-Bot)
- 🐞 [Jira Bug Status Prediction & Recommendation](https://github.com/DhanushGD/Jira-Bug-Status-Prediction-and-Recommendation-System)
- 📧 [Cold Email Generator](https://github.com/DhanushGD/Cold-Email-Generator) 
- 🌍 [AI Translation App](https://github.com/DhanushGD/AI-translation-app) 
- 🌐 [Serverless Blog Generator (LLaMA 3 on AWS)](https://github.com/DhanushGD/BLOG-GENERATOR)

</details>

<details>
<summary><b>📚 Classic ML / DL foundations</b></summary>
<br>

- 🔮 [Next-word prediction — LSTM/GRU](https://github.com/DhanushGD/Next_word_prediction_using_LSTM-GRU)
- 🧠 [RNN sentiment analysis](https://github.com/DhanushGD/RNN---Sentiment-Analysis)
- ⚡ [Customer churn — ANN](https://github.com/DhanushGD/ANN-CLASSIFICATION-CHURN)
- 🩺 [Breast cancer prediction](https://github.com/DhanushGD/Breast-cancer-prediction)
- ✍️ [Full-stack blogging platform](https://github.com/DhanushGD/BLOGGING-PLATFORM)

</details>

<p align="center"><sub>✦ ✧ ✦</sub></p>

## 🛠️ Tech I work with

**LLMs & Agents** — LangChain · LangGraph · LlamaIndex · CrewAI · MCP · A2A · Hugging Face · Unsloth · Guardrails / HITL

**Fine-Tuning & Eval** — SFT · LoRA/QLoRA · DAPT · RLHF (PPO/DPO) · Embedding fine-tuning · RAGAS · LangSmith · W&B

**Search & RAG** — Vespa AI (hybrid BM25 + vector) · FAISS · ChromaDB · Neo4j / GraphRAG

**MLOps & Infra** — AWS SageMaker (Training Jobs, Model Registry, Endpoints) · S3 · EC2 · Docker · FastAPI · GitHub Actions · DVC · Great Expectations · Evidently AI · MongoDB

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" />
  <img src="https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black" />
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white" />
  <img src="https://img.shields.io/badge/LangGraph-FF6F61?style=flat-square" />
  <img src="https://img.shields.io/badge/Unsloth-00A67E?style=flat-square" />
  <img src="https://img.shields.io/badge/RAGAS-6E56CF?style=flat-square" />
  <img src="https://img.shields.io/badge/Vespa-1A73E8?style=flat-square" />
  <img src="https://img.shields.io/badge/AWS%20SageMaker-232F3E?style=flat-square&logo=amazonaws&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/Neo4j-4581C3?style=flat-square&logo=neo4j&logoColor=white" />
</p>

<p align="center"><sub>✦ ✧ ✦</sub></p>

  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=DhanushGD&layout=compact&theme=tokyonight&hide_border=true" height="165" alt="Top languages" />
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:a855f7,100:0ea5e9&height=100&section=footer&animation=twinkling" alt="" />
</p>

<p align="center"><strong>⭐ Open to collaborating on RAG evaluation, LLM alignment, and agent interoperability — reach out!</strong></p>
