# Experiment Tracking & Metadata

Tools for logging parameters, metrics, artifacts, and metadata during ML/LLM experiments. Enables comparison, reproducibility and collaboration.

Focus on **scalability and integration** – supports large‑scale runs, UI for exploration, and hooks into pipelines/orchestration.

---

- **Aim** – Performant, self‑hosted experiment tracker with rich UI for metrics, histograms, images and hyperparams. Handles 10k+ runs efficiently.  
  [GitHub](https://github.com/aimhubio/aim) [Docs](https://aimstack.readthedocs.io/)  
  `language:Python` `deploy:k8s,docker,cli` `focus:ml,llm` `maturity:growing`

- **ClearML** – Full experiment management: auto‑logging, datasets, orchestration, hyperparam sweeps. Strong UI and agent orchestration.  
  [GitHub](https://github.com/allegroai/clearml) [Docs](https://clear.ml/docs/latest/docs/)  
  `language:Python` `deploy:k8s,self-hosted` `focus:ml` `maturity:established`

- **MLflow** – Open source platform for experiment tracking, model registry and reproducibility. Auto‑logging for major frameworks, flexible backend.  
  [GitHub](https://github.com/mlflow/mlflow) [Docs](https://mlflow.org/docs/latest/tracking.html)  
  `language:Python,R` `deploy:self-hosted,library` `focus:ml,llm` `maturity:enterprise`

- **Sacred** – Configurable experiment management with MongoDB backend. Tracks sources, configs, metrics. Pairs with Omniboard UI.  
  [GitHub](https://github.com/IDSIA/sacred) [Docs](https://sacred.readthedocs.io/)  
  `language:Python` `deploy:library` `focus:ml` `maturity:established`

---

**Notes:**  
- **MLflow** dominates due to ecosystem and model registry integration.  
- **Aim** excels for UI/visualisation at scale; **ClearML** for end‑to‑end automation.  
- Weights & Biases, Neptune are popular hosted alternatives (not listed).  
- Missing something? Open a PR with tags and evidence of adoption.
