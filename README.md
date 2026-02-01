[![Stars](https://img.shields.io/github/stars/thush-lp/awesome-ai-ops?style=social)](https://github.com/thush-lp/awesome-ai-ops/stargazers/)

# Awesome AI Ops (MLOps, LLMOps, Observability & Governance)

A curated, opinionated list of the **best** open-source tools for running AI systems in production – from data and training pipelines to LLM orchestration, observability and governance.

The goal is to help practitioners discover high-quality, actively maintained OSS projects that can form the backbone of a modern AI platform.

> **Bias**: Kubernetes-friendly, cloud-portable tools with strong documentation and governance features (auditability, RBAC, transparency).

---

## Categories

Each category has its own file under `categories/` with tool descriptions, GitHub links, and metadata tags.

- [Data, Versioning & Lineage](categories/data.md)  
- [Experiment Tracking & Metadata](categories/experiment-tracking.md)  
- [Pipelines & Orchestration](categories/workflows-orchestration.md)  
- [Model Serving & Inference](categories/model-serving-inference.md)  
- [Feature & Vector Stores](categories/feature-store-vector-store.md)  
- [Monitoring & Observability](categories/monitoring-observability.md)  
- [Evaluation, Testing & Guardrails](categories/evaluation-guardrails.md)  
- [LLM Frameworks, RAG & Agents](categories/llm-frameworks-agents.md)  
- [Security, Policy & Governance](categories/security-governance.md)  
- [Platforms & End-to-End Stacks](categories/infra-platform.md)  

---

## Selection Criteria

Tools must meet most of these standards:

- ✅ Open source licence suitable for commercial use  
- ✅ Active maintenance (commits/releases last 12-18 months)  
- ✅ Proven adoption (500+ GitHub stars OR production usage)  
- ✅ Excellent documentation and onboarding  
- ✅ Clear scope and focus  

**Source-available** or **commercial-first** tools noted explicitly.

---

## Tool Format
    ToolName – One-line description and use case.
    GitHub Docs
    language:Python deploy:k8s focus:ml maturity:established


## Tag Legend

| Prefix | Examples |
|--------|----------|
| `language:` | Python, Go, Rust, JavaScript, Polyglot |
| `deploy:` | k8s, docker, serverless, cli, library |
| `focus:` | data, ml, llm, agents, rag, infra, security, governance |
| `maturity:` | early, growing (500-5k stars), established (>5k stars), enterprise |

---

## Contributing

Contributions welcome! This repo aims to be a living directory of the AI Ops ecosystem.

### Before submitting a PR:

1. **Verify** the tool meets selection criteria  
2. **Check** it's not already listed  
3. **Add** in alphabetical order within category  
4. **Include** GitHub link + 2-3 relevant tags  
5. **Keep** description neutral (no marketing copy)  

### PR Checklist:
✅ Meets selection criteria
✅ Has GitHub + Docs links
✅ Includes language + deploy + focus tags
✅ Alphabetical order
✅ Neutral description

---

## Roadmap

- Tag tools by maturity level and deployment model  
- Highlight governance-relevant features (audit logs, RBAC, policy engines)  
- Add example stacks for common patterns  
- Submit to [sindresorhus/awesome](https://github.com/sindresorhus/awesome)  
- Prune unmaintained projects annually  

---

## Related Lists

[![Stars](https://img.shields.io/github/stars/kelvins/awesome-mlops?style=social)](https://github.com/kelvins/awesome-mlops) [![Stars](https://img.shields.io/github/stars/tensorchord/Awesome-LLMOps?style=social)](https://github.com/tensorchord/Awesome-LLMOps)

**License**: [MIT](LICENSE)  
**Made with**: Love for open source AI infrastructure 💚

