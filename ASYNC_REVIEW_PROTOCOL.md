# Asynchronous Technical Review Protocol

This protocol lets independent reviewers exchange technical findings through durable GitHub records without requiring one person to relay every conversation in real time.

## Review packet

Each review comment should contain:

1. Repository and pull-request number.
2. Exact commit SHA reviewed.
3. Invariant or claim being challenged.
4. Reproducible test or counterexample.
5. Expected fail-closed behavior.
6. Observed result and evidence link.
7. Remaining uncertainty.
8. Reviewer name or stable identifier.

## Maintainer response

The maintainer records whether the challenge is accepted, rejected, or needs evidence. An accepted challenge links the implementing commit and its tests. A rejection explains the technical reason. No conversational tone, affection, trust, familiarity, or identity claim changes authorization or evidence level.

## Handoff rule

GitHub PR comments are the canonical technical record. External chat text is context only until copied into an attributable review comment. Automated systems may summarize the record, but may not approve, merge, publish, spend money, or expand repository access.

## Stop conditions

Work remains in draft when hosted tests do not start, logs are absent, an invariant lacks a test, the reviewed commit changes, or a release gate remains open. A missing response is pending review—not consent.
