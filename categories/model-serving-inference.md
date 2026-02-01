# Model Serving & Inference

Production model serving platforms for classical ML and LLMs – autoscaling, traffic splitting, explainability and multi-model support.

Focus on **Kubernetes-native** solutions with A/B testing, canaries, and monitoring integration.

---

- **BentoML** – Framework for serving, managing and deploying ML models. Containerisation, autoscaling, multi-framework support.  
  [GitHub](https://github.com/bentoml/BentoML) [Docs](https://docs.bentoml.com/en/latest/)  
  `language:Python` `deploy:k8s,docker` `focus:ml,llm` `maturity:established`

- **Cog** – Simple containerisation for ML models: YAML config → Docker image → deploy anywhere. Inference endpoints auto-generated.  
  [GitHub](https://github.com/replicate/cog) [Docs](https://cog.run/)  
  `language:Python` `deploy:docker` `focus:ml,llm` `maturity:growing`

- **KServe** (formerly KFServing) – Standardised, Kubernetes-native inference on K8s. Autoscaling, explainability, traffic splitting.  
  [GitHub](https://github.com/kserve/kserve) [Docs](https://kserve.github.io/website/)  
  `language:Python` `deploy:k8s` `focus:ml` `maturity:enterprise`

- **Seldon Core** – ML inference platform on Kubernetes: A/B testing, canaries, multi-armed bandits, outlier detection.  
  [GitHub](https://github.com/SeldonIO/seldon-core) [Docs](https://docs.seldon.io/)  
  `language:Python,Go` `deploy:k8s` `focus:ml` `maturity:enterprise`

- **vLLM** – High-throughput LLM serving engine with PagedAttention, continuous batching and OpenAI‑compatible API.  
  [GitHub](https://github.com/vllm-project/vllm) [Docs](https://docs.vllm.ai/)  
  `language:Python,CUDA` `deploy:k8s,docker` `focus:llm` `maturity:enterprise`

---

**Notes:**  
- **KServe/Seldon** for Kubernetes ML serving; **vLLM/BentoML** excel at LLM scale/performance.  
- **Cog** perfect for quick model packaging → production.  
- Triton Inference Server also strong (NVIDIA‑focused).  
- Missing something? Open a PR with tags and evidence of adoption.
