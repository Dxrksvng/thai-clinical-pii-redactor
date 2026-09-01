# Roadmap

## Current prototype

- Deterministic detection for supported Thai PII patterns
- Thai national-ID checksum validation
- Irreversible image redaction
- Metadata-only audit output
- Human-review routing for no-detection cases
- Safety-focused automated tests

## Before wider evaluation

1. Generate or license a representative Thai synthetic-document corpus.
2. Annotate PII bounding boxes by entity type.
3. Split evaluation data by template and source to prevent leakage.
4. Report per-class precision, recall, F1, and document-level leakage rate.
5. Add versioned Thai NER and barcode adapters.
6. Add confidence-based review queues and failure-injection tests.

## Public-release gate

Implementation may be progressively opened only after privacy review, reproducible evaluation, secret scanning, dependency review, and removal of operational configuration.

