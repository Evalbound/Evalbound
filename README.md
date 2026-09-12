# Ruslan Vrublevskyi

**AI Systems Architect | AI Solutions Architect | Agentic AI · LLM Systems · Verification | Technical Advisor**

Creator of [EvidenceBound](https://evidencebound.org) · Founder of [SignalReview](https://signalreview.co)

[LinkedIn](https://www.linkedin.com/in/ruslan-vrublevskyi) · [ORCID](https://orcid.org/0009-0004-2468-5232) · `ruslan@evidencebound.org`

I design and build AI and agentic systems that need clear trust boundaries, reproducible evidence, controlled execution, and recoverable failure handling.

My work focuses on moving LLM prototypes into operable systems: system architecture, MCP-based tool use, deterministic verification, provenance, policy-as-code, failure containment, recovery, and human approval boundaries.

I am interested in remote **AI Systems Architect, AI Solutions Architect, Agentic AI Architect, Software Architect, and Technical Advisor** roles where the challenge is turning promising AI capabilities into reliable systems.

## Selected public engineering

| Project | What it demonstrates |
|---|---|
| [EvidenceBound Core](https://github.com/evidencebound/evidencebound-core) | Framework-agnostic deterministic verification, evidence/provenance/policy-bound state, dependency invalidation, selective recovery, signed-receipt and persistence seams |
| [EvidenceBound Recovery Mesh](https://github.com/evidencebound/evidencebound-recovery-mesh) | Multi-agent recovery after trust changes, dependency blast-radius analysis, fail-closed action gates, selective recomputation |
| [EvidenceBound Authority Cut](https://github.com/evidencebound/evidencebound-authority-cut) | Human authority kept outside the model-callable surface, grant/revoke boundaries, correction propagation, reversible compensation |
| [EvidenceBound DataHub Gate](https://github.com/moneyparking/evidencebound-datahub-gate) | MCP-based Read → Verify → Write-Back governance, VERIFIED/BLOCKED paths, reproducible Proof Packs, mandatory human review |
| [EvidenceBound Verified Memory](https://github.com/moneyparking/moneyparking-evidencebound-verified-memory) | Persisted verified decisions, historical-integrity checks, T0 → T1 evidence comparison, current-applicability re-evaluation with CockroachDB and AWS |
| [SignalReview / Qwen Agent Society](https://github.com/moneyparking/Signalreview-Alibaba-Qwen) | Four-role adversarial agent workflow, structured output validation, visible unavailable domains, bounded verdicts and fail-closed handling |

## EvidenceBound control pattern

EvidenceBound is a systems approach for making AI-generated actions inspectable, reproducible, challengeable, and blockable.

```text
Current evidence
      ↓
Deterministic verification
      ↓
Tamper-evident proof
      ↓
Verifiable memory
      ↓
Trust-break detection
      ↓
Selective recovery
      ↓
Mandatory human or policy-controlled decision
```

The LLM may interpret bounded evidence. It does not grant itself trust, hide unavailable inputs, override deterministic gates, or authorize unsafe side effects.

## Architecture and engineering focus

- AI systems and agent platform architecture
- Agentic AI, LLM systems, MCP, Google ADK, OpenAI, Qwen Cloud
- Deterministic runtimes, restricted execution, and fail-closed controls
- Verification contracts, provenance, canonicalization, and content addressing
- Verifiable memory, dependency graphs, invalidation, and selective recovery
- Python, TypeScript, Next.js, React, FastAPI, Pydantic, SQL
- PostgreSQL, Supabase, CockroachDB, AWS, Google Cloud, Vercel, Render, Cloudflare
- Docker, GitHub Actions, OIDC/WIF, pytest, Ruff, Mypy, security and release gates
- Product strategy, QA, deployment, release acceptance, and commercialization planning

## Public evidence

- [EvidenceBound institutional site](https://evidencebound.org)
- [EvidenceBound GitHub organization](https://github.com/evidencebound)
- [EvidenceBound Core](https://github.com/evidencebound/evidencebound-core)
- [EvidenceBound Recovery Mesh](https://github.com/evidencebound/evidencebound-recovery-mesh)
- [EvidenceBound Authority Cut](https://github.com/evidencebound/evidencebound-authority-cut)
- [EvidenceBound ReleaseProof](https://github.com/evidencebound/evidencebound-releaseproof-dws)
- [EvidenceBound DataHub Gate](https://github.com/moneyparking/evidencebound-datahub-gate)
- [EvidenceBound Verified Memory](https://github.com/moneyparking/moneyparking-evidencebound-verified-memory)
- [SignalReview / Qwen](https://github.com/moneyparking/Signalreview-Alibaba-Qwen)
- [EvidenceBound maintainer profile](https://evidencebound.org/#maintainer)
- [Machine-readable identity](https://evidencebound.org/identity/ruslan-vrublevskyi.json)
- [Historical EvidenceBound-MAS whitepaper](https://signalreview.co/docs/EvidenceBound_MAS_Verifiable_Evidence_for_Human_Decision_Making_2026.pdf)

Public materials intentionally exclude private repositories, credentials, customer information, personal address, telephone number, and transient location.
