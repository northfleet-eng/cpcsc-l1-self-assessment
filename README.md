# CPCSC Level 1 self-assessment

An open-source self-assessment template for the Canadian Program for Cyber Security Certification (CPCSC), Level 1.

## What this is

A working assessment artifact (Markdown for diff-friendliness, with a companion `.csv` for spreadsheet import) that lets an organization self-attest against the CPCSC Level 1 control set. The 13 Level 1 controls decompose into 71 determination statements grouped by their six ITSP.10.171 families. Each determination statement is a binary self-attestation criterion paired with organization-defined parameters (ODPs), assessment methods (Examine / Interview / Test), source assessment procedure references (NIST SP 800-171A Rev. 3 lineage), and a per-determination status field.

## Why this exists

Public Services and Procurement Canada (PSPC) made CPCSC Level 1 available to suppliers on April 1, 2026 and is adding it to select defence contracts from summer 2026, required at contract award. PSPC publishes the Level 1 criteria as a web page and provides an online self-assessment tool; suppliers confirm the result in their CanadaBuys profile. Neither PSPC nor the Canadian Centre for Cyber Security (CCCS) publishes the criteria as CSV or a spreadsheet.

This repository fills that gap: a forkable, diff-friendly, vendor-neutral checklist that a procurement-readiness team can keep under version control alongside its other compliance documents.

## Files in this repository

- [`cpcsc-l1-controls.md`](cpcsc-l1-controls.md): the main artifact. All 13 controls grouped by family, with verbatim determination statements, ODPs, assessment methods, and per-determination attestation fields.
- [`cpcsc-l1-controls.csv`](cpcsc-l1-controls.csv): the 71 determination statements as CSV, one row per statement, with Status and Evidence / Notes columns. ODPs and assessment methods are in the Markdown file only.
- [`SOURCES.md`](SOURCES.md): canonical PSPC and CCCS source URLs, plus the NIST SP 800-171A Rev. 3 lineage.
- [`LICENSE`](LICENSE): Apache License 2.0, for this repository's own material.
- [`NOTICE`](NOTICE): the source and reproduction terms of the Government of Canada text.

## How to use

1. Fork this repository or download the files.
2. Open `cpcsc-l1-controls.md` (or import `cpcsc-l1-controls.csv` into a spreadsheet).
3. For each determination statement under each control, determine whether your organization meets the statement as written. Set the **Status** field to `Compliant`, `Partial`, `Non-compliant`, or `N/A`.
4. For controls with organization-defined parameters (ODPs), record your organization's values where the determination statement references them.
5. Use the **Evidence / notes** field to record where the supporting artifact lives, who owns it, and the date of last review.
6. Re-attest annually or whenever the underlying systems change materially.

The formal Level 1 self-assessment is completed with PSPC's online tool, or by another means, and its result and expiry date are confirmed in the supplier's CanadaBuys profile. This repository is for internal readiness assessment, not a substitute for that submission.

## Scope and limits

The Government of Canada content here is reproduced verbatim from PSPC's [Level 1 criteria page](https://www.canada.ca/en/public-services-procurement/services/industrial-security/security-requirements-contracting/cyber-security-certification-defence-suppliers-canada/cyber-security-certification-level1.html): determination statements, ODPs, assessment methods, source procedure references, and family descriptions. The community usability layer added by this repository is limited to the Markdown table format, the CSV layout, the per-determination status fields, and the evidence-notes field.

The underlying CPCSC Level 1 framework is based on the Canadian version of NIST SP 800-171A Rev. 3. There are no substantial technical changes between the Canadian document and the NIST source; differences reflect Canadian regulatory and compliance landscape only.

CPCSC Level 1 is not the same as Level 2, Level 3, the ITSP.10.033 series (formerly ITSG-33), NIST SP 800-171, or any classified-environment accreditation regime. See [`SOURCES.md`](SOURCES.md) for the boundary lines.

## License

The repository's own material is under the Apache License 2.0 ([`LICENSE`](LICENSE)). The reproduced Government of Canada text is not: it is Crown copyright, reproduced under the Canada.ca Terms and conditions, which do not permit commercial redistribution without the Government of Canada's written permission. [`NOTICE`](NOTICE) gives the source and the terms.

## Maintained by

Northfleet ([northfleetsecurity.ca](https://northfleetsecurity.ca)). Issues and pull requests welcome.

## Disclaimer

This template is provided as-is for internal self-assessment use. It is not a PSPC-endorsed or CCCS-endorsed assessment instrument. For authoritative guidance, refer to the source documents in [`SOURCES.md`](SOURCES.md).
