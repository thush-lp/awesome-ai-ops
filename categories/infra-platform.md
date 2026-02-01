# Platforms & End-to-End Stacks

Opinionated, integrated platforms combining orchestration, tracking, serving and monitoring for complete ML/LLM workflows.

Focus on **batteries-included** solutions that reduce tool sprawl while remaining extensible and Kubernetes-native.

---

- **ClearML** – End-to-end MLOps: experiment tracking, orchestration, datasets, hyperparam sweeps and serving. Self-hosted with strong automation.  
  [GitHub](https://github.com/allegroai/clearml) [Docs](https://clear.ml/docs/latest/docs/)  
  `language:Python` `deploy:k8s,self-hosted` `focus:ml` `maturity:enterprise`

- **Flyte** – Kubernetes-native workflow engine for data/ML pipelines. Strong typing, versioning, caching and massive scale (used by Lyft/Spotify).  
  [GitHub](https://github.com/flyteorg/flyte) [Docs](https://docs.flyte.org/)  
  `language:Python,Go` `deploy:k8s` `focus:ml,data` `maturity:enterprise`

- **Kubeflow** – Machine learning toolkit for Kubernetes: pipelines, training ops (TFJob), serving (KServe), notebooks and metadata. CNCF project.  
  [GitHub](https://github.com/kubeflow/kubeflow) [Docs](https://www.kubeflow.org/docs/)  
  `language:Python,Go` `deploy:k8s` `focus:ml` `maturity:enterprise`

- **MLRun** – Open-source MLOps orchestration for data/feature pipelines, training, serving and real-time inference. Kubeflow/Iguazio roots.  
  [GitHub](https://github.com/mlrun/mlrun) [Docs](https://docs.mlrun.org/)  
  `language:Python` `deploy:k8s` `focus:ml,llm` `maturity:growing`

- **ZenML** – Extensible MLOps framework for reproducible pipelines. Integrates Kubeflow, MLflow, BentoML across infra (cloud/K8s/local).  
  [GitHub](https://github.com/zenml-io/zenml) [Docs](https://docs.zenml.io/)  
  `language:Python` `deploy:k8s,cloud` `focus:ml` `maturity:growing`

---

**Notes:**  
- **Kubeflow** for Kubernetes‑centric teams; **Flyte** for workflow‑heavy data/ML pipelines.  
- **ClearML/MLRun** closer to "enterprise platform" feel with UI/automation. **ZenML** excels at portability.  
- Point solutions (Kedro, Argo) belong in orchestration category.  
- Missing something? Open a PR with tags and evidence of adoption.
