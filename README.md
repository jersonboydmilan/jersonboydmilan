<div align="center">

# Jerson Boyd Milan

**AI systems, autonomous agents, and Physical AI — local-first, practical intelligence.**

[![Website](https://img.shields.io/badge/jersonboydmilan.com-000000?style=flat&logo=googlechrome&logoColor=white)](https://www.jersonboydmilan.com)
[![CUDA-Q contributor](https://img.shields.io/badge/NVIDIA_CUDA--Q-contributor-76B900?style=flat&logo=nvidia&logoColor=white)](https://github.com/NVIDIA/cuda-quantum/pulls?q=author%3Ajersonboydmilan)
[![Open-source PRs](https://img.shields.io/badge/open--source-PRs-24292f?style=flat&logo=github&logoColor=white)](https://github.com/pulls?q=author%3Ajersonboydmilan+is%3Apr+-user%3Ajersonboydmilan)

</div>

I build agent systems that can act with real capability **without** handing the agent, or an attacker who compromises it, unrestricted power. Most of my time goes into authority and safety architecture for autonomous agents, and into upstream fixes for the open-source tools I build on.

### Now

- Designing **authority boundaries** for agents: deny-by-default policy, non-transitive delegation, tamper-evident audit.
- Contributing to **NVIDIA CUDA-Q**: docs fixes and Python bridge fixes, each verified against the real runtime.
- Exploring **Physical AI** data pipelines and agent tooling.

---

### Featured projects

<table>
<tr>
<td width="50%" valign="top">

**[Sentinel](https://github.com/jersonboydmilan/Sentinel)**<br>
An authority-attenuating immune architecture for AI agents. Detects and contains compromised agents without giving defenders unrestricted authority.<br>
<sub>Python · agent security</sub>

</td>
<td width="50%" valign="top">

**[Capgate](https://github.com/jersonboydmilan/Capgate)**<br>
A runtime authority boundary for autonomous agents: the agent proposes, the harness authorizes, the executor acts. Deny-by-default policy, non-transitive delegation, tamper-evident audit.<br>
<sub>Python · MCP gateway · isolation</sub>

</td>
</tr>
<tr>
<td width="50%" valign="top">

**[Agent-Skills-Compendium](https://github.com/jersonboydmilan/Agent-Skills-Compendium)**<br>
An open registry of fully specified AI agent skills, with taxonomy, canonical schema, composer, governance model, and a fleet runner.<br>
<sub>TypeScript · multi-agent systems</sub>

</td>
<td width="50%" valign="top">

**[QUANTUM-CUDA](https://github.com/jersonboydmilan/QUANTUM-CUDA)**<br>
The analysis, runnable verification, and patches behind my CUDA-Q contributions. Every claim is checked against what CUDA-Q actually executes, not transcribed from comments.<br>
<sub>Python · quantum computing</sub>

</td>
</tr>
</table>

---

### Open-source contributions

Status badges are live and update as PRs are reviewed.

| Project | Contribution | Status |
| :--- | :--- | :--- |
| **[NVIDIA CUDA-Q](https://github.com/NVIDIA/cuda-quantum)** | Documented `exp_pauli`, `givens_rotation` and `fermionic_swap`, and fixed a sign error in the `applyExpPauli` doc comment every simulator backend inherits | [![#5459](https://img.shields.io/github/pulls/detail/state/NVIDIA/cuda-quantum/5459?label=%235459)](https://github.com/NVIDIA/cuda-quantum/pull/5459) |
| | Documented `qvector` targets for custom ops in Python vs C++. Its review led the architect to state the DSL's overload rules; the maintainers then removed the Python-only behavior in #5652 | [![#5609](https://img.shields.io/github/pulls/detail/state/NVIDIA/cuda-quantum/5609?label=%235609)](https://github.com/NVIDIA/cuda-quantum/pull/5609) |
| | Fixed the custom `KrausChannel` example under `cudaq.apply_noise`, which crashes as printed | [![#5608](https://img.shields.io/github/pulls/detail/state/NVIDIA/cuda-quantum/5608?label=%235608)](https://github.com/NVIDIA/cuda-quantum/pull/5608) |
| | Single-target broadcast for custom operations ([#5646](https://github.com/NVIDIA/cuda-quantum/issues/5646)), verified on the real runtime; direction under discussion after #5652 | [![#5649](https://img.shields.io/github/pulls/detail/state/NVIDIA/cuda-quantum/5649?label=%235649)](https://github.com/NVIDIA/cuda-quantum/pull/5649) |
| | Made the Observe examples on "Executing Kernels" runnable on their own ([#3409](https://github.com/NVIDIA/cuda-quantum/issues/3409)) | [![#5655](https://img.shields.io/github/pulls/detail/state/NVIDIA/cuda-quantum/5655?label=%235655)](https://github.com/NVIDIA/cuda-quantum/pull/5655) |
| | "Building Kernels" now shows the state each example prepares instead of a bare call ([#3384](https://github.com/NVIDIA/cuda-quantum/issues/3384)) | [![#5658](https://img.shields.io/github/pulls/detail/state/NVIDIA/cuda-quantum/5658?label=%235658)](https://github.com/NVIDIA/cuda-quantum/pull/5658) |
| **[NVIDIA Physical AI Data Factory](https://github.com/NVIDIA/physical-ai-data-factory)** | Fixed a `NameError` crash in the Video Data Augmentation pre-submit guard's model-cache check | [![#22](https://img.shields.io/github/pulls/detail/state/NVIDIA/physical-ai-data-factory/22?label=%2322)](https://github.com/NVIDIA/physical-ai-data-factory/pull/22) |
| **[Microsoft Agent Governance Toolkit](https://github.com/microsoft/agent-governance-toolkit)** | A 240-scenario red-team measurement suite that scores real detector catch/miss rates on canonical and evasion prompt-injection probes | [![#4346](https://img.shields.io/github/pulls/detail/state/microsoft/agent-governance-toolkit/4346?label=%234346)](https://github.com/microsoft/agent-governance-toolkit/pull/4346) |
| **[AgentKit](https://github.com/orka-agents/agentkit)** | `x-`/`X-` extension fields in the Agentkitfile, so values can be defined once and reused through YAML anchors | [![#71](https://img.shields.io/github/pulls/detail/state/orka-agents/agentkit/71?label=%2371)](https://github.com/orka-agents/agentkit/pull/71) |
| | Every Agentkitfile validation error names its file and line, and carries a BuildKit source location so Docker shows the surrounding lines | [![#75](https://img.shields.io/github/pulls/detail/state/orka-agents/agentkit/75?label=%2375)](https://github.com/orka-agents/agentkit/pull/75) |
| **[guardrail](https://github.com/FvdHMBAI/guardrail)** | `docker_container_guard`: blocks `docker run`/`create` flags that break container isolation | [![#52](https://img.shields.io/github/pulls/detail/state/FvdHMBAI/guardrail/52?label=%2352)](https://github.com/FvdHMBAI/guardrail/pull/52) |
| **[RepoLens](https://github.com/deswanth12/repolens)** | A `--schema` flag exporting the JSON Schema of the machine-readable report | [![#5](https://img.shields.io/github/pulls/detail/state/deswanth12/repolens/5?label=%235)](https://github.com/deswanth12/repolens/pull/5) |

<sub>Also filed on request of the CUDA-Q architect: Python bridge bugs [#5646](https://github.com/NVIDIA/cuda-quantum/issues/5646) and [#5647](https://github.com/NVIDIA/cuda-quantum/issues/5647). #5647 is now resolved on `main` by #5652.</sub>

---

### How I work

- **Verify, don't transcribe.** Every claim in a PR is checked against what the code actually does, using the real runtime, a reproducer, or a numerical check, and the script goes into the repo.
- **Small, reviewable changes.** One concern per PR, history traced through the linked issues, and open questions left to the maintainers instead of settled unilaterally.
- **Honest scope.** What I couldn't verify is stated in the PR, not glossed over.

### Focus areas

`Agent authority & permission boundaries` · `Multi-agent governance` · `Skill composition` · `Physical AI` · `Local-first AI`

---

<div align="center">
<sub><a href="https://www.jersonboydmilan.com">jersonboydmilan.com</a></sub>
</div>
