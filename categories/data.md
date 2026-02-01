# Data, Versioning & Lineage

**Why it matters for AI Ops**: Reproducible training requires immutable data snapshots and full lineage from raw → features → model. Enables rollback, debugging and compliance audits.

Tools for versioning datasets, tracking transformations, data lineage and cataloging in ML pipelines and data lakes.

Focus on **reproducibility** at scale – Git-like semantics for data, lineage across pipelines, and integration with MLOps workflows.

---

- **Delta Lake** – Storage layer adding ACID transactions, time travel and schema enforcement to data lakes (Parquet format).  
  **AI Ops benefit**: Reliable feature store backing with time‑travel for model debugging ("what data fed v1.2?"). Spark/MLflow native.  
  [GitHub](https://github.com/delta-io/delta) [Docs](https://delta.io/)  
  `language:Scala,Python` `deploy:spark` `focus:data` `maturity:enterprise`

- **DVC (Data Version Control)** – Git-like versioning for datasets and models. Tracks large files via pointers and remote storage (S3/GCP).  
  **AI Ops benefit**: `dvc repro` + MLflow integration = reproducible ML experiments across teams. No more "works on my machine".  
  [GitHub](https://github.com/iterative/dvc) [Docs](https://dvc.org/doc)  
  `language:Python` `deploy:cli,library` `focus:data,ml` `maturity:established`

- **lakeFS** – Git for data lakes: zero-copy branching, merge requests and CI/CD for object storage (S3/GCS/Azure). Enterprise-scale versioning.  
  **AI Ops benefit**: Test model retraining on feature branches without duplicating TBs of training data. Production rollback in seconds.  
  [GitHub](https://github.com/treeverse/lakeFS) [Docs](https://docs.lakefs.io/)  
  `language:Go` `deploy:k8s,docker` `focus:data` `maturity:enterprise`

- **Marquez** – OpenLineage metadata server for job/dataset lineage. Tracks pipeline dependencies, runs and impact analysis.  
  **AI Ops benefit**: Impact analysis = "if dataset X changes, which models break?". Essential for production ML governance.  
  [GitHub](https://github.com/MarquezProject/marquez) [Docs](https://marquezproject.ai/docs/quickstart/)  
  `language:Java,Python` `deploy:k8s,docker` `focus:data,lineage` `maturity:growing`

- **OpenLineage** – Standard for collecting lineage metadata across tools (Airflow, dbt, Spark). Integrates with Marquez/Amundsen.  
  **AI Ops benefit**: Unified lineage across Kedro/Airflow/MLflow. Single source of truth for model debugging and audits.  
  [GitHub](https://github.com/OpenLineage/OpenLineage) [Docs](https://openlineage.io/docs/)  
  `language:Polyglot` `deploy:library` `focus:data,lineage` `maturity:established`

---

**Notes:**  
- **lakeFS + DVC** cover most use cases: lakeFS for production lakes, DVC for experiment-scale ML datasets.  
- **OpenLineage + Marquez** for metadata-driven lineage; **Delta Lake** for reliable lakehouse storage.  
- Missing something? Open a PR with tags and evidence of adoption.
