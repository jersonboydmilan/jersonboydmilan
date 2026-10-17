## Hi, I'm Jerson

Building AI systems, agents, and Physical AI - with a focus on local-first, practical intelligence.

Lately I've been working on authority and safety architecture for autonomous agents: how to let an agent act with real capability without giving it, or an attacker who compromises it, unrestricted power.

### What I'm building

- [Sentinel](https://github.com/jersonboydmilan/Sentinel) - an authority-attenuating immune architecture for AI agents. Detects and contains compromised agents without giving defenders unrestricted authority.
- [Capgate](https://github.com/jersonboydmilan/Capgate) - runtime authority boundary for autonomous AI agents. The agent proposes, the harness authorizes, the executor acts. Deny-by-default policy, non-transitive delegation, tamper-evident audit.
- [Agent-Skills-Compendium](https://github.com/jersonboydmilan/Agent-Skills-Compendium) - an open compendium for discovering, defining, composing, and governing reusable capabilities for AI agents, from digital intelligence to multi-agent systems and Physical AI.
- [QUANTUM-CUDA](https://github.com/jersonboydmilan/QUANTUM-CUDA) - the analysis, runnable verification, and patches behind my NVIDIA CUDA-Q contributions. Every claim is checked against what CUDA-Q actually executes, not transcribed from comments.

### Open-source contributions

**NVIDIA CUDA-Q** ([NVIDIA/cuda-quantum](https://github.com/NVIDIA/cuda-quantum))

- [#5459](https://github.com/NVIDIA/cuda-quantum/pull/5459) (merged) - documented `exp_pauli`, `givens_rotation`, and `fermionic_swap`, and fixed a sign error in the `applyExpPauli` doc comment that every simulator backend inherits.
- [#5609](https://github.com/NVIDIA/cuda-quantum/pull/5609) (merged) - documented how a `qvector` can supply the targets of a custom operation in Python vs C++. In review, the CUDA-Q architect confirmed that an asymmetry it surfaced is a Python bridge bug.
- [#5646](https://github.com/NVIDIA/cuda-quantum/issues/5646), [#5647](https://github.com/NVIDIA/cuda-quantum/issues/5647) (filed on request) - the two Python bridge bugs from that review: single-target custom operations don't broadcast, and multi-target ones pull targets out of a `qvector`.
- [#5608](https://github.com/NVIDIA/cuda-quantum/pull/5608) (in review) - fixed the custom `KrausChannel` example under `cudaq.apply_noise`, which crashes as printed.

**NVIDIA Physical AI Data Factory** ([NVIDIA/physical-ai-data-factory](https://github.com/NVIDIA/physical-ai-data-factory))

- [#22](https://github.com/NVIDIA/physical-ai-data-factory/pull/22) (in review) - fixed a `NameError` crash in the Video Data Augmentation pre-submit guard's model-cache check.

### Focus areas

- Agent authority and permission boundaries
- Multi-agent governance and skill composition
- Physical AI
- Local-first, practical intelligence over hype

### Find me

- Website: https://www.jersonboydmilan.com
