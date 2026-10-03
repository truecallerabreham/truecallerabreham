<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=soft&color=0:0b2027,55:16323b,100:1f4550&height=110&text=Abreham%20Melese&fontSize=34&fontColor=e6edf3&desc=AI%20%26%20LLM%20Systems%20Engineer&descSize=16&descColor=9fb3bd&descAlignY=75" alt="Abreham Melese" width="100%"/>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/abrehammelese/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="https://portifolio-fawn-pi-85.vercel.app"><img src="https://img.shields.io/badge/Portfolio_Website-1f4550?style=for-the-badge&logoColor=white" alt="Portfolio"/></a>
  <a href="mailto:xvimelese@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
</p>

## Hey, I'm Abreham Melese 👋

**AI & LLM Systems Engineer** · Agents · RAG · Observability · MCP Infrastructure · Multimodal AI · Small Language Models

- **11 merged upstream PRs** across tier-1 AI, ML, and agent ecosystems — fixing distributed checkpoint resumption in **Hugging Face Accelerate**, CLI serialization & Windows typing in **Pydantic**, subagent sandbox isolation in **Raven**, batch update consistency in **Qdrant**, MCP server tools in **Google Workspace MCP**, dataset streaming in **Lightning AI**, and auth reliability in **Agenta**.
- **17 active pull requests** under review across **CrewAI** (59k★), **LiteLLM** (60k★), **LlamaIndex** (52k★), **Agno** (42k★), **DSPy** (38k★), **DeepEval** (18k★), and **Instructor** (14k★).
- **480k+ combined GitHub stars** in contributed open-source repositories.
- Builder of end-to-end production AI systems: **EnterpriseRAG**, **SmartGuard**, **LLM Observability Dashboard**, and **Arc Canvas**.

<p align="center">
  <img height="165" src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=truecallerabreham&theme=github_dark" alt="GitHub stats"/>
  <img height="165" src="https://streak-stats.demolab.com/?user=truecallerabreham&theme=github-dark-blue&hide_border=true" alt="Contribution streak"/>
</p>

I focus on:
- LLM agents and agent frameworks
- RAG and retrieval systems
- LLM evaluation and observability
- MCP and tool-use infrastructure
- Multimodal AI
- Efficient language models and inference.
- occasinally i build the tools that i use from scratch.(forexample redis from scratch , docker and some llms architecture)

---

### Open Source Contributions

46 total pull requests across 21 upstream projects, with **11 merged upstream pull requests** in production frameworks representing **480,000+ combined GitHub stars**.

| Project | Merged | What the PRs cover | Highlight fixes |
|---------|:------:|--------------------|-----------------|
| [huggingface/accelerate](https://github.com/huggingface/accelerate) (9.9k★) | **1** | Distributed training & DataLoader checkpoint restoration | [#4296](https://github.com/huggingface/accelerate/pull/4296) Fixed critical checkpoint resumption regression where `skip_first_batches` dropped `drop_last`, `non_blocking`, `slice_fn`, and `mesh` parameters upon dataloader reconstitution |
| [pydantic/pydantic-settings](https://github.com/pydantic/pydantic-settings) (1.5k★) | **2** | CLI argument serialization and cross-platform static typing | [#992](https://github.com/pydantic/pydantic-settings/pull/992) Fixed `IndexError: list index out of range` in `CliApp.serialize` when serializing models with non-empty `CliUnknownArgs`<br>[#982](https://github.com/pydantic/pydantic-settings/pull/982) Resolved Windows Mypy static type checking failure (`mypy --platform win32`) on `Path.is_mount` |
| [EverMind-AI/Raven](https://github.com/EverMind-AI/Raven) (4.9k★) | **1** | Multi-agent execution sandbox isolation and tool boundaries | [#827](https://github.com/EverMind-AI/Raven/pull/827) Propagated `tools.sandbox` and `tools.restrict_to_workspace` down to playbook `SubagentManager` instances and shared `ProviderPool` across stints |
| [The-PR-Agent/pr-agent](https://github.com/The-PR-Agent/pr-agent) (13.2k★) | **1** | Automated code review and VCS provider payload normalization | [#3736](https://github.com/The-PR-Agent/pr-agent/pull/3736) Prepared and normalized outgoing comment bodies in AWS CodeCommit provider before calling `publish_code_suggestions` to prevent AWS API payload rejection |
| [taylorwilsdon/google_workspace_mcp](https://github.com/taylorwilsdon/google_workspace_mcp) (3.3k★) | **3** | Model Context Protocol (MCP) tool schemas for Google Workspace | [#1190](https://github.com/taylorwilsdon/google_workspace_mcp/pull/1190) Relaxed union schema on Google Chat `send_message` to allow plain messages without schema errors<br>[#1189](https://github.com/taylorwilsdon/google_workspace_mcp/pull/1189) Fixed Google Forms tool creation by mapping title to `documentTitle` and applying descriptions via `batchUpdate`<br>[#1155](https://github.com/taylorwilsdon/google_workspace_mcp/pull/1155) Normalized attendee dictionaries into valid Google Calendar API v3 structures |
| [qdrant/qdrant-client](https://github.com/qdrant/qdrant-client) (1.4k★) | **1** | Local vector store consistency and point update semantics | [#1493](https://github.com/qdrant/qdrant-client/pull/1493) Enforced `UpdateMode` semantics in local client batch updates and prevented operations on deleted points from reviving ghost points |
| [Agenta-AI/agenta](https://github.com/Agenta-AI/agenta) (4.8k★) | **1** | Backend authentication and error telemetry logging | [#5377](https://github.com/Agenta-AI/agenta/pull/5377) Fixed logging typo (`exc_infp` → `exc_info`) in auth service that swallowed exception stack traces during organization auto-join failures |
| [Lightning-AI/litData](https://github.com/Lightning-AI/litData) (615★) | **1** | Streaming dataset state tracking and checkpoint resumption | [#928](https://github.com/Lightning-AI/litData/pull/928) Reset wrapper sample and cycle counters on `reset_state_dict` to eliminate distributed offset drift |

<details>
<summary>All 11 Merged Upstream Pull Requests (Detailed Table)</summary>

| Repository | Stars | Pull Request | Category | Problem & Solution |
| :--- | :---: | :---: | :--- | :--- |
| **[The-PR-Agent/pr-agent](https://github.com/The-PR-Agent/pr-agent)** | ⭐ 13.2k | [#3736](https://github.com/The-PR-Agent/pr-agent/pull/3736) | Developer Tools & MCP | Normalizes outgoing comment bodies in AWS CodeCommit provider before calling `publish_code_suggestions` to prevent AWS API payload rejection. |
| **[huggingface/accelerate](https://github.com/huggingface/accelerate)** | ⭐ 9.9k | [#4296](https://github.com/huggingface/accelerate/pull/4296) | AI & ML Infrastructure | Fixed checkpoint resumption regression where `skip_first_batches` dropped `drop_last`, `non_blocking`, `slice_fn`, and `mesh` parameters during distributed DataLoader reconstitution. |
| **[EverMind-AI/Raven](https://github.com/EverMind-AI/Raven)** | ⭐ 4.9k | [#827](https://github.com/EverMind-AI/Raven/pull/827) | Agent Frameworks & Sandbox | Forwards `tools.sandbox` and `tools.restrict_to_workspace` to playbook `SubagentManager` instances and shares `ProviderPool` across subagent stints for reliable sandbox isolation. |
| **[Agenta-AI/agenta](https://github.com/Agenta-AI/agenta)** | ⭐ 4.8k | [#5377](https://github.com/Agenta-AI/agenta/pull/5377) | AI & ML Infrastructure | Fixed logging keyword argument typo (`exc_infp` → `exc_info`) in auth service that swallowed exception tracebacks during organization auto-join failures. |
| **[taylorwilsdon/google_workspace_mcp](https://github.com/taylorwilsdon/google_workspace_mcp)** | ⭐ 3.3k | [#1190](https://github.com/taylorwilsdon/google_workspace_mcp/pull/1190) | Developer Tools & MCP | Allows Google Chat `send_message` MCP tool to send plain text messages without triggering strict union schema validation errors on unused optional fields. |
| **[taylorwilsdon/google_workspace_mcp](https://github.com/taylorwilsdon/google_workspace_mcp)** | ⭐ 3.3k | [#1189](https://github.com/taylorwilsdon/google_workspace_mcp/pull/1189) | Developer Tools & MCP | Fixed Google Forms tool creation by mapping title to `documentTitle` and applying form descriptions through subsequent `batchUpdate` calls. |
| **[taylorwilsdon/google_workspace_mcp](https://github.com/taylorwilsdon/google_workspace_mcp)** | ⭐ 3.3k | [#1155](https://github.com/taylorwilsdon/google_workspace_mcp/pull/1155) | Developer Tools & MCP | Normalized attendee dictionaries into valid Google Calendar API v3 structures, preventing `400 Bad Request` exceptions on event creation. |
| **[pydantic/pydantic-settings](https://github.com/pydantic/pydantic-settings)** | ⭐ 1.5k | [#992](https://github.com/pydantic/pydantic-settings/pull/992) | Developer Tools & MCP | Fixed `IndexError: list index out of range` in `CliApp.serialize` when serializing settings models that capture unknown command-line arguments. |
| **[pydantic/pydantic-settings](https://github.com/pydantic/pydantic-settings)** | ⭐ 1.5k | [#982](https://github.com/pydantic/pydantic-settings/pull/982) | Developer Tools & MCP | Resolved platform-specific static type checking error on Windows (`mypy --platform win32`) by safely guarding `Path.is_mount` attribute resolution. |
| **[qdrant/qdrant-client](https://github.com/qdrant/qdrant-client)** | ⭐ 1.4k | [#1493](https://github.com/qdrant/qdrant-client/pull/1493) | Vector DB & RAG | Enforced `UpdateMode` semantics in Qdrant Local client batch updates and prevented operations on deleted points from reviving ghost points. |
| **[Lightning-AI/litData](https://github.com/Lightning-AI/litData)** | ⭐ 615 | [#928](https://github.com/Lightning-AI/litData/pull/928) | Data & Streaming | Fixed streaming dataset checkpoint state synchronization by resetting wrapper sample and cycle counters upon `reset_state_dict`. |

</details>

<details>
<summary>Active Pull Requests Under Upstream Review (17)</summary>

| Repository | Stars | PR | Highlights |
| :--- | :---: | :---: | :--- |
| **[BerriAI/litellm](https://github.com/BerriAI/litellm)** | ⭐ 59.9k | [#42158](https://github.com/BerriAI/litellm/pull/42158) | Multi-turn reasoning persistence: preserves and promotes `reasoning_content` across conversation turns on DeepSeek thinking models. |
| **[crewAIInc/crewAI](https://github.com/crewAIInc/crewAI)** | ⭐ 59.2k | [#7828](https://github.com/crewAIInc/crewAI/pull/7828) | RAG auto-detection isolation across items and case-insensitive extension matching. |
| **[crewAIInc/crewAI](https://github.com/crewAIInc/crewAI)** | ⭐ 59.2k | [#7779](https://github.com/crewAIInc/crewAI/pull/7779) | Fixed `StaticToolFilter` security semantics so empty tool filter lists block all tools rather than defaulting to allow-all. |
| **[crewAIInc/crewAI](https://github.com/crewAIInc/crewAI)** | ⭐ 59.2k | [#7671](https://github.com/crewAIInc/crewAI/pull/7671) | Safely collapses multimodal user message blocks into clean text strings in Flow state. |
| **[run-llama/llama_index](https://github.com/run-llama/llama_index)** | ⭐ 52.4k | [#23154](https://github.com/run-llama/llama_index/pull/23154) | Enables `BaseWorkflowAgent` and `AgentWorkflow` to initialize gracefully from history containing assistant/tool messages. |
| **[run-llama/llama_index](https://github.com/run-llama/llama_index)** | ⭐ 52.4k | [#23152](https://github.com/run-llama/llama_index/pull/23152) | Preserves non-text content blocks (`ThinkingBlock`, `ToolCallBlock`, `CitationBlock`) during streaming history writes. |
| **[agno-agi/agno](https://github.com/agno-agi/agno)** | ⭐ 42.4k | [#10625](https://github.com/agno-agi/agno/pull/10625) | Prevents leading-dash grep flag injection, fixes match count boundary calculation, and removes unintended truncation footers. |
| **[agno-agi/agno](https://github.com/agno-agi/agno)** | ⭐ 42.4k | [#10623](https://github.com/agno-agi/agno/pull/10623) | Enables `CodeScorer.digest()` to fingerprint callable class instances without `TypeError: inspect.getsource()`. |
| **[stanfordnlp/dspy](https://github.com/stanfordnlp/dspy)** | ⭐ 38.4k | [#10465](https://github.com/stanfordnlp/dspy/pull/10465) | Recursively enforces `additionalProperties: false` across nested `oneOf`, `prefixItems`, and tuple arrays for OpenAI strict mode. |
| **[confident-ai/deepeval](https://github.com/confident-ai/deepeval)** | ⭐ 18.5k | [#3327](https://github.com/confident-ai/deepeval/pull/3327) | Safely extracts model outputs when parsing Claude responses with thinking blocks and tool use signatures. |
| **[567-labs/instructor](https://github.com/567-labs/instructor)** | ⭐ 14.0k | [#2670](https://github.com/567-labs/instructor/pull/2670) | Adds native support for PEP 604 union syntax (`X \| Y`) in Instructor's DSL type introspection and `ModelAdapter`. |
| **[traceloop/openllmetry](https://github.com/traceloop/openllmetry)** | ⭐ 7.5k | [#4334](https://github.com/traceloop/openllmetry/pull/4334) | Prevents `TypeError` crashes in OpenLLMetry tracing by supplying default empty list fallbacks across Bedrock providers. |
| **[traceloop/openllmetry](https://github.com/traceloop/openllmetry)** | ⭐ 7.5k | [#4333](https://github.com/traceloop/openllmetry/pull/4333) | Fixes `UnicodeDecodeError` on Windows systems by specifying `encoding='utf-8'` on all file open calls. |
| **[EverMind-AI/Raven](https://github.com/EverMind-AI/Raven)** | ⭐ 4.9k | [#813](https://github.com/EverMind-AI/Raven/pull/813) | Updated sandbox driver to pass `NetworkSpec` into `BoxOptions`, restoring compatibility with Boxlite 0.9.5 network isolation. |
| **[Agenta-AI/agenta](https://github.com/Agenta-AI/agenta)** | ⭐ 4.8k | [#6979](https://github.com/Agenta-AI/agenta/pull/6979) | Defensive null checks in SDK LiteLLM handler and circular import fixes during lazy asset loading. |
| **[Agenta-AI/agenta](https://github.com/Agenta-AI/agenta)** | ⭐ 4.8k | [#5389](https://github.com/Agenta-AI/agenta/pull/5389) | Prevents global lockouts of anonymous users by gating negative token caching on non-null user identifiers. |
| **[he-yufeng/RepoWiki](https://github.com/he-yufeng/RepoWiki)** | ⭐ 287 | [#6](https://github.com/he-yufeng/RepoWiki/pull/6) | Standard library import ordering ahead of local module imports in test suite per PEP 8. |

</details>

*Explore all 46 open-source pull requests across 21 repositories on my [Portfolio](https://portifolio-fawn-pi-85.vercel.app/open-source).*

---

### Featured Projects

| Project | Stars / Status | What it is |
|---------|:--------------:|------------|
| [EnterpriseRAG](https://github.com/truecallerabreham/Enterprise-RAG-For-teams) | Active | Cross-repository code intelligence for engineering teams: hybrid search + graph expansion, cross-encoder reranking, and citation validation loop. `Python` `FastAPI` `LangGraph` `Tree-sitter` `Qdrant` `BM25` `Neo4j` `RAG` |
| [SmartGuard](https://github.com/truecallerabreham/Smart_cctv) | Active | Multimodal incident-auditing agent for transit CCTV footage: frame-level VLM captioning, semantic video search, FastMCP tool integration, and ffmpeg clip extraction. `Multimodal AI` `VLM` `MCP` `FastAPI` `Pixeltable` `Opik` `ffmpeg` `React` |
| [LLM Observability & Eval Dashboard](https://github.com/truecallerabreham/llm-observability-dashboard) | Active | Self-hosted observability & eval stack for deployed LLM apps: OpenTelemetry traces, DeepEval/RAGAS evaluation scores, ClickHouse metrics, and operational alerts. `OpenTelemetry` `DeepEval` `RAGAS` `ClickHouse` `Prometheus` `Next.js` |
| [Arc - Architecture Canvas](https://github.com/truecallerabreham/Vibe) | Active | Interactive developer tool that maps system ideas to real open-source architectures, renders file trees into interactive diagrams, and facilitates architecture review before coding. `TypeScript` `React Flow` `CLI` `GitHub Search` `LLM` |
| [Clipagent](https://github.com/truecallerabreham/Clipagent) | Active | Multimodal video search & clip extraction tool: natural-language queries, semantic similarity over frames, and automated clip segmentation. `FastMCP` `Pixeltable` `FastAPI` `React` `Docker` |
| [Telecall](https://github.com/truecallerabreham/Telecall) | Active | AI voice mobile-carrier assistant for automated call-center operations: LangGraph + Groq + FastRTC + Twilio + Qdrant for real-time speech and support. `LangGraph` `Groq` `FastRTC` `Twilio` `Qdrant` `STT` `TTS` |

<details>
<summary>All Projects (11)</summary>

| Area | Project | Tech Stack | Notes |
|------|---------|------------|-------|
| Code Intelligence / RAG | [EnterpriseRAG](https://github.com/truecallerabreham/Enterprise-RAG-For-teams) | Python, FastAPI, LangGraph, Qdrant, Neo4j | Cross-repo code retrieval with hybrid search & graph-based code structure extraction. |
| Multimodal AI / Video | [SmartGuard](https://github.com/truecallerabreham/Smart_cctv) | Pixeltable, FastMCP, VLM, FastAPI, React | Automated CCTV incident auditing and video evidence extraction. |
| Observability & Evals | [LLM Observability Dashboard](https://github.com/truecallerabreham/llm-observability-dashboard) | OpenTelemetry, DeepEval, ClickHouse, Next.js | Production traces, drift detection, and evaluation dashboards for LLM apps. |
| System Architecture | [Arc - Architecture Canvas](https://github.com/truecallerabreham/Vibe) | TypeScript, React Flow, GitHub API, LLM | Interactive system design and codebase architecture canvas. |
| Multimodal Video | [Clipagent](https://github.com/truecallerabreham/Clipagent) | FastMCP, Pixeltable, FastAPI, React, Docker | Video understanding, semantic search, and clip extraction pipeline. |
| Real-time Voice AI | [Telecall](https://github.com/truecallerabreham/Telecall) | LangGraph, Groq, FastRTC, Twilio, Qdrant | End-to-end low-latency voice agent for telecom customer support. |
| RAG Research | [Advanced RAG From Scratch](https://github.com/truecallerabreham/Advanced_RAG_From_Scratch.) | Python, BM25, Dense Embeddings, Multimodal | Advanced RAG implementations from foundational dense retrieval to multimodal search. |
| Agent Framework | [Forla](https://github.com/truecallerabreham/FLORA) | Python, AsyncIO, Multi-Agent | Async-first framework for deterministic agent workflows and transparent execution loops. |
| Infrastructure / MCP | [DigitalOcean MCP Server](https://github.com/truecallerabreham/mcp-server-digitalocean) | TypeScript, MCP Protocol, DigitalOcean API | Manage Droplets, databases, domains, and cloud resources via structured tool calls. |
| Developer Ergonomics | [Context Visualizer](https://github.com/truecallerabreham/preflight_contex) | TypeScript, Context Engineering | Local proxy visualizing coding agent prompts, token costs, and context trimming. |
| Classical MLOps | [Fraud Detection System](https://github.com/truecallerabreham/fraud_detection_system) | Python, MLflow, Docker, GitHub Actions | End-to-end ML classification pipeline with automated testing and containerized CI/CD. |

</details>

---

### Research in Progress

**[Efficient InkubaLM for Edge and Mobile Inference](https://huggingface.co/Lelapa-AI/InkubaLM-0.4B)** *(Active Research)*  
Independent research exploring attention redesign (LLaMA attention → Multi-head Latent Attention / MLA) for low-latency on-device inference while retaining low-resource language representations through knowledge distillation.

**[LLM-Powered Android Keyboard](https://developer.android.com/)** *(Active Prototyping)*  
Investigating small on-device language models for contextual next-word and phrase prediction under strict mobile compute, latency, and thermal budgets.

---

### Technical Skills

#### LLMs, Agents & Tooling
![Python](https://img.shields.io/badge/Python-1a1a1a?style=for-the-badge&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-1a1a1a?style=for-the-badge&logo=fastapi&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1a1a1a?style=for-the-badge)
![LangChain](https://img.shields.io/badge/LangChain-1a1a1a?style=for-the-badge&logo=langchain&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-1a1a1a?style=for-the-badge&logo=huggingface&logoColor=white)
![Transformers](https://img.shields.io/badge/Transformers-1a1a1a?style=for-the-badge)
![MCP](https://img.shields.io/badge/MCP-1a1a1a?style=for-the-badge)
![LangSmith](https://img.shields.io/badge/LangSmith-1a1a1a?style=for-the-badge)
![Pydantic](https://img.shields.io/badge/Pydantic-1a1a1a?style=for-the-badge&logo=pydantic&logoColor=white)

#### RAG & Retrieval
![Qdrant](https://img.shields.io/badge/Qdrant-1a1a1a?style=for-the-badge&logo=qdrant&logoColor=white)
![Pinecone](https://img.shields.io/badge/Pinecone-1a1a1a?style=for-the-badge)
![ChromaDB](https://img.shields.io/badge/ChromaDB-1a1a1a?style=for-the-badge)
![Neo4j](https://img.shields.io/badge/Neo4j-1a1a1a?style=for-the-badge&logo=neo4j&logoColor=white)
![BM25](https://img.shields.io/badge/BM25-1a1a1a?style=for-the-badge)
![Tree-sitter](https://img.shields.io/badge/Tree--sitter-1a1a1a?style=for-the-badge)
![Voyage AI](https://img.shields.io/badge/Voyage%20AI-1a1a1a?style=for-the-badge)
![FAISS](https://img.shields.io/badge/FAISS-1a1a1a?style=for-the-badge)

#### LLM Observability & Evaluation
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-1a1a1a?style=for-the-badge&logo=opentelemetry&logoColor=white)
![DeepEval](https://img.shields.io/badge/DeepEval-1a1a1a?style=for-the-badge)
![RAGAS](https://img.shields.io/badge/RAGAS-1a1a1a?style=for-the-badge)
![ClickHouse](https://img.shields.io/badge/ClickHouse-1a1a1a?style=for-the-badge&logo=clickhouse&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-1a1a1a?style=for-the-badge&logo=prometheus&logoColor=white)
![Opik](https://img.shields.io/badge/Opik-1a1a1a?style=for-the-badge)
![Grafana](https://img.shields.io/badge/Grafana-1a1a1a?style=for-the-badge&logo=grafana&logoColor=white)

#### Multimodal AI
![VLM](https://img.shields.io/badge/VLM-1a1a1a?style=for-the-badge)
![CLIP](https://img.shields.io/badge/CLIP-1a1a1a?style=for-the-badge)
![FFmpeg](https://img.shields.io/badge/FFmpeg-1a1a1a?style=for-the-badge&logo=ffmpeg&logoColor=white)
![Pixeltable](https://img.shields.io/badge/Pixeltable-1a1a1a?style=for-the-badge)
![OpenCV](https://img.shields.io/badge/OpenCV-1a1a1a?style=for-the-badge&logo=opencv&logoColor=white)
![Whisper](https://img.shields.io/badge/Whisper-1a1a1a?style=for-the-badge)
![React](https://img.shields.io/badge/React-1a1a1a?style=for-the-badge&logo=react&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind-1a1a1a?style=for-the-badge&logo=tailwindcss&logoColor=white)

#### Voice, Audio & Mobile
![Twilio](https://img.shields.io/badge/Twilio-1a1a1a?style=for-the-badge&logo=twilio&logoColor=white)
![WebRTC](https://img.shields.io/badge/WebRTC-1a1a1a?style=for-the-badge&logo=webrtc&logoColor=white)
![FastRTC](https://img.shields.io/badge/FastRTC-1a1a1a?style=for-the-badge)
![TTS](https://img.shields.io/badge/TTS-1a1a1a?style=for-the-badge)
![STT](https://img.shields.io/badge/STT-1a1a1a?style=for-the-badge)
![Android](https://img.shields.io/badge/Android-1a1a1a?style=for-the-badge&logo=android&logoColor=white)

#### LLM Architecture & Efficient Inference
![Multi-head Latent Attention](https://img.shields.io/badge/MLA-1a1a1a?style=for-the-badge)
![Knowledge Distillation](https://img.shields.io/badge/Knowledge%20Distillation-1a1a1a?style=for-the-badge)
![Quantization](https://img.shields.io/badge/Quantization-1a1a1a?style=for-the-badge)
![PyTorch](https://img.shields.io/badge/PyTorch-1a1a1a?style=for-the-badge&logo=pytorch&logoColor=white)
![vLLM](https://img.shields.io/badge/vLLM-1a1a1a?style=for-the-badge)

#### Languages & Infrastructure
![TypeScript](https://img.shields.io/badge/TypeScript-1a1a1a?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-1a1a1a?style=for-the-badge&logo=javascript&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-1a1a1a?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-1a1a1a?style=for-the-badge&logo=githubactions&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-1a1a1a?style=for-the-badge&logo=next.js&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-1a1a1a?style=for-the-badge&logo=postgresql&logoColor=white)
