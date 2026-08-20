# Agentic Work Patterns

As AI-assisted software delivery evolves in the ecosystem, standardizing how human and AI agents collaborate is essential. These patterns are extracted from repository rule sets (`AGENTS.md`) and successful delivery histories.

## 1. Multi-Agent Delegation Strategy
**Description:** Separating concerns among different LLMs or sub-agents improves quality and prevents conflicting edits.
- **Implementation Agent**: Focuses strictly on writing production code, adhering to existing architecture, and adding tests.
- **Review/Testing Agent (Principal Engineer role)**: Reviews implementation branches, writes test plans, validates edge cases, and checks against architecture boundaries.
- **Planner Agent**: Breaks down large projects into structured milestone task packets.

## 2. Iterative Delivery & Thin Vertical Slices
**Description:** Breaking down large projects into smaller, verifiable phases. 
- Prefer "thin vertical slices" over broad, unfinished scaffolding to deliver minimal value and test assumptions early.
- Perform frequent commits and pushes at points of value. This ensures progress is preserved and makes rollback easier if an AI agent hallucinates or takes a wrong architectural turn.

## 3. Strict Definition of Done (DoD) & Verification
**Description:** AI-generated code must not be merged or considered complete without rigorous verification.
- Output must explicitly list assumptions, consumed inputs, and open questions.
- Deterministic testing must accompany the code changes.
- Security assessments and architectural reviews must be performed before major PRs are accepted.

## 4. Continuous Documentation Maintenance
**Description:** Documentation is the ultimate source of truth for agents.
- Agents must update the project state, decision logs (ADRs), and schemas whenever contracts change.
- Never rely solely on chat history; write state to Markdown specs so future agents have the correct context.
