# 09 SAP Output Design

## Purpose

This document describes sample SAP output preparation by invoice type.

## Output Logic

Non-PO invoice -> SAMPLE_NON_PO_UPLOAD_TEMPLATE
PO invoice -> PO_INVOICE_VERIFICATION_STAGING_OUTPUT
Unclear invoice -> No output until AP classification

## Design Decision

SAP output should follow invoice type and control logic. PO invoices should not be processed through a Non-PO output path if matching control is required.
