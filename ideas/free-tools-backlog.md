# Free Tools Backlog

These are intentionally small. Each one should have a clear promise, local-first behavior, and a reason someone would star the repo.

## Accounting and GST helpers

### GST invoice number normalizer

Normalize invoice numbers from GSTR-2B, Tally, Zoho Books, Busy, and purchase registers.

Why it is useful:

- GST reconciliation often fails on formatting, not accounting.
- This can be a tiny browser tool or CLI.
- It avoids duplicating ClearLedger while feeding the same audience.

Inputs:

- Paste invoice numbers.
- Upload CSV.

Outputs:

- Original invoice number.
- Normalized invoice number.
- Normalization rule applied.
- Possible collision warning.

### GSTR-2B column mapper

Detect common GSTR-2B export columns and map them to a standard schema.

Why it is useful:

- Safer than publishing full ClearLedger in Labs.
- Good SEO around `GSTR-2B Excel column format`.

Outputs:

- Mapped schema.
- Missing required fields.
- Downloadable clean CSV.

### Tally export cleaner

Clean common Tally export artifacts: repeated headers, summary rows, blank lines, amount strings, and weird date formats.

Why it is useful:

- Tally data cleanup is common, painful, and search-driven.
- It can reuse ideas from Sheet Doctor without copying the active web app.

### GST mismatch reason explainer

Paste a row-level mismatch and get a plain-English reason checklist.

Keep it deterministic:

- Amount differs.
- Date outside tolerance.
- GSTIN invalid.
- Invoice number normalized differently.
- Present in portal but missing in register.
- Present in register but missing in portal.

## Spreadsheet utilities

### Spreadsheet risk scanner

Upload a workbook and get a non-destructive report:

- Hidden sheets.
- Merged ranges.
- Formula errors.
- Duplicate headers.
- Empty edge columns.
- Mixed date columns.

This is a good companion to Sheet Doctor CLI without duplicating the active web tool.

### CSV encoding fixer

Detect and repair common mojibake/encoding issues, then let users download UTF-8 CSV.

Good repo angle:

- `Fix broken CSV encoding locally. Nothing uploaded.`

### Workbook sheet inventory

Generate a table of every sheet in a workbook:

- Sheet name.
- Visibility.
- Row/column count.
- Formula count.
- Error count.
- Last modified metadata if available.

### Formula residue detector

Find formula cells, cached values, error formulas, and pasted-value inconsistencies.

This is especially useful for finance teams receiving workbook exports from clients.

## Privacy helpers

### Bank statement anonymizer

Replace names, account numbers, descriptions, and exact amounts with safe sample values while preserving row shape.

Use case:

- People can share bug reports or examples without leaking real finances.

### UPI statement cleaner

Clean UPI transaction exports into a standard CSV:

- Date.
- Counterparty.
- Direction.
- Amount.
- UPI reference.
- Notes.

## General data helpers

### CSV duplicate finder

Find duplicate rows or near-duplicates by selected columns.

### Local JSON to CSV converter

Flatten JSON and JSONL locally, with a preview of nested paths.

### Filename invoice renamer

Rename downloaded invoice PDFs or images into a consistent pattern:

`YYYY-MM-DD_vendor_invoice-number_amount.ext`

The first version can be manual-entry only. OCR can come later.

## Best first three

1. GST invoice number normalizer.
2. Spreadsheet risk scanner.
3. Bank statement anonymizer.

These hit the sweet spot: searchable pain, local-first trust, low build complexity, and a clean bridge back to Quietly.tools.

