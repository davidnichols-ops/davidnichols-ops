# David Nichols

I work on computer vision, inference reliability, and tools for inspecting and controlling what AI agents do.

I'm especially interested in the parts around the model: preserving data and coordinate contracts through a workflow, isolating runtime failures across hardware backends, and making automated decisions traceable to code and policy. Most of my work is in Python, with JavaScript for MCP tooling and a focus on Apple Silicon.

## Active project

- **[trustcard](https://github.com/davidnichols-ops/trustcard)** — tooling for inspecting MCP servers, signing capability manifests, detecting capability drift, and enforcing which tool calls are allowed. Published as [`mcp-trustcard`](https://www.npmjs.com/package/mcp-trustcard).

## Selected upstream contributions

Merged pull requests in projects maintained by their respective teams:

| Project | Contribution |
| --- | --- |
| Roboflow Inference | [Reuse a run-scoped thread pool for workflow execution](https://github.com/roboflow/inference/pull/3052) |
| Roboflow Inference | [Preserve image dimensions on empty VLM detections](https://github.com/roboflow/inference/pull/2892) |
| Roboflow Inference | [Clear every touched namespace in workflow cache blocks](https://github.com/roboflow/inference/pull/2834) |
| Roboflow Python SDK | [Return single-upload results from `Project.upload()`](https://github.com/roboflow/roboflow-python/pull/502) |
| TensorFlow | [Fix XLA `DenseBincount` negative-input validation for runtime tensors](https://github.com/tensorflow/tensorflow/pull/122706) |
| Ultralytics | [Exclude `Sigmoid` from TensorRT INT8 quantization](https://github.com/ultralytics/ultralytics/pull/25020) |
| Hugging Face PEFT | [Document hybrid Mamba-Transformer `target_modules` pitfalls](https://github.com/huggingface/peft/pull/3603) |

[All merged upstream pull requests](https://github.com/pulls?q=is%3Apr+is%3Amerged+is%3Apublic+author%3Adavidnichols-ops+-user%3Adavidnichols-ops)

## How I work

I focus on understanding a system well enough to reproduce and explain why it failed—building that judgment through root-cause debugging, differential testing, and maintaining my own tools.

- Start with a minimal reproducible failure and keep fixes narrow.
- Add regression tests that fail before the patch and report exact verification boundaries.
- Keep model observations, deterministic policy, and human authorization separate where reliability matters.

Older repositories hold prototypes, archived experiments, and retired research (including [`apple-quality-recognition-engine`](https://github.com/davidnichols-ops/apple-quality-recognition-engine), closed out with a [documented engineering postmortem](https://github.com/davidnichols-ops/apple-quality-recognition-engine/blob/main/docs/RETIREMENT.md) and partial dataset). Each repository's README states its current status.
