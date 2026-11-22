# CareerOS ATS Service â€” service overview

## Responsibility

Validate final resume artifacts for extractability, structure, readability and job relevance.

## Data ownership

Versioned validation reports and internal compatibility scores.

## Interfaces

- Inputs: Final PDF/DOCX artifact, profile version and job version.
- Outputs: Blocking findings, warnings and evidence-based recommendations.
- Dependencies: resume, profile and job services.

## Contract rules

- APIs and events are versioned.
- Consumers must be idempotent where retries are possible.
- Correlation identifiers are propagated without logging sensitive payloads.
- Authorization and ownership are checked at the service boundary.

## Non-goals

This service does not absorb responsibilities owned by another CareerOS service. Cross-service workflows are coordinated through explicit contracts rather than shared databases.

## Security and privacy

Persist the minimum data required, record provenance, define retention, redact logs and use synthetic examples in this public repository.