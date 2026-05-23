# CPCSC Level 1 self-assessment

An open-source self-assessment template for the Canadian Programme for Cyber Security Certification (CPCSC), Level 1.

## What this is

A working assessment artifact (Markdown for diff-friendliness, with companion `.csv` for spreadsheet import) that lets an organization self-attest against the CPCSC Level 1 control set. The 13 Level 1 controls are organized by their six ITSP.10.171 families, paired with plain-English descriptions, typical-evidence guidance, and an attestation field per control.

## Why this exists

CPCSC Level 1 became effective April 1, 2026 as a procurement gate for Canadian defence contracts. Public Services and Procurement Canada (PSPC) publishes the framework and provides an online self-assessment tool through the CanadaBuys supplier portal. No machine-readable artifact (CSV, spreadsheet, structured markdown) is published.

This repository fills that gap: a forkable, diff-friendly, vendor-neutral checklist that a procurement-readiness team can keep under version control alongside its other compliance documents.

## Files in this repository

- [`cpcsc-l1-controls.md`](cpcsc-l1-controls.md) — the main artifact. All 13 controls grouped by family, with descriptions, evidence guidance, and attestation fields.
- [`cpcsc-l1-controls.csv`](cpcsc-l1-controls.csv) — same content as CSV for spreadsheet import.
- [`SOURCES.md`](SOURCES.md) — canonical PSPC and CCCS source URLs.
- [`LICENSE`](LICENSE) — Apache License 2.0.

## How to use

1. Fork this repository or download the files.
2. Open `cpcsc-l1-controls.md` (or import `cpcsc-l1-controls.csv` into a spreadsheet).
3. For each control, determine whether your organization meets it as written. Set the **Status** field to `Compliant`, `Partial`, `Non-compliant`, or `N/A`.
4. Use the **Notes** field to record evidence location, owner, and last review date.
5. Re-attest annually or whenever the underlying systems change materially.

The CPCSC formal attestation happens through PSPC's online tool on the CanadaBuys portal. This repository is for internal readiness assessment, not a substitute for that submission.

## Scope and limits

This repository contains only public CPCSC framework content drawn from PSPC and CCCS source documents, plus a community usability layer (attestation fields, evidence guidance, organization-by-family layout). It does not contain proprietary content from any vendor.

Control descriptions in this repository are paraphrased plain-English summaries. The authoritative text is the PSPC Level 1 criteria page (linked in [`SOURCES.md`](SOURCES.md)). Issues and pull requests welcome to refine wording toward the verbatim PSPC source.

CPCSC Level 1 is not the same as Level 2, Level 3, ITSG-33, NIST SP 800-171, or any classified-environment accreditation regime. See [`SOURCES.md`](SOURCES.md) for the boundary lines.

## License

Apache License 2.0. See [`LICENSE`](LICENSE).

## Maintained by

Northfleet (`https://northfleet.tech`). Issues and pull requests welcome.

## Disclaimer

This template is provided as-is for internal self-assessment use. It is not a PSPC-endorsed or CCCS-endorsed assessment instrument. For authoritative guidance, refer to the source documents in [`SOURCES.md`](SOURCES.md).
