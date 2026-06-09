# Building the AI Engine — A Practical Approach to Red Hat OpenShift AI 3.4

A sprint-focused, hands-on training course for Platform Engineers and AI infrastructure teams deploying and governing Red Hat OpenShift AI 3.4+. This course is designed to be completed in 1-2 days, equipping learners with the skills to build self-service GenAI platforms and enable production agentic applications for their organizations.

## Course Overview

This course uses a practical, narrative-driven approach across 8 modules. Each module includes three components:

| Component | Purpose |
|-----------|---------|
| **Interactive Quiz** | Diagnostic assessment to gauge readiness before studying the module |
| **Runbook** | Feature overview covering architecture, anti-patterns, cheat sheets, and business value |
| **Interactive Labs** | UI click-path walkthroughs for hands-on experience without dedicated lab infrastructure |

## Modules

| Module | Chapter | Topic | Key Skills |
|--------|---------|-------|------------|
| 2 | chapter1 | Platform Setup & Readiness | DSCI/DSC configuration, Gateway API, serving runtime selection, operator prerequisites |
| 3 | chapter2 | Governing Access with Models-as-a-Service | MaaS subscriptions, two-tier authentication, token quotas, API key lifecycle, self-service enablement |
| 4 | chapter3 | Scaling Massive Models | Distributed inference with llm-d, Kueue resource queuing, tensor parallelism, WVA autoscaling |
| 5 | chapter4 | Securing Agentic Workflows | Model Context Protocol (MCP), mcp-gateway, EvalHub, garak security scanning, Prompt Guard, TrustyAI Guardrails |
| 6 | chapter5 | Model Catalog, Registry & Storage | Model Registry, OCI Modelcars, immutable distribution, smart connection handling |
| 7 | chapter6 | Hardware Profiles & GPU Performance | Hardware Profiles, MIG vs. time-slicing, DCGM observability, multi-vendor GPU support (NVIDIA/AMD/Intel) |
| 8 | chapter7 | Enabling Rapid Prototyping | Llama Stack distributions, Gen AI Studio & Playground, AI Hub, vector DB integration, RAG |
| 9 | chapter8 | Observability, Monitoring & Showback | Telemetry flow (DCGM/vLLM/OTC), LLM-specific metrics (TTFT/TPOT/KV Cache), financial showback |

## Target Audience

- **Platform Engineers** building or operating OpenShift AI environments
- **AI/ML Infrastructure teams** enabling self-service GenAI for their organizations
- **Solutions Architects** evaluating RHOAI 3.4 capabilities for enterprise AI deployment

### Prerequisites

- Familiarity with OpenShift/Kubernetes administration concepts
- Basic understanding of LLM inference and model serving

## Learning Outcomes

After completing this course, learners will be able to:

- Deploy and configure the full OpenShift AI 3.4 operator stack with proper governance
- Implement Models-as-a-Service with token quotas, showback reporting, and self-service API key management
- Scale massive LLMs across multiple GPUs/nodes using distributed inference (llm-d) and Kueue
- Secure agentic AI workflows using MCP, EvalHub, and defense-in-depth guardrails
- Manage model lifecycle with the Model Registry and immutable OCI Modelcars
- Configure multi-vendor GPU sharing (time-slicing, MIG) with Hardware Profiles
- Stand up rapid prototyping environments with Llama Stack, Gen AI Studio, and the AI Hub
- Build enterprise observability with LLM-specific metrics and financial showback

## Supplemental Resources

The appendix references companion deep-dive repositories for learners who want to go deeper into specific topics:

- **rhoai3-mass2** — Advanced MaaS multi-tenant governance
- **rhoai3-llmd** — llm-d performance tuning (EPP, prefill/decode routing)
- **rhoai3-validate** — TrustyAI Guardrails, red-teaming, ROI calculation
- **rhoai3-gpu-aas** — MIG partition strategies
- **rhoai3-hwprofiles** — Advanced Kueue preemption policies
- **rhoai3-storage** — Storage performance and OCI caching
- **rhoai3-deploy** — Cost modeling and platform maturity
- **rhoai3-journey** — End-to-end learning path (Phases 0-4)

## Building the Course

```bash
# Install dependencies
npm install

# Build the Antora site
npm run build

# View the rendered content
open build/site/index.html
```

## Development

- [Content editing guidelines](./USAGEGUIDE.adoc)
