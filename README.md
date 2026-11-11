# David Nichols

I work on computer vision, inference reliability, and tools for inspecting and controlling what AI agents do.

I'm especially interested in the parts around the model: preserving data through a workflow, understanding runtime failures, and making decisions traceable to code and policy. Most of my work is in Python, with JavaScript for MCP tooling and a particular interest in Apple Silicon.

## Projects

- **[trustcard](https://github.com/davidnichols-ops/trustcard)** — tooling for inspecting MCP servers, signing capability manifests, detecting changes, and enforcing which tool calls are allowed. Available as [`mcp-trustcard`](https://www.npmjs.com/package/mcp-trustcard).
- **[Apple Quality Recognition Engine](https://github.com/davidnichols-ops/apple-quality-recognition-engine)** — an apple-grading prototype that separates visual observations from a versioned grading policy. The current work centers on annotation, case review, and human-approved training data. It does not yet include a trained apple checkpoint or a validated commercial grading system.

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

Older repositories include experiments and archived work. Their READMEs describe their status; the two projects above are my current focus.
