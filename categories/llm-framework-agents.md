# LLM Frameworks, RAG & Agents

Frameworks for LLM orchestration, RAG pipelines, multi-agent systems and tool calling.

Focus on **production maturity** – tracing, error recovery, streaming, async support and deployment hooks.

---

- **AutoGen** – Microsoft framework for multi-agent conversations. Enables complex workflows with human-in-loop and tool use.  
  [GitHub](https://github.com/microsoft/autogen) [Docs](https://microsoft.github.io/autogen/)  
  `language:Python` `deploy:library` `focus:llm,agents` `maturity:established`

- **Haystack** – End-to-end framework for search and RAG pipelines. Modular nodes, advanced retrieval, evaluation.  
  [GitHub](https://github.com/deepset-ai/haystack) [Docs](https://docs.haystack.deepset.ai/docs/intro)  
  `language:Python` `deploy:library,k8s` `focus:llm,rag` `maturity:established`

- **LangChain** – Modular framework for LLM chains, agents, tools, RAG and memory. Massive ecosystem but higher complexity.  
  [GitHub](https://github.com/langchain-ai/langchain) [Docs](https://python.langchain.com/docs/)  
  `language:Python,JS` `deploy:library` `focus:llm,agents,rag` `maturity:enterprise`

- **LlamaIndex** – Data framework for LLM apps: ingestion, indexing, querying, agents. Strong RAG and structured data focus.  
  [GitHub](https://github.com/run-llama/llama_index) [Docs](https://docs.llamaindex.ai/)  
  `language:Python` `deploy:library` `focus:llm,rag,agents` `maturity:enterprise`

---

**Notes:**  
- **LangChain/LlamaIndex** dominate ecosystem; **Haystack** for search‑heavy RAG; **AutoGen** for multi‑agent.  
- LiteLLM (proxy/gateway) belongs in serving/inference.  
- Semantic Kernel, CrewAI emerging but less mature for production.  
- Missing something? Open a PR with tags and evidence of adoption.
