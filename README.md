# CareerOS ATS Service

Validate final resume artifacts for extractability, structure, readability and job relevance.

## Scope

- **Owns:** Versioned validation reports and internal compatibility scores.
- **Inputs:** Final PDF/DOCX artifact, profile version and job version.
- **Outputs:** Blocking findings, warnings and evidence-based recommendations.
- **Dependencies:** resume, profile and job services.

## Safety baseline

This public repository must never contain secrets, real resumes, real applications or personal data. External communication and application submission always require explicit user approval.

## Documentation

See [docs/overview.md](docs/overview.md) and the central [CareerOS workspace](https://github.com/FievezRomain/careeros-workspace).

## Status

Architecture and security baseline. Functional implementation will be added incrementally with tests and versioned contracts.

## License

Apache-2.0.