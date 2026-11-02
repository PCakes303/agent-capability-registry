# Repository 15 deployment and audit status

**Repository:** [PCakes303/agent-capability-registry](https://github.com/PCakes303/agent-capability-registry)  
**Audited baseline:** `0220f7ecc89589b9ccd256a705188d7ff27d1371`  
**Baseline CI:** [Run 41413613566](https://github.com/PCakes303/agent-capability-registry/actions/runs/41413613566) — success  
**Staging source:** `provisioning/staged/agent-capability-registry/` in the master repository.

## Current deployment record

The public remote exists and is authoritative for current implementation. The historical 18-file deployment and CI records are provenance only; refresh path/blob-SHA parity against current `main` before portfolio sign-off.

## Remediation in progress

Registered capability declarations are now copied into immutable attribute mappings, preventing caller-side mutation after validation. Match requests are bounded to 128 requirements by default. Policy callback results must be explicit boolean `True`; false, non-boolean and exception outcomes deny candidates.

## Remaining verification

- Bind capability declarations to Resource Manifest and Schema Registry canonical contracts; pin compatible versions and publish reproducible cross-repository fixtures.
- Connect policy callback to an authenticated policy service; it remains a test/integration seam.
- Verify GitHub private vulnerability reporting/security advisory configuration; SECURITY.md records that no dedicated private reporting address is published.
- Apply and verify GitHub About homepage/topics (description exists).
- Verify branch rulesets/protection, Actions permissions, secret scanning, push protection and dependency alerts.
- Refresh staging-to-remote path/blob-SHA parity.
- Retain pending license status until an explicit repository/artifact licensing decision is approved.

## Maturity and limitations

This remains an experimental process-local registry. Matching is advisory only; it does not authenticate agents, prove capability claims, grant permissions, execute work, verify health or provide distributed discovery/consistency. No release is published.
