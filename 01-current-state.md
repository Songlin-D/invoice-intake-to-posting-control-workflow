# 01 Current State

## Purpose

This document describes the current invoice intake and SAP upload preparation process in a public-safe and anonymized way.

## Current Process

Invoice PDF or supporting document
-> User manually fills a fixed request form
-> AP reviews submitted information
-> Form data is converted into a Non-PO SAP upload preparation file
-> AP performs upload through an approved internal process

## Current Strengths

- A fixed request format already exists.
- AP review happens before SAP output.
- A repeatable Non-PO upload preparation path exists.
- The process provides a foundation for controlled automation.

## Current Limitations

- Manual invoice data entry creates rekeying risk.
- Business users may not know accounting fields.
- Exception handling may happen offline.
- PO and Non-PO invoices may not be separated early enough.

## Design Decision

The future workflow should reuse the current Non-PO output preparation logic while improving invoice intake, classification, validation, approval evidence, and exception tracking.
