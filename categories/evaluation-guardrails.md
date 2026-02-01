# Evaluation, Testing & Guardrails

Frameworks for automated testing, evaluation metrics, and runtime guardrails for ML models and LLM applications.

Focus on **quantifiable quality** – LLM-as-judge metrics, RAG evaluation, bias detection, output validation and safety guardrails.

---

- **Deepchecks** – Comprehensive validation for ML/LLM pipelines: data integrity, model performance, bias, drift. Modular and production-ready.  
  [GitHub](https://github.com/deepchecks/deepchecks) [Docs](https://docs.deepchecks.com/)  
  `language:Python` `deploy:library,cli` `focus:ml,llm` `maturity:established`

- **DeepEval** – Pytest-like framework for LLM testing with 30+ metrics (RAG, hallucination, consistency). Unit tests for prompts and chains.  
  [GitHub](https://github.com/confident-ai/deepeval) [Docs](https://deepeval.com/docs/getting-started)  
  `language:Python` `deploy:library` `focus:llm,rag` `maturity:growing`

- **Guardrails AI** – Runtime output validation using Pydantic schemas, RAIL specs and retry logic. Ensures structured, safe LLM responses.  
  [GitHub](https://github.com/guardrails-ai/guardrails) [Docs](https://www.guardrailsai.com/docs)  
  `language:Python` `deploy:library` `focus:llm,guardrails` `maturity:growing`

- **LM Evaluation Harness** – Standardised few-shot evaluation framework for language models. Powers Open LLM Leaderboard, 200+ benchmarks.  
  [GitHub](https://github.com/EleutherAI/lm-evaluation-harness) [Docs](https://github.com/EleutherAI/lm-evaluation-harness#usage)  
  `language:Python` `deploy:cli` `focus:llm` `maturity:established`

- **MLflow LLM Evaluate** – Built-in LLM evaluation module for RAG, QA and custom metrics. Integrates with MLflow tracking.  
  [GitHub](https://github.com/mlflow/mlflow) [Docs](https://mlflow.org/docs/latest/llms/llm-evaluate/)  
  `language:Python` `deploy:library` `focus:llm,rag` `maturity:established`

- **Ragas** – Framework for RAG pipeline evaluation: faithfulness, context precision, answer relevance. LLM-as-judge metrics.  
  [GitHub](https://github.com/explodinggradients/ragas) [Docs](https://docs.ragas.io/en/stable/)  
  `language:Python` `deploy:library` `focus:llm,rag` `maturity:growing`

---

**Notes:**  
- **Ragas + DeepEval** dominate RAG/agent testing; **Guardrails** for production output safety.  
- **LM Harness** for academic/research benchmarks; **MLflow** if already in MLflow ecosystem.  
- Missing something? Open a PR with tags and evidence of adoption.
