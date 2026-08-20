# Technology Radar

Based on an ecosystem-wide analysis, the following technologies, tools, and frameworks have been categorized for current and future projects.

## Adopt (Proven & Standardized)
These technologies are widely adopted across the ecosystem and should be chosen by default for new projects in their respective domains.

- **Languages**: 
  - `TypeScript/JavaScript` (14+ projects) - Standard for front-end and full-stack web.
  - `Python` (11+ projects) - Standard for data, ML, backend scripts, and RAG architectures.
  - `HTML/CSS` (16+ projects) - Ubiquitous for UI.
- **Frameworks/Platforms**:
  - `Node.js` (11+ projects) - Default JavaScript runtime.
  - `Docker` (7+ projects) - Standardized containerization for services.
  - `Godot` (GDScript) - Default engine for 2D/3D games and interactive apps.

## Trial (Experimenting with Success)
Technologies that are showing great promise and have been integrated into multiple advanced projects.

- **MCP (Model Context Protocol)** (7 projects)
  - Heavily used in AI integrations (`AIWF-POC`, `blender_mcp`, `Brad-RAG`, `jx-mcp`, `godot-mcp`, `PublisherPotato-Demo`).
  - Represents a shift towards composable AI agents and tool use. Future AI-centric projects should natively support MCP.
- **Go / Go Modules** (3 projects)
  - Used for performance-critical backends (`AIWF-GO`, `GT7-RaceEngineer`, `RaceRox`). Great for microservices.
- **Next.js**
  - Observed in full-stack setups (`osiris`, `ProjectPotato`) indicating a shift towards SSR/SSG React architectures.

## Assess (Niche or Emerging)
Technologies used for specific use-cases that don't apply universally but require specialized knowledge.

- **C/C++** (5 projects)
  - Crucial for embedded systems firmware (`ByteBoi-Firmware`) and low-level performance (`RaceRox`).
- **Unity / C#**
  - Found in `PMC` for robust 3D/physics simulations. Competing with Godot for game engine share.

## Hold (Avoid or Deprecate)
*(None explicitly identified in the scan, though older, unmaintained projects may naturally fall off.)*
