# Project overview

Divinark is being built to make coding-agent failures easier to investigate without confusing a plausible explanation with a verified result.

The user interacts with a terminal coding agent. Model inference happens through the API, while the terminal handles permitted tools. Recorded inference attempts and tool reports provide the initial evidence for the reliability subsystem. The dashboard exposes the resulting findings and uncertainty.

## The engineering problem

A failed agent interaction can involve several different layers: a provider stream, a file operation, a shell process, missing execution reports, or the task's actual requirements. An HTTP success says little about whether the requested program is correct. A failed tool call alone does not establish that the model caused the failure.

Divinark currently supports narrower operational findings. For example, a filesystem tool reporting a missing path supports a statement about that lookup. Without the requested path, file state or task requirement, it does not establish why the path was absent or whether the whole task failed.

## Evidence distinctions

| Result | Meaning |
| --- | --- |
| Supported observation | A bounded deterministic rule identifies a recorded execution event. The event's provenance remains visible. |
| Unverified explanation | A possible explanation is stated as a hypothesis. It cannot override the recorded result. |
| Inconclusive investigation | The available metadata do not demonstrate a technical failure or distinguish the relevant explanations. |
| Task correctness not evaluated | No reviewed task-level assertion or required-artifact check has been supplied to the operational investigator. |

An investigation marked complete means its bounded check finished and found an observable technical failure. It does not mean the agent completed the user's task or that a causal explanation has been proved.

## Development and research

The product includes the terminal agent and its reliability interface. Separate evaluation-integrity work uses controlled task contracts, intentionally defective graders and frozen model outputs to study how evaluation procedures can mislead. Those controls are calibration exercises, not a claim of novel diagnosis performance.

The long-term goal is independently evaluated failure detection and evidence-based diagnosis across agents and environments. The current implementation integrates Divinark's own agent only. Automatic repair, autonomous retries and a trained failure predictor are not implemented.
