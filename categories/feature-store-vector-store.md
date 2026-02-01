# Feature & Vector Stores

Online/offline feature stores for ML serving and vector databases/embeddings stores for semantic search and RAG.

Focus on **production scale** – low‑latency serving, consistency guarantees, TTL/eviction and hybrid search (vector + metadata).

---

- **Feast** – Open‑source feature store with online/offline consistency. Batch/streaming ingestion, Redis/DynamoDB online stores.  
  [GitHub](https://github.com/feast-dev/feast) [Docs](https://docs.feast.dev/)  
  `language:Python,Java` `deploy:k8s,self-hosted` `focus:ml` `maturity:enterprise`

- **pgvector** – PostgreSQL extension for vector similarity search (HNSW/IVFFlat indexes). Leverage existing Postgres infra.  
  [GitHub](https://github.com/pgvector/pgvector) [Docs](https://github.com/pgvector/pgvector)  
  `language:C` `deploy:postgres` `focus:vector` `maturity:established`

- **Qdrant** – Vector database with advanced filtering, payload search and recommendation APIs. Rust‑based, high performance.  
  [GitHub](https://github.com/qdrant/qdrant) [Docs](https://qdrant.tech/documentation/)  
  `language:Rust` `deploy:k8s,docker` `focus:vector,rag` `maturity:enterprise`

- **Redis** – In‑memory store with vector search (RediSearch module). Sub‑ms latency, ideal for real‑time features/embeddings.  
  [GitHub](https://github.com/redis/redis) [Docs](https://redis.io/docs/latest/)  
  `language:C` `deploy:k8s,docker` `focus:vector,features` `maturity:enterprise`

---

**Notes:**  
- **Feast** for classical ML features; **Qdrant/pgvector** for embeddings/RAG.  
- **Redis** bridges both worlds with ultra‑low latency caching + vectors.  
- Tecton/Hopsworks are popular but not fully OSS (enterprise platforms).  
- Missing something? Open a PR with tags and evidence of adoption.
