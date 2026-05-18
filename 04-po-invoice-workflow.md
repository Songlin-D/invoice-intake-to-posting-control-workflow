# 04 PO Invoice Workflow

## Purpose

This document describes the PO invoice path.

## Process

Invoice PDF
-> OCR Extraction
-> PO Number Identification
-> PO / GR / Invoice Matching
-> Match or Exception Handling
-> AP Review
-> PO Invoice Verification Staging Output

## Control Logic

PO invoices should be controlled through matching logic rather than asking the requester to re-enter accounting assignment fields.
