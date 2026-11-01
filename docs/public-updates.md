# Updating the showcase

Development remains separate. This repository receives selected, verified progress through a manual review; it does not pull or mirror application history.

## Weekly procedure

1. Inspect the exact development revision and its actual test results. Check whether a feature is merged, under review, experimental or only planned.
2. Draft a short public summary in your own words. State what changed, how it was checked, what was observed and what remains unverified. Do not include private repository links, branch names or source revisions.
3. Update the dated status table and roadmap. Keep controlled software tests separate from real model observations and independently reviewed evaluation.
4. For each screenshot or example, confirm ownership or redistribution permission. Use only sanitized genuine captures; review the entire file, including image metadata. The [media checklist](../media/README.md) applies.
5. Review the complete staged changes and file list. Check for credentials, personal details, machine paths, internal addresses, identifiers, restricted source and private experiment material. An ignored file can still be force-added: the allowlist is a guard, not a clearance decision.
6. Commit the selected public files to this repository and review the rendered GitHub pages after pushing. Do not attach unreviewed archives or copy the development Git directory.

Use exact paths when staging, for example:

```bash
git status --short
git diff --check
git add -- README.md docs/current-status.md docs/roadmap.md
git diff --cached --stat
git diff --cached
git commit -m "docs: update verified project status"
git push origin main
```

Run those commands only from the separate showcase checkout. Its origin must point to the public showcase, never to a development repository. The initial package uses an explicit file allowlist in .gitignore. Add new public paths to that allowlist only after reviewing them.

## A useful progress entry

Record the date, the implemented behavior, the kind of check performed, the observed result and the remaining limitation. Do not turn an unchanged calibration result into a new milestone, count skipped tests as passes or report a performance gain without a reproducible comparison.

Revisit [publication scope](../RIGHTS.md) before adding any source, binary, third-party asset or model file. Public documentation does not settle the application's redistribution rights.
