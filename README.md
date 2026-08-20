# AI Factory Core

Welcome to the **AI Factory Core** repository. This project serves as a centralized knowledge base, extracting the patterns, skills, tools, and roles from the broader ecosystem of projects within this environment.

By cataloging the diverse range of software architectures and technologies, this repository acts as a springboard for accelerating the development of future projects.

## Directory Structure

- `/knowledge` - Technology radar and overarching domain insights (Game Dev, AI, Embedded, Web).
- `/patterns` - Architectural and design patterns observed across multiple codebases (e.g., Monorepos, MCP architectures).
- `/roles` - Personas and roles required to support the tech stack effectively.
- `/skills` - The specific programming skills and tool competencies needed for future endeavors.

## Ecosystem Overview

An analysis of over 50 projects in the adjacent directories reveals a highly diverse software environment. 

### Key Domains
- **AI & Automation**: Extensive use of Model Context Protocol (MCP) in tooling, demonstrating a focus on Agentic AI integration.
- **Web Applications**: Modern web apps built with Node.js and frameworks like Next.js.
- **Game Development**: Simulation and game projects leveraging both Godot (GDScript) and Unity (C#).
- **Backend Services**: High-performance services powered by Go and Python ecosystems.
- **Embedded Systems**: Low-level embedded C/C++ (e.g., ByteBoi firmware).

Leverage the artifacts in this repository to standardize approaches and rapidly onboard AI agents or developers to new projects!

## How to Bootstrap a New Project

When spinning up a new project in the ecosystem, follow these steps to leverage the AI Factory Core:

1. **Establish the Documentation Scaffold**
   - Copy the required 14-part file structure defined in [`patterns/standard_project_docs.md`](patterns/standard_project_docs.md) into your new project's root.
   - Flesh out the `01_Project_Overview.md` and `02_Product_PRD.md` to ground human and AI contributors.

2. **Configure Your Agents**
   - Copy [`patterns/agent_configuration_template.yaml`](patterns/agent_configuration_template.yaml) to the root of your new project as `.agent-config.yaml`.
   - Modify it to assign the correct LLMs (e.g., Gemini 1.5 Pro, Codex) and execution frameworks for the specific roles your project requires.

3. **Align on Architecture and Tech Stack**
   - Consult the [`knowledge/technology_radar.md`](knowledge/technology_radar.md) to choose approved frameworks (e.g., Next.js, Godot, Go Modules).
   - Review [`patterns/architectural_patterns.md`](patterns/architectural_patterns.md) to align on structures like Monorepos or Agentic MCP integrations.

4. **Define Team Roles and Workflows**
   - Reference [`roles/roles_and_personas.md`](roles/roles_and_personas.md) and [`skills/required_skills.md`](skills/required_skills.md) to determine if you need to hire human engineers or configure specific AI sub-agents (e.g., an MCP Integration Specialist vs. a Principal Review Agent).
   - Adopt the iterative delivery and testing strategies from [`patterns/agentic_work_patterns.md`](patterns/agentic_work_patterns.md).

5. **Enforce Engineering Hygiene**
   - Ensure the new project implements the logging, CI/CD, testing, and Conventional Commit standards laid out in [`patterns/hygiene_and_standards.md`](patterns/hygiene_and_standards.md).
