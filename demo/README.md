# Demonstration record

No executable demo, application source, model weights or hosted endpoint is included in this repository. The descriptions below summarize observed development behavior; they are not a substitute for a reproducible public benchmark.

## Available observations

**A supported execution finding.** An owner-supplied local dashboard capture shows a filesystem tool reporting a missing path. The investigator links that report to its request and presents it as an observable execution failure. It leaves the reason for the missing path and overall task correctness unresolved. This came from a smoke check, not a randomly sampled production incident.

**An inconclusive attempt.** A second capture shows a completed inference request without linked tool reports or a task contract. The dashboard explicitly declines to certify task success. Missing tool reports do not prove that no tools executed.

**Local K2 text streaming.** Owner-supplied test output shows a real K2 Horizon 7B Q4_K_M PLAN text response through the Divinark server/SDK path. The test uses fixture authentication and storage. It does not establish K2 tool execution, database-backed dashboard recording, coding quality or comparative speed.

## What a complete product demonstration must still show

A continuous local demonstration should show an actual task, permitted tool execution, linked inference/tool records and an investigation appearing automatically. It must also include a successful execution that is not incorrectly labelled as a failure and a case where the system has insufficient evidence.

Use disposable, non-sensitive files and the existing restricted execution boundary. Label deliberate fault injection as controlled. Do not run arbitrary generated programs directly on the host, expose credentials or substitute fabricated terminal output for an observed run.

## Public media

Available full-window captures have not been included because they contain non-public context and visual assets still need publication clearance. See the [media checklist](../media/README.md). There are no substitute UI mockups or invented performance charts in this repository.
