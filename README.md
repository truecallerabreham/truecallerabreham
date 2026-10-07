<p align="center">
ABREHAM MELESE
<p align="center">
  <a href="https://www.linkedin.com/in/abrehammelese/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="https://portifolio-fawn-pi-85.vercel.app"><img src="https://img.shields.io/badge/Portfolio_Website-1f4550?style=for-the-badge&logoColor=white" alt="Portfolio"/></a>
  <a href="mailto:xvimelese@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
</p>

## Hey, I'm Abreham Melese 👋

**AI & LLM Systems Engineer** · AI Agents · RAG Systems · LLM Applications · AI Backend Engineering · Open Source  · (Passionate about LLM Inference hobby)
- **12 merged upstream PRs** across tier-1 AI, ML, and agent ecosystems — fixing distributed checkpoint resumption in **Hugging Face Accelerate**, hardening CLI serialization for dynamic agent schemas and resolving critical Windows runtime typing bugs **Pydantic** subagent sandbox isolation & Boxlite network specs in **Raven**, batch update consistency in **Qdrant**, MCP server tools in **Google Workspace MCP**, dataset streaming in **Lightning AI**, and auth reliability in **Agenta**.
- Merged per repository: Google Workspace MCP (3), pydantic-settings (2), Raven (2), accelerate (1), pr-agent (1), agenta (1), qdrant-client (1), litData (1).
- Selected public projects led by **[EnterpriseRAG](https://github.com/truecallerabreham/Enterprise-RAG-For-teams)** ([Demo Video](https://cap.so/s/901ps3jsw09s8x9)), **[SmartGuard](https://github.com/truecallerabreham/Smart_cctv)** ([Demo Video](https://cap.so/s/ryg3x6qx2r187yk)), **LLM Observability Dashboard**, and **Arc Canvas**.

<p align="center">
  <img height="165" src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=truecallerabreham&theme=github_dark" alt="GitHub stats"/>
  <img height="165" src="https://streak-stats.demolab.com/?user=truecallerabreham&theme=github-dark-blue&hide_border=true" alt="Contribution streak"/>
</p>

---

### Open Source Contributions

| Repository | Pull Request | Focus | What it fixes |
|---------|:---:|--------|-----------------|
| **[The-PR-Agent/pr-agent](https://github.com/The-PR-Agent/pr-agent)** <small>13.2k&#9733;</small> | [#3736](https://github.com/The-PR-Agent/pr-agent/pull/3736) | Automated code review & VCS provider payloads | Normalizes outgoing comment bodies in AWS CodeCommit provider before calling `publish_code_suggestions` to prevent AWS API payload rejection. |
| **[huggingface/accelerate](https://github.com/huggingface/accelerate)** <small>9.9k&#9733;</small> | [#4296](https://github.com/huggingface/accelerate/pull/4296) | Distributed training & DataLoader checkpoint restoration | Fixed checkpoint resumption regression where `skip_first_batches` dropped `drop_last`, `non_blocking`, `slice_fn`, and `mesh` parameters during distributed DataLoader reconstitution. |
| **[EverMind-AI/Raven](https://github.com/EverMind-AI/Raven)** <small>4.9k&#9733;</small> | [#827](https://github.com/EverMind-AI/Raven/pull/827) | Multi-agent sandbox isolation & tool boundaries | Forwards `tools.sandbox` and `tools.restrict_to_workspace` to playbook `SubagentManager` instances and shares `ProviderPool` across subagent stints for reliable sandbox isolation. |
| **[EverMind-AI/Raven](https://github.com/EverMind-AI/Raven)** <small>4.9k&#9733;</small> | [#813](https://github.com/EverMind-AI/Raven/pull/813) | Sandbox execution & Boxlite 0.9.5 network specification | Passed `NetworkSpec` to Boxlite 0.9.5 `BoxOptions`, resolving `TypeError` on sandbox startup when configuring network modes and domain allowlists (#797). |
| **[Agenta-AI/agenta](https://github.com/Agenta-AI/agenta)** <small>4.8k&#9733;</small> | [#5377](https://github.com/Agenta-AI/agenta/pull/5377) | Backend authentication & error telemetry logging | Fixed logging keyword argument typo (`exc_infp` → `exc_info`) in auth service that swallowed exception tracebacks during organization auto-join failures. |
| **[taylorwilsdon/google_workspace_mcp](https://github.com/taylorwilsdon/google_workspace_mcp)** <small>3.3k&#9733;</small> | [#1190](https://github.com/taylorwilsdon/google_workspace_mcp/pull/1190) | MCP tool schemas for Google Workspace | Allows Google Chat `send_message` MCP tool to send plain text messages without triggering strict union schema validation errors on unused optional fields. |
| **[taylorwilsdon/google_workspace_mcp](https://github.com/taylorwilsdon/google_workspace_mcp)** <small>3.3k&#9733;</small> | [#1189](https://github.com/taylorwilsdon/google_workspace_mcp/pull/1189) | MCP tool schemas for Google Workspace | Fixed Google Forms tool creation by mapping title to `documentTitle` and applying form descriptions through subsequent `batchUpdate` calls. |
| **[taylorwilsdon/google_workspace_mcp](https://github.com/taylorwilsdon/google_workspace_mcp)** <small>3.3k&#9733;</small> | [#1155](https://github.com/taylorwilsdon/google_workspace_mcp/pull/1155) | MCP tool schemas for Google Workspace | Normalized attendee dictionaries into valid Google Calendar API v3 structures, preventing `400 Bad Request` exceptions on event creation. |
| **[pydantic/pydantic-settings](https://github.com/pydantic/pydantic-settings)** <small>1.5k&#9733;</small> | [#992](https://github.com/pydantic/pydantic-settings/pull/992) | CLI argument serialization | Fixed `IndexError: list index out of range` in `CliApp.serialize` when serializing settings models that capture unknown command-line arguments. |
| **[pydantic/pydantic-settings](https://github.com/pydantic/pydantic-settings)** <small>1.5k&#9733;</small> | [#982](https://github.com/pydantic/pydantic-settings/pull/982) | Cross-platform static typing | Resolved platform-specific static type checking error on Windows (`mypy --platform win32`) by safely guarding `Path.is_mount` attribute resolution. |
| **[qdrant/qdrant-client](https://github.com/qdrant/qdrant-client)** <small>1.4k&#9733;</small> | [#1493](https://github.com/qdrant/qdrant-client/pull/1493) | Local vector store consistency & update semantics | Enforced `UpdateMode` semantics in Qdrant Local client batch updates and prevented operations on deleted points from reviving ghost points. |
| **[Lightning-AI/litData](https://github.com/Lightning-AI/litData)** <small>615&#9733;</small> | [#928](https://github.com/Lightning-AI/litData/pull/928) | Streaming dataset checkpoint state tracking | Fixed streaming dataset checkpoint state synchronization by resetting wrapper sample and cycle counters upon `reset_state_dict`. |

<details>
<summary>Active Pull Requests Under Upstream Review (15)</summary>

| Repository | Pull Request | Focus | What it fixes |
|------------|:------------:|-------|---------------|
| **[crewAIInc/crewAI](https://github.com/crewAIInc/crewAI)** <small>59.2k&#9733;</small> | [#7828](https://github.com/crewAIInc/crewAI/pull/7828) | Multi-item RAG auto-detection | Isolates content-type autodetection across multi-item RAG knowledge loaders and adds case-insensitive support for uppercase file extensions. |
| **[crewAIInc/crewAI](https://github.com/crewAIInc/crewAI)** <small>59.2k&#9733;</small> | [#7779](https://github.com/crewAIInc/crewAI/pull/7779) | Tool filtering security | Fixed tool filtering security semantics so that providing an explicit empty allowed_tool_names array blocks all tools rather than defaulting to allow-all. |
| **[crewAIInc/crewAI](https://github.com/crewAIInc/crewAI)** <small>59.2k&#9733;</small> | [#7671](https://github.com/crewAIInc/crewAI/pull/7671) | Multimodal message handling | Safely collapses multimodal user message blocks into clean text strings in Flow state to prevent serialization errors when passing history to text-only LLMs. |
| **[run-llama/llama_index](https://github.com/run-llama/llama_index)** <small>52.4k&#9733;</small> | [#23154](https://github.com/run-llama/llama_index/pull/23154) | Agent workflow initialization | Enables BaseWorkflowAgent and AgentWorkflow to initialize gracefully from chat history containing prior assistant or tool responses without requiring a new user message. |
| **[run-llama/llama_index](https://github.com/run-llama/llama_index)** <small>52.4k&#9733;</small> | [#23152](https://github.com/run-llama/llama_index/pull/23152) | Streaming chat history preservation | Preserves non-text content blocks when writing streaming chat responses back to message history. |
| **[BerriAI/litellm](https://github.com/BerriAI/litellm)** <small>26.5k&#9733;</small> | [#42158](https://github.com/BerriAI/litellm/pull/42158) | DeepSeek reasoning extraction | Promotes reasoning_content on multi-turn conversations for default thinking models. |
| **[agno-agi/agno](https://github.com/agno-agi/agno)** <small>22.6k&#9733;</small> | [#10625](https://github.com/agno-agi/agno/pull/10625) | Coding tools regex & pagination | Handles leading-dash grep patterns, exact-limit match counts, and truncated read_file footers in CodingTools. |
| **[agno-agi/agno](https://github.com/agno-agi/agno)** <small>22.6k&#9733;</small> | [#10623](https://github.com/agno-agi/agno/pull/10623) | Code scoring digestibility | Adds support for callable object instances in CodeScorer.digest(). |
| **[stanfordnlp/dspy](https://github.com/stanfordnlp/dspy)** <small>22.8k&#9733;</small> | [#10465](https://github.com/stanfordnlp/dspy/pull/10465) | Structured schema validation | Recursively applies strict JSON schema rules to oneOf, prefixItems, and items lists. |
| **[567-labs/instructor](https://github.com/567-labs/instructor)** <small>9.4k&#9733;</small> | [#2670](https://github.com/567-labs/instructor/pull/2670) | DSL type introspection | Adds native support for PEP 604 union syntax (X \| Y) in Instructor's DSL type introspection and ModelAdapter. |
| **[confident-ai/deepeval](https://github.com/confident-ai/deepeval)** <small>6.4k&#9733;</small> | [#3327](https://github.com/confident-ai/deepeval/pull/3327) | Anthropic tool output extraction | Safely extracts output parameters for tool use and thinking blocks in Anthropic evaluation runs. |
| **[traceloop/openllmetry](https://github.com/traceloop/openllmetry)** <small>5.6k&#9733;</small> | [#4334](https://github.com/traceloop/openllmetry/pull/4334) | Bedrock span telemetry | Adds missing default values to dictionary lookup calls in Bedrock span_utils. |
| **[traceloop/openllmetry](https://github.com/traceloop/openllmetry)** <small>5.6k&#9733;</small> | [#4333](https://github.com/traceloop/openllmetry/pull/4333) | Cross-platform file I/O | Adds explicit utf-8 encoding to file operations for Windows compatibility. |
| **[Agenta-AI/agenta](https://github.com/Agenta-AI/agenta)** <small>4.8k&#9733;</small> | [#6979](https://github.com/Agenta-AI/agenta/pull/6979) | SDK handler safeguards | Adds defensive safeguards to LiteLLM handler and lazy assets loading. |
| **[Agenta-AI/agenta](https://github.com/Agenta-AI/agenta)** <small>4.8k&#9733;</small> | [#5389](https://github.com/Agenta-AI/agenta/pull/5389) | Auth cache isolation | Gates cache deny on non-null user_id to prevent cross-user cache pollution. |

</details>

*Explore my complete open-source pull requests catalog on my [Portfolio](https://portifolio-fawn-pi-85.vercel.app/open-source).*

---

### Featured Projects

| Project | Demo | Status | What it is |
|---------|:----:|:------:|------------|
| [EnterpriseRAG](https://github.com/truecallerabreham/Enterprise-RAG-For-teams) | [▶ Video](https://cap.so/s/901ps3jsw09s8x9) | Active | Cross-repository code intelligence for engineering teams: hybrid search + graph expansion, cross-encoder reranking, and citation validation loop. `Python` `FastAPI` `LangGraph` `Tree-sitter` `Qdrant` `BM25` `Neo4j` `RAG` |
| [SmartGuard](https://github.com/truecallerabreham/Smart_cctv) | [▶ Video](https://cap.so/s/ryg3x6qx2r187yk) | Active | Multimodal incident-auditing agent for transit CCTV footage: frame-level VLM captioning, semantic video search, FastMCP tool integration, and ffmpeg clip extraction. `Multimodal AI` `VLM` `MCP` `FastAPI` `Pixeltable` `Opik` `ffmpeg` `React` |
| [LLM Observability & Eval Dashboard](https://github.com/truecallerabreham/llm-observability-dashboard) | — | Active | Self-hosted observability & eval stack for deployed LLM apps: OpenTelemetry traces, DeepEval/RAGAS evaluation scores, ClickHouse metrics, and operational alerts. `OpenTelemetry` `DeepEval` `RAGAS` `ClickHouse` `Prometheus` `Next.js` |
| [Arc - Architecture Canvas](https://github.com/truecallerabreham/Vibe) | — | Active | Interactive developer tool that maps system ideas to real open-source architectures, renders file trees into interactive diagrams, and facilitates architecture review before coding. `TypeScript` `React Flow` `CLI` `GitHub Search` `LLM` |
| [Clipagent](https://github.com/truecallerabreham/Clipagent) | — | Active | Multimodal video search & clip extraction tool: natural-language queries, semantic similarity over frames, and automated clip segmentation. `FastMCP` `Pixeltable` `FastAPI` `React` `Docker` |
| [Telecall](https://github.com/truecallerabreham/Telecall) | — | Active | AI voice mobile-carrier assistant for automated call-center operations: LangGraph + Groq + FastRTC + Twilio + Qdrant for real-time speech and support. `LangGraph` `Groq` `FastRTC` `Twilio` `Qdrant` `STT` `TTS` |

<details>
<summary>All Projects (11)</summary>

| Area | Project | Demo | Tech Stack | Notes |
|------|---------|:----:|------------|-------|
| Code Intelligence / RAG | [EnterpriseRAG](https://github.com/truecallerabreham/Enterprise-RAG-For-teams) | [▶ Video](https://cap.so/s/901ps3jsw09s8x9) | Python, FastAPI, LangGraph, Qdrant, Neo4j | Cross-repo code retrieval with hybrid search & graph-based code structure extraction. |
| Multimodal AI / Video | [SmartGuard](https://github.com/truecallerabreham/Smart_cctv) | [▶ Video](https://cap.so/s/ryg3x6qx2r187yk) | Pixeltable, FastMCP, VLM, FastAPI, React | Automated CCTV incident auditing and video evidence extraction. |
| Observability & Evals | [LLM Observability Dashboard](https://github.com/truecallerabreham/llm-observability-dashboard) | — | OpenTelemetry, DeepEval, ClickHouse, Next.js | Production traces, drift detection, and evaluation dashboards for LLM apps. |
| System Architecture | [Arc - Architecture Canvas](https://github.com/truecallerabreham/Vibe) | — | TypeScript, React Flow, GitHub API, LLM | Interactive system design and codebase architecture canvas. |
| Multimodal Video | [Clipagent](https://github.com/truecallerabreham/Clipagent) | — | FastMCP, Pixeltable, FastAPI, React, Docker | Video understanding, semantic search, and clip extraction pipeline. |
| Real-time Voice AI | [Telecall](https://github.com/truecallerabreham/Telecall) | — | LangGraph, Groq, FastRTC, Twilio, Qdrant | End-to-end low-latency voice agent for telecom customer support. |
| RAG Research | [Advanced RAG From Scratch](https://github.com/truecallerabreham/Advanced_RAG_From_Scratch.) | — | Python, BM25, Dense Embeddings, Multimodal | Advanced RAG implementations from foundational dense retrieval to multimodal search. |
| Agent Framework | [Forla](https://github.com/truecallerabreham/FLORA) | — | Python, AsyncIO, Multi-Agent | Async-first framework for deterministic agent workflows and transparent execution loops. |
| Infrastructure / MCP | [DigitalOcean MCP Server](https://github.com/truecallerabreham/mcp-server-digitalocean) | — | TypeScript, MCP Protocol, DigitalOcean API | Manage Droplets, databases, domains, and cloud resources via structured tool calls. |
| Developer Ergonomics | [Context Visualizer](https://github.com/truecallerabreham/preflight_contex) | — | TypeScript, Context Engineering | Local proxy visualizing coding agent prompts, token costs, and context trimming. |
| Classical MLOps | [Fraud Detection System](https://github.com/truecallerabreham/fraud_detection_system) | — | Python, MLflow, Docker, GitHub Actions | End-to-end ML classification pipeline with automated testing and containerized CI/CD. |

</details>

---

### Research in Progress

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
