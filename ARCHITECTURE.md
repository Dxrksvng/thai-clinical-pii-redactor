# Architecture overview

The prototype uses a small, auditable pipeline:

1. An OCR adapter emits text regions and bounding boxes.
2. Deterministic detectors identify supported PII classes.
3. The redactor paints opaque black rectangles over matched regions.
4. The audit layer records metadata only, never detected values or raw OCR text.
5. Documents with no detections are routed to mandatory human review.

The deterministic OCR sidecar keeps tests reproducible without downloading model weights. EasyOCR is an optional adapter rather than a trusted safety boundary.

Implementation details remain private during prototype hardening.

