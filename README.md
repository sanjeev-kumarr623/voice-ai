# Voice AI: End-to-End Voice Orchestration Platform

An open-source voice AI orchestration platform designed for agencies needing full ownership and enterprises requiring scale, control, and deploy-anywhere flexibility.  

It is built around three core principles:

- **Ownership** — run managed or self-hosted while keeping control of data, credentials, branding, and deployment boundaries.
- **Control** — choose your models, prompts, tools, and integrations without vendor lock-in.
- **Scale** — operate real-time voice workloads with observability, governance, and production-grade reliability.

This project provides both a **platform** and a **framework** for teams building white-label client deployments, internal AI operations, and enterprise voice infrastructure.

The core services are written in **Go**, utilizing the highly optimized [gRPC](https://github.com/grpc/grpc-go) protocol for fast, efficient, bidirectional communication.

---

## Features

- **Real-time Voice Orchestration**  
  Stream and process audio with low latency using gRPC.

- **Ownership by Default**  
  Self-host or run managed while keeping control of infrastructure, credentials, and runtime behavior.

- **Provider and Model Control**  
  Bring your own model—OpenAI, Anthropic, open-source models, or custom inference.

- **Production-grade Reliability**  
  Built-in retries, error handling, call lifecycle management, and health checks.

- **Full Observability**  
  Call logs, streaming events, tool traces, latency breakdowns, metrics, and dashboards.

- **Governance-ready Tooling**  
  Build custom tools, lock down API surfaces, and manage deployments with audit-friendly controls.

- **Built for Agencies and Enterprise**  
  Support multi-client delivery, private deployments, and large-scale internal operations from the same platform.

---

## Prerequisites

- **Docker** & **Docker Compose** ([Install](https://www.docker.com/))
- **Just** command runner ([Install](https://github.com/casey/just#installation))
- **Go 1.26+**, **Node.js 22**, and **Yarn 1.22+** for `just ci`
- **16GB+ RAM** (for running all services concurrently)

---

## Quick Start

Get all services running in 4 commands:

```bash
# Clone repo
git clone [https://github.com/sanjeev-kumarr623/voice-ai.git](https://github.com/sanjeev-kumarr623/voice-ai.git) && cd voice-ai

# Setup & build
just setup-local build-all

# Start all services
just up-all

# View running services
docker compose ps
