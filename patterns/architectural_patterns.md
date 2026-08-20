# Architectural Patterns

By analyzing the ecosystem, several distinct architectural and design patterns have emerged. These patterns should be referenced when bootstrapping new projects to ensure consistency and maintainability.

## 1. The Monorepo Workspace (Turbo/NX style)
**Description:**
Complex projects are partitioned into monorepos with an `apps/` and `packages/` structure.
- **`apps/`**: Contains deployable applications (e.g., `web`, `api`, `blockchain-indexer`).
- **`packages/`**: Contains shared libraries and modules (e.g., `common`, `database`, `contracts`, `types`).
**Benefit:** Easier dependency management, shared tooling, and unified CI/CD for complex, multi-service systems.

## 2. MCP-Enabled Agentic Architecture
**Description:**
Systems are being designed not just for human users, but for AI agents. This is achieved by implementing the **Model Context Protocol (MCP)**.
- Services expose tools and context via MCP servers.
- Examples include integrating Godot engines or Blender rendering pipelines with LLMs.
**Benefit:** Makes existing software domains immediately programmable and accessible to agentic AI assistants.

## 3. Containerized Microservices
**Description:**
Backend systems are built using Docker to isolate services. Often, different services are written in different languages optimized for the task (e.g., Go for high-throughput APIs, Python for data/ML processing).
**Benefit:** Scalability, language-agnostic orchestration, and reproducible environments.

## 4. Headless API + Modern Frontend
**Description:**
A clean separation between a backend data layer (Go, Python) and a rich, interactive frontend layer (React, Next.js, HTML/TS).
**Benefit:** Teams can iterate on UI/UX without impacting core business logic.
