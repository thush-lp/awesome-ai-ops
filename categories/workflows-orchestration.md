# Pipelines & Orchestration

Workflow engines and pipeline frameworks for data engineering, ML training and LLM processing.

Focus on **declarative, scalable** orchestration with Kubernetes support, caching, retries and lineage integration.

---

- **Argo Workflows** – Kubernetes-native container-native workflows. Dynamic DAGs, loops, conditionals, artifact passing. CNCF graduated.  
  [GitHub](https://github.com/argoproj/argo-workflows) [Docs](https://argo-workflows.readthedocs.io/)  
  `language:Go,YAML` `deploy:k8s` `focus:data,ml` `maturity:enterprise`

- **Kedro** – Framework for reproducible ML pipelines with data catalog, modularity and best practices. Pipeline templating.  
  [GitHub](https://github.com/kedro-org/kedro) [Docs](https://kedro.org/)  
  `language:Python` `deploy:library,cli` `focus:ml,data` `maturity:established`

- **Kubeflow Pipelines** – ML-focused workflow SDK on Kubernetes. Component reuse, versioning, caching, UI scheduling.  
  [GitHub](https://github.com/kubeflow/pipelines) [Docs](https://www.kubeflow.org/docs/components/pipelines/)  
  `language:Python` `deploy:k8s` `focus:ml` `maturity:enterprise`

- **Metaflow** – Human‑centric data science workflows from Netflix. Versioning, branching, AWS integration.  
  [GitHub](https://github.com/Netflix/metaflow) [Docs](https://docs.metaflow.org/)  
  `language:Python` `deploy:cloud,aws` `focus:ml,data` `maturity:established`

---

**Notes:**  
- **Argo** for general container orchestration; **Kubeflow Pipelines** for ML‑specific.  
- **Kedro** excels at project structure/reproducibility; **Metaflow** for data scientist productivity.  
- Flyte/MLRun belong in platforms category (full‑stack).  
- Missing something? Open a PR with tags and evidence of adoption.
