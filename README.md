# CPCSC Level 1 self-assessment

An open-source self-assessment template for the Canadian Programme for Cyber Security Certification (CPCSC), Level 1.

## What this is

A working assessment artifact (Markdown for diff-friendliness, with companion `.csv` for spreadsheet import) that lets an organization self-attest against the CPCSC Level 1 control set. The 13 Level 1 controls decompose into approximately 70 individual determination statements grouped by their six ITSP.10.171 families. Each determination statement is a binary self-attestation criterion paired with organization-defined parameters (ODPs), assessment methods (Examine / Interview / Test), source assessment procedure references (NIST SP 800-171A Rev. 3 lineage), and a per-determination status field.

## Why this exists

CPCSC Level 1 became effective April 1, 2026 as a procurement gate for Canadian defence contracts. Public Services and Procurement Canada (PSPC) publishes the framework as a web page and provides an online self-assessment tool through the CanadaBuys supplier portal. No machine-readable artifact (CSV, spreadsheet, structured markdown) is published.

This repository fills that gap: a forkable, diff-friendly, vendor-neutral checklist that a procurement-readiness team can keep under version control alongside its other compliance documents.

## Files in this repository

- [`cpcsc-l1-controls.md`](cpcsc-l1-controls.md) — the main artifact. All 13 controls grouped by family, with verbatim determination statements, ODPs, assessment methods, and per-determination attestation fields.
- [`cpcsc-l1-controls.csv`](cpcsc-l1-controls.csv) — same content as CSV with one row per determination statement (~70 rows). Designed for spreadsheet import and GRC-tool ingestion.
- [`SOURCES.md`](SOURCES.md) — canonical PSPC and CCCS source URLs, plus the NIST SP 800-171A Rev. 3 lineage.
- [`LICENSE`](LICENSE) — Apache License 2.0.

## How to use

1. Fork this repository or download the files.
2. Open `cpcsc-l1-controls.md` (or import `cpcsc-l1-controls.csv` into a spreadsheet).
3. For each determination statement under each control, determine whether your organization meets the statement as written. Set the **Status** field to `Compliant`, `Partial`, `Non-compliant`, or `N/A`.
4. For controls with organization-defined parameters (ODPs), record your organization's values where the determination statement references them.
5. Use the **Evidence / notes** field to record where the supporting artifact lives, who owns it, and the date of last review.
6. Re-attest annually or whenever the underlying systems change materially.

The CPCSC formal attestation happens through PSPC's online tool on the CanadaBuys portal. This repository is for internal readiness assessment, not a substitute for that submission.

## Scope and limits

This repository contains only public CPCSC framework content drawn verbatim, where possible, from PSPC's published [Level 1 criteria page](https://www.canada.ca/en/public-services-procurement/services/industrial-security/security-requirements-contracting/cyber-security-certification-defence-suppliers-canada/cyber-security-certification-level1.html). Determination statements, ODPs, assessment methods, and source procedure references are taken from that page. The community usability layer added by this repository is limited to the Markdown table format, the per-determination status fields, and the evidence-notes field.

The underlying CPCSC Level 1 framework is based on the Canadian version of NIST SP 800-171A Rev. 3. There are no substantial technical changes between the Canadian document and the NIST source; differences reflect Canadian regulatory and compliance landscape only.

CPCSC Level 1 is not the same as Level 2, Level 3, ITSG-33, NIST SP 800-171, or any classified-environment accreditation regime. See [`SOURCES.md`](SOURCES.md) for the boundary lines.

## License

Apache License 2.0. See [`LICENSE`](LICENSE).

## Maintained by

Northfleet (`https://northfleet.tech`). Issues and pull requests welcome.

## Disclaimer

This template is provided as-is for internal self-assessment use. It is not a PSPC-endorsed or CCCS-endorsed assessment instrument. For authoritative guidance, refer to the source documents in [`SOURCES.md`](SOURCES.md).
