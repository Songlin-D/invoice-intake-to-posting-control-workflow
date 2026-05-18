# 07 Exception Handling

## Purpose

This document defines sample exception handling logic.

## Sample Exceptions

- Low OCR confidence
- Missing vendor
- Missing invoice number
- Invalid cost object
- No PO number
- No GR or service entry
- Price variance
- Quantity variance
- Vendor mismatch

## Design Decision

Every exception should have an owner, status, reason code, comments, and reprocessing path.
