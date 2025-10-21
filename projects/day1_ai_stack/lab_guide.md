# Day 1 Lab Guide — Build Your First AI System Blueprint

Goal: Design a production-ready AI system architecture (like a ChatGPT-style app).
Time: ~60 minutes
Deliverables: one .drawio diagram (editable), one .png (exported), and a short README.

------------------------------------------------------------
1) Learn (10–15 min)
Read two quick intros (skim is fine):
- The Modern LLM Stack (LangChain blog)
- How ChatGPT Actually Works (AssemblyAI blog)
Understand the 6 layers: Data → Embedding → Retrieval → LLM/Reasoning → Serving → Monitoring

------------------------------------------------------------
2) Design the diagram (15–20 min)
a) Open https://app.diagrams.net (diagrams.net)
b) Create 6 boxes labeled:
   - Data Ingestion (PDFs / TXT / APIs)
   - Embedding Service (OpenAI or sentence-transformers)
   - Vector DB (Chroma / FAISS / PGVector)
   - LLM Reasoning (GPT-4o-mini / Claude / Llama 3)
   - Serving Layer (FastAPI / Streamlit)
   - Monitoring (LangSmith / TruLens)
c) Connect them left→right in that order.
d) File → Save As → Device → save as: architecture_day1.drawio
   Location: ~/AIChampion/projects/day1_ai_stack
e) File → Export As → PNG → save as: architecture_day1.png
   Same folder.

------------------------------------------------------------
3) Document (10–15 min)
Open README.md in this folder and write:
- A table listing each layer, the tool you chose, and why.
- 2–3 trade-offs (e.g., vendor lock-in, latency vs quality, cost vs context).
- Next step: “Tomorrow I’ll run a Transformer locally.”

------------------------------------------------------------
4) Commit to GitHub (2–3 min)
From project root (~/AIChampion):
  git add .
  git commit -m "Day 1: AI stack architecture diagram + README"
  git push

------------------------------------------------------------
5) Reflect (2–3 min)
Edit ~/AIChampion/notes/day1.md and add 2–3 bullets:
- What clicked for you?
- One trade-off you’d revisit later.
- What you’ll do first on Day 2.

