# Ruslan Vrublevskyi

**AI-Native Systems Architect · Creator of EvidenceBound · Founder of SignalReview**

[EvidenceBound](https://evidencebound.org) · `ruslan@evidencebound.org` · [LinkedIn](https://www.linkedin.com/in/ruslan-vrublevskyi) · [ORCID](https://orcid.org/0009-0004-2468-5232)

I design agentic AI systems that fail closed when evidence, dependencies, integrity, or policy state can no longer be trusted.

My work spans deterministic verification, bounded execution, tamper-evident Proof Packs, verifiable memory, trust-graph recovery, multi-agent orchestration, security boundaries, CI/CD, and production acceptance.

Based in Kyiv, Ukraine. Open to research/consortium collaboration around trustworthy agentic systems and to remote AI systems architecture, applied AI, agent platform, verification, and technical product engineering roles.

## EvidenceBound architecture

**Institutional site:** https://evidencebound.org  
**Canonical OSS core:** https://github.com/moneyparking/evidencebound-core  
**Project contact:** ruslan@evidencebound.org

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

## Selected public implementations

| Project | Architectural problem | Verified implementation |
|---|---|---|
| [EvidenceBound Core](https://github.com/moneyparking/evidencebound-core) | Bind agent state to evidence/provenance/policy and recover selectively after trust changes | Framework-agnostic Python runtime, deterministic verification, dependency blast-radius analysis, fail-closed selective recovery, signed-receipt and persistence seams, conformance corpus, supply-chain attestations |
| [EvidenceBound Recovery Mesh](https://github.com/moneyparking/evidencebound-recovery-mesh) | Recover an agent fleet after one checkpoint becomes untrustworthy without restarting safe work | Google ADK, Vertex AI / Gemini 3.5 Flash, Cloud Run, Agent Registry, Secret Manager, Workload Identity Federation, Trust Graph blast-radius analysis, fail-closed action gate, selective recomputation |
| [EvidenceBound DataHub Gate](https://github.com/moneyparking/evidencebound-datahub-gate) | Decide whether an agent-generated data action is bound to current metadata before human review | Official DataHub MCP, schema and bounded-lineage binding, Restricted AST Policy, no-`exec` bounded interpreter, SHA-256 Proof Packs, Ed25519 seals, native DataHub description write-back |
| [EvidenceBound Verified Memory](https://github.com/moneyparking/moneyparking-evidencebound-verified-memory) | Reopen prior agent state and prove what changed rather than merely recalling an answer | CockroachDB persistence, canonical snapshots, integrity verification, T0 → T1 comparison, AWS Lambda, S3, CloudFormation, GitHub OIDC → AWS STS |
| [Governed Codex Module Factory](https://devpost.com/software/signalreview-autonomous-multi-agent-ai) | Generate analytics modules without granting generated code automatic deployment authority | Codex workflow, isolated execution, validation gates, sealed review artifacts, mandatory human review |
| [Forensic Multi-Agent Sports Intelligence](https://github.com/moneyparking/Signalreview-Alibaba-Qwen) | Produce a bounded verdict from adversarial agent roles without inventing unavailable provider facts | Qwen Cloud, four-role evidence-first review, visible missing-data states, orchestrated bounded verdict |
| [SignalReview](https://signalreview.co) | Turn structured match evidence into a retained, transparent decision-support workflow | Next.js, TypeScript, React, Python, FastAPI, PostgreSQL, Supabase, Docker, GitHub Actions, Vercel, Render, Cloudflare |

### Recovery Mesh production evidence

A controlled production run compared a full restart with selective recovery:

- full restart: 4 model calls / 1,781 input tokens;
- selective recovery: 3 model calls / 1,358 input tokens;
- saved in that exact run: 1 model call / 423 input tokens (~24%).

This is a measured result from one controlled run, not a universal savings claim. The current bounded Cloud Run slice does not claim durable multi-week memory.

### DataHub reproducibility

```bash
git clone https://github.com/moneyparking/evidencebound-datahub-gate.git
cd evidencebound-datahub-gate
make test-repro
```

Expected retained states include:

```text
VERIFIED
BLOCKED: SCHEMA_MISMATCH
REPRODUCED
ARTIFACT_TAMPERING_DETECTED
SIGNATURE_VALID
```

`VERIFIED` is deliberately narrow. It does not mean production authorization, data truth, certification, or permission to deploy.

## Architecture and engineering focus

- AI-native systems and agent platform architecture
- Agentic AI, MCP, Google ADK, OpenAI, and Qwen Cloud
- Deterministic runtimes, restricted execution, and fail-closed controls
- Verification contracts, canonicalization, provenance, and content addressing
- Verifiable memory, dependency graphs, invalidation, and selective recovery
- Python, TypeScript, Next.js, React, FastAPI, Pydantic, SQL
- PostgreSQL, Supabase, CockroachDB, AWS, Google Cloud, Vercel, Render, Cloudflare
- Docker, GitHub Actions, OIDC/WIF, pytest, Ruff, Mypy, security and release gates
- Product strategy, monetization, QA, deployment, and production acceptance

## Public evidence

- [EvidenceBound institutional site](https://evidencebound.org)
- [EvidenceBound Core](https://github.com/moneyparking/evidencebound-core)
- [Canonical professional profile](https://signalreview.co/about/ruslan-vrublevskyi)
- [Machine-readable identity](https://signalreview.co/identity/ruslan-vrublevskyi.json)
- [LinkedIn](https://www.linkedin.com/in/ruslan-vrublevskyi)
- [ORCID](https://orcid.org/0009-0004-2468-5232)
- [EvidenceBound-MAS whitepaper](https://signalreview.co/docs/EvidenceBound_MAS_Verifiable_Evidence_for_Human_Decision_Making_2026.pdf)
- [Recovery Mesh on Devpost](https://devpost.com/software/evidencebound-recovery-mesh)
- [DataHub Gate on Devpost](https://devpost.com/software/evidencebound-datahub-gate)
- [Verified Memory on Devpost](https://devpost.com/software/evidencebound-verified-memory)

For EvidenceBound research, OSS, security and consortium work: **ruslan@evidencebound.org**.

Public materials intentionally exclude private repositories, credentials, customer information, personal address, and telephone number.
