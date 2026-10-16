# David Nichols

I land narrow, tested fixes in upstream computer-vision code, and I keep the
decision outside the weights when I can. Detection identifies. A versioned
policy decides. A boolean from the thing that just ran is not evidence.

Outside contributor. I do not maintain the projects in the table below.

## Merged upstream

| Merged | Project | Change |
| --- | --- | --- |
| 2026-09-25 | [roboflow/inference#3052](https://github.com/roboflow/inference/pull/3052) | One run-scoped thread pool for executor-less workflow runs. Shipped in inference v1.7.2. |
| 2026-09-25 | [roboflow/inference#3038](https://github.com/roboflow/inference/pull/3038) | Preserve image metadata on empty Template Matching results. Shipped in v1.7.2. |
| 2026-09-18 | [roboflow/inference#2983](https://github.com/roboflow/inference/pull/2983) | Carry image dimensions through empty Florence-2 detections. |
| 2026-09-11 | [roboflow/inference#2892](https://github.com/roboflow/inference/pull/2892) | Preserve image dimensions on empty VLM detection output. |
| 2026-08-28 | [roboflow/inference#2834](https://github.com/roboflow/inference/pull/2834) | Clear every touched namespace in workflow cache blocks. |
| 2026-08-28 | [roboflow/inference#2844](https://github.com/roboflow/inference/pull/2844) | Resolve `inference.Model` through the lazy package init (PEP 562). |
| 2026-08-03 | [roboflow/roboflow-python#501](https://github.com/roboflow/roboflow-python/pull/501), [#502](https://github.com/roboflow/roboflow-python/pull/502) | Relax the opencv-python-headless pin; return the `single_upload` result. |
| 2026-07-27 | [tensorflow/tensorflow#122706](https://github.com/tensorflow/tensorflow/pull/122706) | XLA DenseBincount negative-input validation for runtime tensors. |
| 2026-07-09 | [ultralytics/ultralytics#25020](https://github.com/ultralytics/ultralytics/pull/25020) | Exclude Sigmoid from TensorRT INT8 quantization. |
| 2026-08-26 | [huggingface/peft#3603](https://github.com/huggingface/peft/pull/3603) | Docs only: troubleshooting for hybrid-architecture `target_modules`. |

Typo and comment fixes exist and are not listed. Closed, unmerged attempts are
not listed either. An npm RFC for install-trust telemetry was closed; the
scanner lives in trustcard instead of waiting on the registry.

## What I maintain

- **[trustcard](https://github.com/davidnichols-ops/trustcard)** — signed manifests,
  TOFU pinning, and a scanner for MCP servers. Published as
  [`mcp-trustcard`](https://www.npmjs.com/package/mcp-trustcard) 3.2.0 (2026-10-15).
- **[apple-quality-recognition-engine](https://github.com/davidnichols-ops/apple-quality-recognition-engine)** —
  edge grading prototype. A detector proposes regions; `grading_policy.yaml`
  grades; a human promotes labels and checkpoints. No trained apple checkpoint
  is in the tree. Not a commercial grader.

## Method

- Reproducer, then fix, then a scoped regression test. Not a full-suite claim.
- Judgment stays in config a person can diff.
- Verification has to produce evidence. It does not accept a boolean from the
  agent that ran the action.

## Not the portfolio

Older public experiments — agent P2P drafts, a macOS cleaner, local agent-OS
snapshots, benchmark notes — are unmaintained. If a README and the tree
disagree, the tree wins.
