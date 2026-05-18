# Invoice Intake-to-Posting Control Workflow

## Overview

This repository documents a public-safe, anonymized sample workflow for OCR-assisted invoice intake and SAP posting preparation in Accounts Payable.

The workflow separates invoices into three paths before SAP output preparation:

- Non-PO invoice path
- PO invoice path
- Unclear or low-confidence invoice path

The sample focuses on workflow design, controls, exception handling, and SAP posting readiness. It does not include real company data, real supplier data, real SAP configuration, or production upload files.

## Target Process Summary

Invoice PDF Intake
-> OCR Extraction
-> Invoice Type Classification
-> Route to Non-PO, PO, or AP Triage
-> AP Review
-> Generate invoice-type-specific SAP output preparation file

## Key Design Principles

- Non-PO invoices require business confirmation and approval control.
- PO invoices require PO / GR / Invoice matching control.
- Unclear invoices require AP triage before further processing.
- AP remains the final quality gate before SAP output preparation.
- SAP output should be generated only after required controls are complete.

## Repository Contents

- 01-current-state.md
- 02-future-state-process.md
- 03-non-po-workflow.md
- 04-po-invoice-workflow.md
- 05-field-mapping.md
- 06-risk-control-matrix.md
- 07-exception-handling.md
- 08-approval-matrix-sample.md
- 09-sap-output-design.md
- sample-templates/

## Public-Safe Data Notice

This repository uses generic sample names and placeholder values only.

Examples:

- SAMPLE_COMPANY_CODE
- SAMPLE_VENDOR_ID
- SAMPLE_COST_CENTER
- SAMPLE_INTERNAL_ORDER
- SAMPLE_TAX_CODE
- SAMPLE_PO_NUMBER
- SAMPLE_GR_NUMBER
- SAMPLE_NON_PO_UPLOAD_PROGRAM

Do not upload real invoices, supplier names, vendor codes, cost centers, internal orders, tax configuration, SAP Z transaction names, payment details, or company-specific templates to a public repository.
