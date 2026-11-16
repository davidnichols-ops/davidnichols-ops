# David Nichols

I work on computer vision, inference reliability, and tools for inspecting and controlling what AI agents do.

I'm especially interested in the parts around the model: preserving data through a workflow, understanding runtime failures, and making decisions traceable to code and policy. Most of my work is in Python, with JavaScript for MCP tooling and a particular interest in Apple Silicon.

## Active project

- **[trustcard](https://github.com/davidnichols-ops/trustcard)** — tooling for inspecting MCP servers, signing capability manifests, detecting changes, and enforcing which tool calls are allowed. Available as [`mcp-trustcard`](https://www.npmjs.com/package/mcp-trustcard).

## Research case study: AQRE

**[Apple Quality Recognition Engine](https://github.com/davidnichols-ops/apple-quality-recognition-engine)** — a retired computer-vision research prototype for apple grading. I built capture and annotation tooling, a deterministic grading engine, review-evidence logging, and a model smoke-test adapter. A trained YOLO26s-Seg model was exercised on 127 images, including 30 four-view apple profiles.

The experiment exposed weak surface-defect recall, dataset split leakage, and gaps in bruise assessment, size measurement, and per-apple conveyor tracking. I retired active development rather than expand annotation work without evidence that it would resolve the operating requirements. The closeout preserves the implementation, 65 passing tests, known limitations, and a 120-image partial dataset.

[Engineering findings and retirement decision](https://github.com/davidnichols-ops/apple-quality-recognition-engine/blob/main/docs/RETIREMENT.md) · [Prediction evidence and replay instructions](https://github.com/davidnichols-ops/apple-quality-recognition-engine/tree/main/research/closeout) · [Partial dataset release](https://github.com/davidnichols-ops/apple-quality-recognition-engine/releases/tag/research-retirement-2026-11-16)

## Selected upstream contributions

These are merged contributions to projects maintained by their respective teams.

| Project | Contribution |
| --- | --- |
| Roboflow Inference | [Reuse a run-scoped thread pool for workflow execution](https://github.com/roboflow/inference/pull/3052) |
| Roboflow Inference | [Preserve image metadata on empty Template Matching results](https://github.com/roboflow/inference/pull/3038) |
| Roboflow Python SDK | [Return upload results to callers](https://github.com/roboflow/roboflow-python/pull/502) |
| TensorFlow | [Fix XLA DenseBincount negative-input validation for runtime tensors](https://github.com/tensorflow/tensorflow/pull/122706) |
| Ultralytics | [Exclude Sigmoid from TensorRT INT8 quantization](https://github.com/ultralytics/ultralytics/pull/25020) |

[More merged contributions](https://github.com/pulls?q=is%3Apr+is%3Amerged+is%3Apublic+author%3Adavidnichols-ops+-user%3Adavidnichols-ops)

## How I work

I like understanding a system well enough to explain why it failed. I'm building that judgment through debugging, code review, and maintaining my own tools.

- Start with a reproducible failure and keep fixes focused.
- Add regression coverage and report exactly what was tested.
- Keep model outputs, policy decisions, and human approval separate where the application calls for it.

Older repositories include experiments and archived work. Their READMEs describe their status. Trustcard remains active; AQRE is preserved as a documented research case study.
