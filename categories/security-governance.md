# Security, Policy & Governance

Policy engines, authorisation services and AI‑specific security tools for access control, prompt protection and compliance.

Focus on **infrastructure‑level controls** – policy‑as‑code, fine‑grained auth, auditability and LLM‑safe defaults.

---

- **Cedar** – Open‑source policy language and agent implementations that can be used for fine‑grained ABAC around LLM endpoints and vector DBs.
  [GitHub](https://github.com/cedar-policy/cedar) [Docs](https://docs.cedarpolicy.com/)
  `language:Rust,Go` `deploy:library,sidecar` `focus:policy-as-code,authorisation` `maturity:cloud-proven`

- **LLM Guard** – Comprehensive security scanner for LLM inputs/outputs: toxicity, PII detection, prompt injection, jailbreaks.  
  [GitHub](https://github.com/protectai/llm-guard) [Docs](https://protectai.github.io/llm-guard/#getting-started)  
  `language:Python` `deploy:library` `focus:llm,security` `maturity:growing`

- **NeMo GuardRAILS** – Programmable guardrails layer between app and LLM, with input/output rails for jailbreak detection, topic control, content safety, and hallucination/self‑check flows.  
  [GitHub](https://github.com/NVIDIA/NeMo-Guardrails) [Docs](https://docs.nvidia.com/nemo/guardrails/latest/index.html)
  `language:Python` `deploy:library,service` `focus:llm,guardrails,security` `maturity:enterprise`

- **OpenFGA** – Zanzibar‑inspired fine‑grained authorisation for relationships ("user X edits document Y"). Scalable tuple store.  
  [GitHub](https://github.com/openfga/openfga) [Docs](https://openfga.dev/docs)  
  `language:Go` `deploy:k8s,docker` `focus:governance,security` `maturity:enterprise`

- **Open Policy Agent (OPA)** – General‑purpose policy engine using Rego. Kubernetes admission, API gateways, data filters.  
  [GitHub](https://github.com/open-policy-agent/opa) [Docs](https://www.openpolicyagent.org/docs/latest/)  
  `language:Go` `deploy:k8s,sidecar` `focus:governance,security` `maturity:enterprise`

- **Purple Llama** – Open‑source guardrail framework acting as a final security layer for agents.  
  [GitHub](https://github.com/meta-llama/PurpleLlama) [Docs](https://meta-llama.github.io/PurpleLlama/LlamaFirewall/)
  `language:Python` `deploy:library,service` `focus:llm,agents,,security` `maturity:research`

---

**Notes:**  
- **OPA/OpenFGA** for infrastructure/app authorisation (complementary: relationships + policy logic).  
- Protect AI, NeMo Guardrails also relevant for model scanning/runtime.  
- Missing something? Open a PR with tags and evidence of adoption.
