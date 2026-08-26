# David Nichols

**Building systems that have to be right on real hardware.** 17. Edge-first. The work lives at the boundary where a model's opinion stops and an auditable decision has to be made.

[![GitHub](https://img.shields.io/badge/GitHub-davidnichols--ops-181717?logo=github)](https://github.com/davidnichols-ops)
[![HuggingFace](https://img.shields.io/static/v1?label=%F0%9F%A4%97+HuggingFace&message=davidnichols--ops&color=yellow)](https://huggingface.co/davidnichols-ops)
[![X](https://img.shields.io/badge/follow-%40davidnicholsops-000000?logo=x)](https://x.com/davidnicholsops)

---

## Open-source contributions

I open PRs upstream when the fix is general. Some merge, some don't. Here's the full record.

### Merged

| Date | Repo | PR | What |
|------|------|----|------|
| 2026-08-25 | huggingface/peft | [#3603](https://github.com/huggingface/peft/pull/3603) | Troubleshooting section for hybrid architecture target_modules |
| 2026-07-06 | tensorflow/tensorflow | [#122706](https://github.com/tensorflow/tensorflow/pull/122706) | XLA DenseBincount negative input validation for runtime tensors |
| 2026-07-02 | ultralytics/ultralytics | [#25020](https://github.com/ultralytics/ultralytics/pull/25020) | Exclude Sigmoid from TensorRT INT8 quantization |
| 2026-06-30 | roboflow/roboflow-python | [#502](https://github.com/roboflow/roboflow-python/pull/502) | Return single_upload result from Project.upload() |
| 2026-06-30 | roboflow/roboflow-python | [#501](https://github.com/roboflow/roboflow-python/pull/501) | Relax opencv-python-headless pin to >=4.10.0 |
| 2026-07-12 | inceptyon-labs/gargantua | [#6](https://github.com/inceptyon-labs/gargantua/pull/6) | Fix singular byte formatting in AlertItem.formatBytes |
| 2026-07-12 | Lcharvol/MacSift | [#12](https://github.com/Lcharvol/MacSift/pull/12) | Fix case-sensitive path matching in iOS backup description |
| 2026-07-12 | haukesomm/apple-photos-export | [#14](https://github.com/haukesomm/apple-photos-export/pull/14) | Fix README typos: Sequoia, always |
| 2026-07-12 | thaw-app/Thaw | [#775](https://github.com/thaw-app/Thaw/pull/775) | Fix typo and IceBar references in URI schemes |
| 2026-07-12 | everettjf/atosl-rs | [#15](https://github.com/everettjf/atosl-rs/pull/15) | Add C++ demangling and non-mangled passthrough tests |
| 2026-07-12 | tuna-f1sh/cyme | [#122](https://github.com/tuna-f1sh/cyme/pull/122) | Fix typos in doc comments |
| 2026-07-12 | jackson-storm/DynamicNotch | [#145](https://github.com/jackson-storm/DynamicNotch/pull/145) | Fix incorrect alt text for gallery images in README |

### Open

| Date | Repo | PR | What |
|------|------|----|------|
| 2026-08-24 | npm/rfcs | [#917](https://github.com/npm/rfcs/pull/917) | RFC: install trust audit — classified fetch telemetry for package publishers |
| 2026-08-23 | roboflow/inference | [#2844](https://github.com/roboflow/inference/pull/2844) | Resolve Model through the lazy package init |
| 2026-08-20 | roboflow/inference | [#2834](https://github.com/roboflow/inference/pull/2834) | Clear every touched namespace in cache blocks (refcounted ownership) |
| 2026-08-17 | huggingface/transformers | [#48022](https://github.com/huggingface/transformers/pull/48022) | Warn when pad_token_id is in eos_token_id list |

### Closed (not merged)

| Date | Repo | PR | What happened |
|------|------|----|---------------|
| 2026-08-20 | roboflow/inference | [#2835](https://github.com/roboflow/inference/pull/2835) | AST topology test. Maintainers said the current numpy/tensor pairing is transitional, not a permanent contract. Closed, lesson recorded. |
| 2026-08-19 | huggingface/trl | [#6815](https://github.com/huggingface/trl/pull/6815) | Nemotron 3 SFT LoRA target modules. Superseded by maintainer fix. |
| 2026-08-17 | huggingface/peft | [#3556](https://github.com/huggingface/peft/pull/3556) | Warn when LoRA target_modules match low percentage of layers. Closed after discussion — the docs PR (#3603) addressed the root cause instead. |
| 2026-08-17 | huggingface/transformers | [#48021](https://github.com/huggingface/transformers/pull/48021) | NemotronHConfig num_hidden_layers property. Maintainer addressed differently. |
| 2026-07-28 | microsoft/onnxruntime | [#29921](https://github.com/microsoft/onnxruntime/pull/29921) | Document EP fallback detection. Closed — docs went elsewhere. |
| 2026-07-28 | ultralytics/ultralytics | [#25481](https://github.com/ultralytics/ultralytics/pull/25481) | ONNX export parity test. Closed — overlap with existing work. |
| 2026-07-27 | OpenHands/OpenHands | [#16104](https://github.com/OpenHands/OpenHands/pull/16104) | Vite file watcher fix. Closed — fixed upstream independently. |
| 2026-07-25 | ultralytics/ultralytics | [#25425](https://github.com/ultralytics/ultralytics/pull/25425) | ONNX export parity test (earlier attempt). |
| 2026-07-25 | apple/coremltools | [#2763](https://github.com/apple/coremltools/pull/2763) | Numerically stable log_softmax and logcumsumexp. |
| 2026-07-16 | haukesomm/apple-photos-export | [#15–17](https://github.com/haukesomm/apple-photos-export/pull/15) | Album filter and dedup fixes. Maintainer implemented own version. |
| 2026-07-12 | sindresorhus/nano-spawn | [#116](https://github.com/sindresorhus/nano-spawn/pull/116) | Accept strings as stdin input. Out of scope. |
| 2026-07-12 | apple/coremltools | [#2754–2756](https://github.com/apple/coremltools/pull/2754) | numpy 2.x scalar conversion and softplus fixes. |
| 2026-07-12 | ultralytics/ultralytics | [#25118, #25125](https://github.com/ultralytics/ultralytics/pull/25118) | DDP callback serialization. |
| 2026-07-12 | huggingface/transformers | [#47267](https://github.com/huggingface/transformers/pull/47267) | Restore dict return type in create_masks_for_generate. |
| 2026-07-12 | roboflow/roboflow-python | [#506](https://github.com/roboflow/roboflow-python/pull/506) | YOLO data.yaml path fix. Closed — maintainer addressed. |

### Review contributions

- **[roboflow/roboflow-python#495](https://github.com/roboflow/roboflow-python/pull/495)** — Reviewed the api-key CLI PR (authored by @yeldarby, Roboflow CTO). Three findings the author addressed before merge: (1) root-caused a numpy 2.5.0 × mypy PEP 695 CI failure blocking the entire repo, (2) caught `custom_metadata` vs `customMetadata` camelCase bug silently dropping metadata on every api-key create, (3) flagged error hint accuracy in protect/disable handlers.
- **[roboflow/roboflow-python#498](https://github.com/roboflow/roboflow-python/issues/498)** — Opened the issue diagnosing the CI failure, opened PR #499 with the fix, then closed my PR in favor of #495 after coordinating with the author.

### Issues opened

| Date | Repo | Issue | What |
|------|------|-------|------|
| 2026-08-24 | roboflow/inference | [#2846](https://github.com/roboflow/inference/issues/2846) | Cache Set/Get `__del__` only clears the last video namespace |
| 2026-08-24 | roboflow/inference | [#2845](https://github.com/roboflow/inference/issues/2845) | `inference.Model` is in `__all__` but does not resolve after lazy-init rewrite |
| 2026-08-17 | huggingface/transformers | [#48016](https://github.com/huggingface/transformers/issues/48016) | GenerationConfig should validate pad_token_id not in eos_token_id list |
| 2026-08-17 | huggingface/trl | [#6773](https://github.com/huggingface/trl/issues/6773) | Nemotron 3 SFT example uses target_modules that may not exist in hybrid architecture |
| 2026-08-17 | huggingface/peft | [#3554](https://github.com/huggingface/peft/issues/3554) | NemotronH LoRA: default target_modules only cover 7% of layers, silent failure |
| 2026-08-17 | state-spaces/mamba | [#1019](https://github.com/state-spaces/mamba/issues/1019) | No prebuilt wheels for sm_103 (B300) and sm_121 (GB10) |
| 2026-08-17 | Dao-AILab/causal-conv1d | [#119](https://github.com/Dao-AILab/causal-conv1d/issues/119) | No prebuilt wheels for sm_121 (GB10 / DGX Spark) |
| 2026-07-28 | microsoft/onnxruntime | [#29913](https://github.com/microsoft/onnxruntime/issues/29913) | Feature proposal: expose which execution providers actually ran |
| 2026-07-19 | OpenHands/OpenHands | [#15441](https://github.com/OpenHands/OpenHands/issues/15441) | Dev server infinite reload loop from literal `$HOME` in env var |
| 2026-07-15 | modelcontextprotocol/registry | [#1445](https://github.com/modelcontextprotocol/registry/issues/1445) | Proposal: mcp.health — standard health metadata field for registry entries |
| 2026-06-30 | roboflow/roboflow-python | [#498](https://github.com/roboflow/roboflow-python/issues/498) | CI typecheck fails: numpy 2.5.0 stubs use PEP 695 type statements |

---

## Models and datasets

I fine-tune and publish models on [HuggingFace](https://huggingface.co/davidnichols-ops). 15 models, 1 dataset.

| Model | Base | What | Downloads |
|-------|------|------|-----------|
| [claude-yolo-vibes](https://huggingface.co/davidnichols-ops/claude-yolo-vibes) | Qwen2.5-Coder-7B | Code assistant fine-tuned for the agent loop on macOS | 1,170 |
| [claude-yolo-vibes-v4-mlx-4bit](https://huggingface.co/davidnichols-ops/claude-yolo-vibes-v4-mlx-4bit) | Qwen2.5-Coder-7B | 4-bit MLX, runs on M4 16GB | 72 |
| [claude-yolo-vibes-v4-GGUF](https://huggingface.co/davidnichols-ops/claude-yolo-vibes-v4-GGUF) | Qwen2.5-Coder-7B | GGUF for Ollama/LM Studio | 239 |
| [adaptive-operator-v4](https://huggingface.co/davidnichols-ops/adaptive-operator-v4) | Qwen3.5-9B | Agentic tool-use with custom control tokens for adaptive compute | 299 |
| [yolo-hybrid-v6](https://huggingface.co/davidnichols-ops/yolo-hybrid-v6) | YOLO | Hybrid detection model | 37 |
| [NVIDIA-Nemotron-Nano-9B-v2-fork](https://huggingface.co/davidnichols-ops/NVIDIA-Nemotron-Nano-9B-v2-fork) | Nemotron Nano 9B | Fork with config fixes for GGUF conversion | 142 |
| [NVIDIA-Nemotron-3-Nano-30B-A3B-BF16-fork](https://huggingface.co/davidnichols-ops/NVIDIA-Nemotron-3-Nano-30B-A3B-BF16-fork) | Nemotron 3 Nano 30B | Fork with config fixes | 135 |
| [Anti-Reasoning-Engine-0.5B](https://huggingface.co/davidnichols-ops/Anti-Reasoning-Engine-0.5B) | Qwen2.5-0.5B | A joke model that refuses to reason. 194 downloads. The internet is weird. | 194 |

[adaptive-operator-v4-dataset](https://huggingface.co/datasets/davidnichols-ops/adaptive-operator-v4-dataset) — SFT + DPO training data for agentic tool use (4,992 SFT examples, 5,000 DPO pairs).

---

## Engineering Philosophy

These are observations I keep arriving at, not slogans I started with.

**Neural networks identify. Algorithms decide.** Judgment does not belong in floating-point weights. Put the decision logic in config, make it auditable, and let the network do what networks are good at — perception. A facility rule change should not require retraining.

**Freeze the wire, evolve above it.** The protocol is not the place to be clever. Bake interfaces, not algorithms. The acid test for any addition: does it make the system more capable, or merely more complicated? If it's merely complicated, it belongs in an implementation, not the spec.

**A working deterministic version beats a broken AI version.** Ship the heuristic first. Label it as an estimate. No fake precision. Add the LLM later, when it earns its place.

**Hardware reliability is table stakes, not an afterthought.** Cameras drop. Indexes enumerate wrong. The system has to reconnect, auto-detect, and keep grading. "Validated against the wrong camera" is a real failure mode I have shipped and then fixed.

**Read-only by default. Destructive actions commented out.** A scan that can't break your machine is a scan people will actually run. Remediation scripts get reviewed by a human before anything runs.

**Trust is a continuity problem, not a one-time check.** Before an agent calls a capability it didn't build, it needs to know what it is, who authorized it, whether it has changed, and whether this specific call is allowed. A boolean from the agent itself is not evidence — the verification has to produce the evidence, not consume it.

**Reality remains the final authority.** A neural network can be wrong about a fruit. A system misaligned with facility rules is useless. The README should say what's pending, not what's impressive.

---

## Selected Projects

### [apple-quality-recognition-engine](https://github.com/davidnichols-ops/apple-quality-recognition-engine)
Real-time CV pipeline for apple variety detection and USDA-style grading, built for the family orchard. YOLO26 detects; a `grading_policy.yaml` file grades. Defects bind to apples via Intersection-over-Area. Low-confidence frames are harvested as free training data. Runs on the Apple Neural Engine through CoreML. This is the project where my principles actually have to hold up against a piece of fruit.

### [AAFP](https://github.com/davidnichols-ops/aafp) · [research umbrella](https://github.com/davidnichols-ops/AAFP-research) · [Go interop](https://github.com/davidnichols-ops/aafp-go)
A post-quantum, agent-first P2P networking stack. Rust reference (19 crates, ~140K lines), a TypeScript SDK, and a Go implementation written strictly from the RFCs to validate that the wire format is unambiguous. The transport is frozen at Rev 6; the work above it is an Intelligence Plane — predictive routing, intent routing, reputation, pubsub. The competitor is not HTTP. The competitor is cloud silos that own the agent graph.

### [trustcard](https://github.com/davidnichols-ops/trustcard)
Cryptographic trust infrastructure for MCP servers — content-addressed capability identity, Ed25519-signed manifests, TOFU pinning, and two-gate call-time enforcement. Ships with an empirical health scanner (the "npm audit for MCP") that probes a server and produces a scorecard instead of trusting the agent's self-attested booleans. Three-engine danger detection: heuristic, semantic, and prompt-injection fusion.

### [mac-ai-os](https://github.com/davidnichols-ops/mac-ai-os)
A local-first AI operating system for macOS — an intelligence layer over the computer, not a chatbot. It reasons, retrieves, chooses tools, executes, verifies, and explains. The part I'm proudest of is the PR governance system: an evidence-producing state machine (DRAFT → UNDERSTOOD → VERIFIED → PR_READY) that captures real command output tied to a commit, so an agent can't fake "tests pass" by claiming a boolean.

### [X-MaC](https://github.com/davidnichols-ops/X-MaC) · [Homebrew tap](https://github.com/davidnichols-ops/homebrew-xmac)
A macOS system sanitizer and discovery tool in Rust. Every engine is read-only. Privacy redaction is on by default — home paths, tokens, keys, emails, IPs. Remediation scripts are emitted with destructive commands commented out and paths shell-quoted against injection.

### [repo-archaeologist](https://github.com/davidnichols-ops/repo-archaeologist)
Point it at an abandoned repo. Get an opinionated architecture, risk, and onboarding briefing in seconds. Zero runtime deps, offline, deterministic. The v1 deliberately avoids LLM prose — a working heuristic is more useful than a broken AI version.

### [dependency-intelligence](https://github.com/davidnichols-ops/dependency-intelligence)
Local-first dependency observability. Scans manifests across Python/JS/Rust/Go, builds a SQLite graph with recursive CTEs for transitive traversal, enriches with OSV vulnerabilities and registry metadata, computes risk findings mapped to a maintainer-corpus failure taxonomy, and exports to Obsidian + an agent-first JSON API. Built after watching a Roboflow PR get closed because the test assumed observed topology was a declared contract — the system enriches observed data with external ground truth instead.

---

## Current Interests

- **Edge ML on Apple Silicon** — CoreML, the Neural Engine, and the gap between a notebook model and a pipeline that survives a real camera.
- **Distributed systems and protocol design** — DHTs at scale, NAT traversal, post-quantum handshakes, and what it takes to make a spec unambiguous enough to implement twice.
- **Agent infrastructure and trust** — MCP security, signed manifests, TOFU pinning, and the governance layer that keeps autonomous agents from routing around their own constraints.
- **Developer tooling** — tools that read a system or a repo and tell you something true, with zero config and no API key.
- **Native macOS software** — Swift, SwiftUI, and apps that feel like they belong on the machine.
