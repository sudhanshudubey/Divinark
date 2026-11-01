# Current status

Reviewed **1 November 2026** against the available implementation, GitHub checks and owner-supplied local observations.

## Release status

This is an early development project. The latest reliability and K2 changes are in draft review and are not merged into the application's stable branch. The public repository's main branch contains showcase documentation only. It is not the application release branch, and no installable release is offered here.

## What the evidence supports

| Capability | Implementation and checks | Remaining qualification |
| --- | --- | --- |
| PLAN/BUILD and model selection | Terminal workflow, selector and controlled permission tests are present. File operations are exercised in disposable test directories. | These checks do not validate arbitrary coding tasks or every model's behavior. |
| Qwen through Ollama | Local models are integrated; owner-supplied local records show completed and cancelled requests. A single Qwen3.5 file-write smoke result is recorded in development notes. | This is limited smoke evidence, not a broad tool-use reliability study or a model ranking. |
| K2 Horizon 7B Q4_K_M | Optional local alias is selectable. Controlled HTTP/SDK tests cover incremental streaming, structured tool deltas, file operations, errors, timeout and cancellation. Owner-supplied output shows a successful real K2 PLAN text stream. | That live text test used test authentication/storage fixtures. Genuine K2 read/write tool calls and a matched Qwen comparison have not been demonstrated. Advertised tool capability is not proof of compatibility. |
| Telemetry and visualization | Recorded request outcomes, token availability, durations and linked tool events feed the dashboard. Reporting-contract and partial-data tests are present. | Not every agent action is instrumented. Unknown measurements are not zero, and a completed request does not establish task success. |
| Automatic investigation | Lifecycle hooks enqueue persistent jobs; controlled database-backed integration checks exercise the investigation path. | Owner-supplied dashboard captures show a linked missing-path finding and an inconclusive attempt. Captures alone do not establish automatic queue timing across a complete live task. |
| Restricted shell | Separate Docker integration checks exercise the execution boundary, a nonzero exit and timeout handling. | These are controlled software checks, not proof that all generated code is safe or that a task was solved. |
| Evaluation integrity | Controlled calibration, local-model pilot captures, diagnostic replays and retrospective baseline reporting have been performed. | Private bundles are withheld. Independent reference review, blind generalization and a research-method advantage are not established. |

## Verification record

The inspected development revision has successful GitHub checks for offline tests, TypeScript checks and production builds, plus a separate product job exercising disposable PostgreSQL and restricted Docker execution. Recorded local verification reports 164 passing tests and 17 explicit skips. Skipped real-model or unavailable-environment checks are not counted as live verification.

These are previously recorded software checks. Preparing this documentation does not rerun models, regenerate experiment data, authenticate a new application session or retest the owner's Mac. Private CI links, branch names, source revisions and raw outputs are deliberately not published. This summary is maintainer-reported; it is not a publicly reproducible application test suite.

## Known limitations

- Investigations use request-level metadata, not a complete task-level execution graph.
- The operational investigator does not evaluate task assertions, source semantics or required output artifacts.
- A tool-reported missing path demonstrates a failed lookup, not why it failed or who caused it.
- Missing, stale, truncated and interrupted observations remain uncertain. Client reports are not independently attested.
- Automatic investigation needs functioning persistence and monitoring. It cannot recover evidence that was never recorded.
- Optional cloud adapters remain implemented; live cloud-provider behavior was not revalidated for this showcase.
- There is no trained failure predictor, validated causal diagnosis, cross-agent integration, automatic repair or autonomous retry system.
- There is no public hosted service, downloadable application, independent benchmark result or production-readiness claim.

For the next implementation priorities, see the [roadmap](roadmap.md). For publication boundaries, see [rights and scope](../RIGHTS.md).
