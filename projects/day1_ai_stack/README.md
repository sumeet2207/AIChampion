# Day 1 — Modern AI Stack

## My Architecture (v1)
Data → Embedding → Retrieval → LLM/Reasoning → Serving → Monitoring

| Layer       | Tool I chose                     | Why I chose it                       |
|------------|----------------------------------|--------------------------------------|
| Data       | PDFs + simple web/API ingestion  | Easy to start, realistic inputs      |
| Embedding  | OpenAI text-embedding-3-small    | Robust quality, cheap, fast          |
| Vector DB  | Chroma (local)                   | Simple, open source, no infra setup  |
| LLM        | GPT-4o-mini                      | Good quality/cost balance            |
| Serving    | FastAPI                          | Lightweight Python microservice      |
| Monitoring | LangSmith (or TruLens)           | Tracing, evals, token/cost tracking  |

### Trade-offs
- Some vendor lock-in (OpenAI embeddings/LLM)
- Latency vs quality: larger models cost more and respond slower
- Context vs cost: long contexts increase token spend

### Next
- Day 2: run a Transformer locally and visualize attention

