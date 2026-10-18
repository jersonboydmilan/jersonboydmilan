## Hi, I'm Jerson

Building AI systems, agents, and Physical AI - with a focus on local-first, practical intelligence.

Lately I've been working on authority and safety architecture for autonomous agents: how to let an agent act with real capability without giving it, or an attacker who compromises it, unrestricted power.

### What I'm building

- [Sentinel](https://github.com/jersonboydmilan/Sentinel) - an authority-attenuating immune architecture for AI agents. Detects and contains compromised agents without giving defenders unrestricted authority.
- [Capgate](https://github.com/jersonboydmilan/Capgate) - runtime authority boundary for autonomous AI agents. The agent proposes, the harness authorizes, the executor acts. Deny-by-default policy, non-transitive delegation, tamper-evident audit.
- [Agent-Skills-Compendium](https://github.com/jersonboydmilan/Agent-Skills-Compendium) - an open compendium for discovering, defining, composing, and governing reusable capabilities for AI agents, from digital intelligence to multi-agent systems and Physical AI.
- [QUANTUM-CUDA](https://github.com/jersonboydmilan/QUANTUM-CUDA) - the analysis, runnable verification, and patches behind my NVIDIA CUDA-Q contributions: 2 merged PRs, 2 in review, and 2 bridge bugs filed at the architect's request. Every claim is checked against what CUDA-Q actually executes, not transcribed from comments.

### Open-source contributions

**NVIDIA CUDA-Q** ([NVIDIA/cuda-quantum](https://github.com/NVIDIA/cuda-quantum))

- [#5459](https://github.com/NVIDIA/cuda-quantum/pull/5459) (merged) - documented `exp_pauli`, `givens_rotation`, and `fermionic_swap`, and fixed a sign error in the `applyExpPauli` doc comment that every simulator backend inherits.
- [#5609](https://github.com/NVIDIA/cuda-quantum/pull/5609) (merged) - documented how a `qvector` can supply the targets of a custom operation in Python vs C++. In review, the CUDA-Q architect confirmed that an asymmetry it surfaced is a Python bridge bug.
- [#5646](https://github.com/NVIDIA/cuda-quantum/issues/5646), [#5647](https://github.com/NVIDIA/cuda-quantum/issues/5647) (filed on request) - the two Python bridge bugs from that review: single-target custom operations don't broadcast, and multi-target ones pull targets out of a `qvector`. The architect has since settled #5647's direction: the conflicting proposal #2484 should not be implemented.
- [#5649](https://github.com/NVIDIA/cuda-quantum/pull/5649) (in review) - fix for #5646: single-target custom operations now broadcast over a `qvector` and over several qubits, in plain and `.adj` calls, matching the built-in gates and the C++ bridge. Verified on the real CUDA-Q 0.16.0 runtime: the PR's tests go from 26/30 to 30/30 with no regressions. The architect's reply to its out-of-scope section laid down the DSL's operation-overload rules for both Python and C++.
- [#5608](https://github.com/NVIDIA/cuda-quantum/pull/5608) (in review) - fixed the custom `KrausChannel` example under `cudaq.apply_noise`, which crashes as printed.

**NVIDIA Physical AI Data Factory** ([NVIDIA/physical-ai-data-factory](https://github.com/NVIDIA/physical-ai-data-factory))

- [#22](https://github.com/NVIDIA/physical-ai-data-factory/pull/22) (in review) - fixed a `NameError` crash in the Video Data Augmentation pre-submit guard's model-cache check.

**Microsoft Agent Governance Toolkit** ([microsoft/agent-governance-toolkit](https://github.com/microsoft/agent-governance-toolkit))

- [#4346](https://github.com/microsoft/agent-governance-toolkit/pull/4346) (in review) - a 240-scenario red-team measurement suite scoring real detector catch/miss rate against canonical and evasion prompt-injection probes, without weakening the existing hard release gate.

**AgentKit** ([orka-agents/agentkit](https://github.com/orka-agents/agentkit))

- [#71](https://github.com/orka-agents/agentkit/pull/71) (merged) - `x-`/`X-` extension field prefixes for the Agentkitfile (Docker Compose/OpenAPI convention), so a value can be defined once behind an `x-` field and reused elsewhere via a YAML anchor.

**guardrail** ([FvdHMBAI/guardrail](https://github.com/FvdHMBAI/guardrail))

- [#52](https://github.com/FvdHMBAI/guardrail/pull/52) (in review) - `docker_container_guard`, a pre-bash hook blocking `docker run`/`docker create` with flags that break container isolation: `--privileged`, host network/PID namespace, host-root bind mounts.

**RepoLens** ([deswanth12/repolens](https://github.com/deswanth12/repolens))

- [#5](https://github.com/deswanth12/repolens/pull/5) (in review) - a `--schema` flag exporting the JSON Schema for RepoLens' machine-readable report, so tool integrators and AI agents can validate output without reverse-engineering the models.

### Focus areas

- Agent authority and permission boundaries
- Multi-agent governance and skill composition
- Physical AI
- Local-first, practical intelligence over hype

### Find me

- Website: https://www.jersonboydmilan.com
