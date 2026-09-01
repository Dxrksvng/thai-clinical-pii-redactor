# Safety and privacy boundaries

- Synthetic documents only; no patient or employer data is included.
- Raw OCR text and detected PII values are excluded from audit logs.
- Redaction uses opaque rectangles, not reversible blur or pixelation.
- A zero-detection result is not considered safe and requires human review.
- Name detection is intentionally conservative.
- Production use requires independently evaluated Thai NER, representative licensed data, access controls, retention controls, and security review.
- The prototype is not medical advice, a production medical system, or proof of PDPA compliance.

Never attach real clinical records to a public issue.

