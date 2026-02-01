# Monitoring & Observability

Tools for metrics collection, logging, tracing, data drift detection and LLM-specific observability in production AI systems.

Focus here is on tools that provide **actionable insights** – not just dashboards, but with alerting, drift detection, and integration into CI/CD or governance workflows.

---

- **Arize Phoenix** – Open-source observability for embeddings, LLMs and RAG pipelines (tracing, eval, drift). Jupyter-first but production scalable.  
  [GitHub](https://github.com/Arize-ai/phoenix) [Docs](https://docs.arize.com/phoenix/)  
  `language:Python` `deploy:library,k8s` `focus:llm,rag` `maturity:growing`

- **Evidently AI** – Monitoring dashboards for data drift, target drift, model performance and regression analysis. Jupyter and API friendly.  
  [GitHub](https://github.com/evidentlyai/evidently) [Docs](https://docs.evidentlyai.com/)  
  `language:Python` `deploy:library,cli` `focus:ml` `maturity:growing`

- **Grafana** – Visualisation and dashboarding for Prometheus, Loki (logs), Tempo (traces). Rich plugin ecosystem including ML metrics.  
  [GitHub](https://github.com/grafana/grafana) [Docs](https://grafana.com/docs/)  
  `language:Go,TypeScript` `deploy:k8s,docker` `focus:infra,ml` `maturity:enterprise`

- **OpenTelemetry** – Vendor-neutral standard and SDKs for distributed traces, metrics and logs. Essential for observability in microservices and AI pipelines.  
  [GitHub](https://github.com/open-telemetry/opentelemetry-collector) [Docs](https://opentelemetry.io/docs/)  
  `language:Polyglot` `deploy:k8s,library` `focus:infra` `maturity:established`

- **Prometheus** – Time-series metrics collection and querying, the de facto standard for infra and service monitoring. Pairs with Grafana and Alertmanager.  
  [GitHub](https://github.com/prometheus/prometheus) [Docs](https://prometheus.io/docs/)  
  `language:Go` `deploy:k8s,docker` `focus:infra` `maturity:enterprise`

- **TruLens** – Evaluation and observability framework for LLM apps with feedback functions, instrumentation and experiment tracking.  
  [GitHub](https://github.com/truera/trulens) [Docs](https://www.trulens.org/)  
  `language:Python` `deploy:library` `focus:llm,agents` `maturity:early`

- **LangFuse** – Open source LLM observability and engineering platform for tracing, evaluations, prompt management, metrics and experiment tracking across LLM apps and agents.  
  [GitHub](https://github.com/langfuse/langfuse) [Docs](https://langfuse.com/docs)
  `language:Python,TypeScript` `deploy:sdk,hosted` `focus:llm,observability,evals` `maturity:enterprise`

---

**Notes:**  
- Infra tools (Prometheus stack, OpenTelemetry) are foundational – most ML/LLM tools build on them.  
- For LLM-specific observability, tools like Phoenix and TruLens bridge evaluation and production monitoring.  
- Missing something? Open a PR with tags and evidence of adoption.
