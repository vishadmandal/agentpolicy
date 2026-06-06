# Contributing to agentpolicy

Thank you for your interest. This project is in early spec phase — contributions to the spec are as valuable as code contributions right now.

---

## What We Need Most (Right Now)

### 1. Spec Feedback
Read `spec/APS_v0.1.md` and open an issue if:
- A concept is unclear or ambiguous
- A real-world use case isn't covered
- The token schema has a flaw
- The delegation model has a security gap

This is the most valuable contribution at this stage. The spec shapes everything downstream.

### 2. Real-World Policy Examples
If you run agents in production, sharing anonymized policy examples (what tools your agents need, what they should never do) helps make the spec practical rather than theoretical.

Add them to `policies/examples/` as a PR.

### 3. Security Review
The injection defense model and delegation chain trust propagation need adversarial review. If you work in security, please open issues with attack scenarios we haven't considered.

### 4. Framework Adapter Interest
If you maintain or heavily use LangGraph, CrewAI, LlamaIndex, AutoGen, or any other agentic framework and want to discuss native APS support, open an issue tagged `adapter-request`.

---

## Issue Types

Use the issue templates:

- **Spec Feedback** — questions, ambiguities, gaps in the spec
- **Policy Example** — share a real-world policy pattern
- **Adapter Request** — request or propose a framework adapter
- **Security Issue** — attack vectors or model flaws (use private disclosure for serious vulnerabilities)
- **Bug** — only relevant once the SDK ships in v0.2

---

## Pull Request Guidelines

### For spec changes (`spec/`)
- Open an issue first to discuss the change
- Spec PRs require at least 2 approvals
- Breaking changes to the schema require a version bump discussion

### For policy examples (`policies/examples/`)
- Anonymize any real company/system names
- Include a comment explaining the use case context
- Must be valid YAML

### For SDK code (`sdk/`) — available in v0.2
- Follow existing code style
- Include tests
- Update the relevant adapter docs

---

## Code of Conduct

Be direct, be constructive, assume good intent. Technical disagreements are welcome. Personal attacks are not.

---

## License

By contributing, you agree your contributions are licensed under Apache 2.0.
