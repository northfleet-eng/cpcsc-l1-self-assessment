# CPCSC Level 1 controls

Thirteen mandatory self-attestation controls across six ITSP.10.171 families. Each control is binary at Level 1: Met or Not Met. The assessment is a self-attestation. Evidence is not submitted to PSPC at attestation time but must be retained and defensible.

## How to use this file

Fork or download. For each control:

1. Read the description and the typical-evidence guidance.
2. Determine whether your organization currently meets the control as written.
3. Set the **Status** field to one of: `Compliant`, `Partial`, `Non-compliant`, or `N/A`.
4. Use the **Notes** field to record where the evidence lives, who owns it, and the date of last review.
5. Re-review annually and update.

## On the source text

Control descriptions in this file are paraphrased plain-English summaries derived from PSPC's Level 1 criteria page and the underlying CCCS technical standard ITSP.10.171. The canonical PSPC page (`https://www.canada.ca/en/public-services-procurement/services/industrial-security/security-requirements-contracting/cyber-security-certification-defence-suppliers-canada/cyber-security-certification-level1.html`) is the authoritative text. Issues and pull requests welcome to refine wording toward the verbatim source.

Verification notes:
- Control IDs, family groupings, family counts (4 / 3 / 1 / 2 / 1 / 2), and the binary attestation model are verified against PSPC, the Standards Council of Canada release, and corroborating Canadian legal-firm and security-firm analyses.
- One secondary source proposes a different family split (4 / 2 / 1 / 2 / 2 / 2). The split used in this file is the canonical version per PSPC and SCC.

---

## Access Control (4)

### 03.01.01: Account Management

**Family:** Access Control
**Description:** Create, modify, review, disable, and remove system accounts so only authorized identities have access.
**Typical evidence:**
- Joiner / mover / leaver standard operating procedure
- Account inventory (system-by-system)
- Periodic access-review records

**Status:** _Pending_
**Notes:** _record evidence location, owner, last review date_

---

### 03.01.02: Access Enforcement

**Family:** Access Control
**Description:** Enforce approved authorizations for logical access by users and processes. Apply least-privilege and role-based access principles.
**Typical evidence:**
- RBAC matrix
- ACL or group-policy exports
- Deny-by-default configuration evidence

**Status:** _Pending_
**Notes:** _record evidence location, owner, last review date_

---

### 03.01.20: Use of External Systems

**Family:** Access Control
**Description:** Set terms for the use of external and personal systems and cloud services that touch specified information.
**Typical evidence:**
- Acceptable-use policy
- Approved-SaaS list
- BYOD / MDM configuration

**Status:** _Pending_
**Notes:** _record evidence location, owner, last review date_

---

### 03.01.22: Publicly Accessible Content

**Family:** Access Control
**Description:** Control what is posted to public-facing systems so specified information is never exposed.
**Typical evidence:**
- Content-review workflow
- Designated approvers list
- Periodic public-site scans for sensitive content

**Status:** _Pending_
**Notes:** _record evidence location, owner, last review date_

---

## Identification and Authentication (3)

### 03.05.01: User Identification and Authentication

**Family:** Identification and Authentication
**Description:** Uniquely identify and authenticate every user before granting access.
**Typical evidence:**
- Identity provider or directory records of unique accounts
- Policy banning shared accounts
- Authentication logs

**Status:** _Pending_
**Notes:** _record evidence location, owner, last review date_

---

### 03.05.02: Device Identification and Authentication

**Family:** Identification and Authentication
**Description:** Identify and authenticate devices before they connect to systems handling specified information.
**Typical evidence:**
- Device inventory
- 802.1X or certificate-based network access control configuration
- MDM enrolment records

**Status:** _Pending_
**Notes:** _record evidence location, owner, last review date_

---

### 03.05.03: Multifactor Authentication

**Family:** Identification and Authentication
**Description:** Require multifactor authentication for privileged accounts and for remote or network access to systems handling specified information.
**Typical evidence:**
- MFA enrolment report from identity provider
- Conditional-access policies
- Screenshot or configuration export showing enforcement scope

**Status:** _Pending_
**Notes:** _record evidence location, owner, last review date_

---

## Media Protection (1)

### 03.08.03: Media Sanitization

**Family:** Media Protection
**Description:** Sanitize or destroy media containing specified information before disposal, release, or reuse.
**Typical evidence:**
- Sanitization standard operating procedure referencing NIST SP 800-88 or CCCS ITSP.40.006
- Destruction certificates
- Disposal log

**Status:** _Pending_
**Notes:** _record evidence location, owner, last review date_

---

## Physical Protection (2)

### 03.10.01: Physical Access Authorizations

**Family:** Physical Protection
**Description:** Maintain a list of personnel authorized to enter facilities housing systems with specified information. Issue and revoke credentials accordingly.
**Typical evidence:**
- Authorized-personnel roster
- Badge-issuance log
- Termination revocation records

**Status:** _Pending_
**Notes:** _record evidence location, owner, last review date_

---

### 03.10.07: Physical Access Control

**Family:** Physical Protection
**Description:** Enforce physical access at entry and exit points. Mechanisms include locks, badges, guards, and visitor escorts.
**Typical evidence:**
- Badge-reader logs
- Visitor log with escort signatures
- Photos or documentation of controlled entry points

**Status:** _Pending_
**Notes:** _record evidence location, owner, last review date_

---

## System and Communications Protection (1)

### 03.13.01: Boundary Protection

**Family:** System and Communications Protection
**Description:** Monitor, control, and protect communications at external boundaries and key internal boundaries of the systems handling specified information.
**Typical evidence:**
- Firewall rule export
- Network diagram with trust zones
- Egress filtering configuration

**Status:** _Pending_
**Notes:** _record evidence location, owner, last review date_

---

## System and Information Integrity (2)

### 03.14.01: Flaw Remediation

**Family:** System and Information Integrity
**Description:** Identify, report, and correct system flaws in a timely manner.
**Typical evidence:**
- Vulnerability-scan reports
- Patch SLA policy
- Patch-deployment evidence (WSUS, Intune, Jamf, or equivalent)

**Status:** _Pending_
**Notes:** _record evidence location, owner, last review date_

---

### 03.14.02: Malicious Code Protection

**Family:** System and Information Integrity
**Description:** Deploy and maintain malicious-code protection on endpoints and gateways.
**Typical evidence:**
- AV / EDR console showing coverage across the in-scope environment
- Definition-update logs
- Detection and quarantine records

**Status:** _Pending_
**Notes:** _record evidence location, owner, last review date_
