# David Nichols

Inference and edge-runtime engineer. I land narrow, tested fixes in upstream
computer-vision and ML codebases, and build local-first tooling that verifies a
system is still what it claims to be. Most of the work sits at the boundary
where a model's output stops and an auditable decision has to be made.

*1,029 contributions in the trailing year (GitHub contributions graph, 2026-09-12).*

## Merged upstream contributions

| Merged | Project | Change |
|---|---|---|
| 2026-09-11 | [roboflow/inference#2892](https://github.com/roboflow/inference/pull/2892) | Preserve image dimensions on empty VLM detection workflow output |
| 2026-08-28 | [roboflow/inference#2834](https://github.com/roboflow/inference/pull/2834) | Clear every touched namespace in workflow cache blocks — refcounted ownership + per-instance locking |
| 2026-08-28 | [roboflow/inference#2844](https://github.com/roboflow/inference/pull/2844) | Resolve `inference.Model` through the lazy package init (PEP 562) |
| 2026-08-26 | [huggingface/peft#3603](https://github.com/huggingface/peft/pull/3603) | Troubleshooting docs for hybrid-architecture `target_modules` |
| 2026-08-03 | [roboflow/roboflow-python#501](https://github.com/roboflow/roboflow-python/pull/501), [#502](https://github.com/roboflow/roboflow-python/pull/502) | Relax the `opencv-python-headless` pin; return the `single_upload` result from `Project.upload()` |
| 2026-07-27 | [tensorflow/tensorflow#122706](https://github.com/tensorflow/tensorflow/pull/122706) | XLA `DenseBincount` negative-input validation for runtime tensors |
| 2026-07-09 | [ultralytics/ultralytics#25020](https://github.com/ultralytics/ultralytics/pull/25020) | Exclude `Sigmoid` from TensorRT INT8 quantization |

Eight merged pull requests across six third-party projects. I contribute upstream
as an outside contributor — I don't maintain these projects.

**Open now**

- [roboflow/inference#2983](https://github.com/roboflow/inference/pull/2983) — **draft**, open 2026-09-12: carry image dimensions on empty Florence-2 VLM results.
- [huggingface/transformers#48022](https://github.com/huggingface/transformers/pull/48022) — open: warn when `pad_token_id` is in the `eos_token_id` list.

I also have closed attempts and small doc/typo merges; the merged set above is
the substantive record, so I don't enumerate the rest here.

## Verification tooling

Tools that answer "is this still the same thing?" — published and installable:

- **[trustcard](https://github.com/davidnichols-ops/trustcard)** — cryptographic
  trust infrastructure for MCP servers: signed manifests, TOFU pinning, two-gate
  call-time enforcement, and a scanner that probes a server and emits a scorecard
  instead of trusting the agent's self-attested booleans. Published to npm as
  [`mcp-trustcard`](https://www.npmjs.com/package/mcp-trustcard) (v3.1.0, 2026-09-12).
- **[cvconform](https://github.com/davidnichols-ops/cvconform)** — differential
  conformance for computer-vision models: compares ONNX/TensorRT exports against
  source checkpoints across backends and precisions to catch silent numeric drift
  that passes unit tests but breaks a production pipeline. Published to PyPI as
  [`cvconform`](https://pypi.org/project/cvconform/) (0.1.1).
- **[repo-archaeologist](https://github.com/davidnichols-ops/repo-archaeologist)** —
  offline, zero-dependency architecture / risk / onboarding briefing for an
  unfamiliar repo. Published to PyPI as
  [`repo-archaeologist`](https://pypi.org/project/repo-archaeologist/) (0.1.2).

## Edge and runtime work

- **[apple-quality-recognition-engine](https://github.com/davidnichols-ops/apple-quality-recognition-engine)** —
  real-time CV pipeline for apple variety detection and USDA-style grading. YOLO26
  detects; a `grading_policy.yaml` grades. Defects bind via Intersection-of-Area,
  low-confidence frames are harvested as training data, and it runs on the Apple
  Neural Engine through CoreML. A prototype with a placeholder model — not a
  validated commercial grader.
- **[mac-ai-os](https://github.com/davidnichols-ops/mac-ai-os)** — a local-first AI
  operating system for macOS. Its PR-governance system is an evidence-producing
  readiness state machine that captures real command output tied to a commit, so
  an agent can't fake "tests pass" with a boolean. Public with CI. Caveat: the
  public tree is a snapshot and trails local work.
- **[aafp-commons](https://github.com/davidnichols-ops/aafp-commons)** — a signed,
  append-only evidence ledger for agents: Ed25519-signed packets with conflict and
  resolution tracking, readable over MCP/CLI. Hook-and-file only; no daemon.
- **[X-MaC](https://github.com/davidnichols-ops/X-MaC)** — macOS system sanitizer
  and discovery tool in Rust + SwiftUI. Every engine is read-only; privacy
  redaction is on by default, and remediation scripts ship with destructive
  commands commented out.

I also work at the hardware/deployment boundary: filed public issues for missing
prebuilt wheels on newer NVIDIA targets —
[state-spaces/mamba#1019](https://github.com/state-spaces/mamba/issues/1019) (sm_103 / B300),
[Dao-AILab/causal-conv1d#119](https://github.com/Dao-AILab/causal-conv1d/issues/119) (sm_121 / GB10).

## Working method

- **Reproducer first.** Failure case → trace → fix → regression test. Fixes land
  with a scoped test, not a full-suite claim.
- **Detection identifies; algorithms decide.** Keep judgment out of the weights and
  in auditable config, so a rule change doesn't require retraining.
- **Verification has to produce evidence, not consume it.** A boolean from the
  agent that ran the action is not proof.

## Models and datasets

20 public models and 1 dataset on
[HuggingFace](https://huggingface.co/davidnichols-ops) (2026-09-12), mostly small
fine-tunes and GGUF/MLX conversions for local agent loops.
