# 02 Future State Process

## Purpose

This document describes the proposed OCR-assisted future-state workflow.

## Future Process

Invoice PDF Intake
-> OCR Extraction
-> Mandatory Field and Confidence Check
-> Invoice Type Classification
-> Non-PO Workflow, PO Workflow, or AP Triage
-> AP Review
-> Invoice-type-specific SAP output preparation

## Design Decision

Invoice classification should happen before approval, matching, or SAP output preparation.
