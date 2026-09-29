# CPCSC Level 1 controls

Thirteen mandatory self-attestation controls across six ITSP.10.171 families. Each control decomposes into one or more determination statements (lettered A.XX.XX.X); each determination statement is a binary attestation: Met or Not Met. The assessment is a self-attestation. Evidence is not submitted to PSPC at attestation time but must be retained and defensible.

This file is derived verbatim, where possible, from PSPC's published [Level 1 criteria page](https://www.canada.ca/en/public-services-procurement/services/industrial-security/security-requirements-contracting/cyber-security-certification-defence-suppliers-canada/cyber-security-certification-level1.html). Where wording is reformatted (Markdown tables instead of HTML), the underlying text is preserved. That text is Crown copyright and is not covered by this repository's Apache License 2.0; see [`NOTICE`](NOTICE) for its source and reproduction terms.

## How to use this file

Walk through each determination statement. For each:

1. Read the statement and any associated organization-defined parameter (ODP) values your organization has set.
2. Determine whether the statement is currently met in your environment.
3. Set the **Status** field to one of: `Compliant`, `Partial`, `Non-compliant`, or `N/A`.
4. In the **Evidence / notes** field, record where the supporting artifact lives, who owns it, and the date of last review.
5. Annually re-attest, or sooner if the underlying systems materially change.

The formal Level 1 self-assessment is completed with PSPC's online tool, or by another means, and its result and expiry date are confirmed in the supplier's CanadaBuys profile. This file is for internal readiness assessment, not a substitute for that submission.

## Contents

- [3.01 Access control](#301-access-control)
  - [03.01.01 — Account management](#030101--account-management)
  - [03.01.02 — Access enforcement](#030102--access-enforcement)
  - [03.01.20 — Use of external systems](#030120--use-of-external-systems)
  - [03.01.22 — Publicly accessible content](#030122--publicly-accessible-content)
- [3.05 Identification and authentication](#305-identification-and-authentication)
  - [03.05.01 — User identification, authentication, and re-authentication](#030501--user-identification-authentication-and-re-authentication)
  - [03.05.02 — Device identification and authentication](#030502--device-identification-and-authentication)
  - [03.05.03 — Multi-factor authentication](#030503--multi-factor-authentication)
- [3.08 Media protection](#308-media-protection)
  - [03.08.03 — Media sanitization](#030803--media-sanitization)
- [3.10 Physical protection](#310-physical-protection)
  - [03.10.01 — Physical access authorizations](#031001--physical-access-authorizations)
  - [03.10.07 — Physical access control](#031007--physical-access-control)
- [3.13 System and communications protection](#313-system-and-communications-protection)
  - [03.13.01 — Boundary protection](#031301--boundary-protection)
- [3.14 System and information integrity](#314-system-and-information-integrity)
  - [03.14.01 — Flaw remediation](#031401--flaw-remediation)
  - [03.14.02 — Malicious code protection](#031402--malicious-code-protection)

---

## 3.01 Access control

The controls in the Access control family support the ability to permit or deny user access to resources within the system.

### 03.01.01 — Account management

**Family:** Access control
**Source assessment procedures:** AC-02, AC-02(03), AC-02(05), AC-02(13)

#### Organization-defined parameters

| Parameter | Definition |
|---|---|
| A.03.01.01.ODP[01] | the time period for account inactivity before disabling is defined |
| A.03.01.01.ODP[02] | the time period within which to notify account managers and designated personnel or roles when accounts are no longer required is defined |
| A.03.01.01.ODP[03] | the time period within which to notify account managers and designated personnel or roles when users are terminated or transferred is defined |
| A.03.01.01.ODP[04] | the time period within which to notify account managers and designated personnel or roles when system usage or the need-to-know changes for an individual is defined |
| A.03.01.01.ODP[05] | the time period of expected inactivity requiring users to log out of the system is defined |
| A.03.01.01.ODP[06] | circumstances requiring users to log out of the system are defined |

#### Determination statements

| ID | Statement | Status | Evidence / notes |
|---|---|---|---|
| A.03.01.01.a[01] | system account types allowed are defined | _Pending_ | |
| A.03.01.01.a[02] | system account types prohibited are defined | _Pending_ | |
| A.03.01.01.b[01] | system accounts are created in accordance with organizational policy, procedures, prerequisites, and criteria | _Pending_ | |
| A.03.01.01.b[02] | system accounts are enabled in accordance with organizational policy, procedures, prerequisites, and criteria | _Pending_ | |
| A.03.01.01.b[03] | system accounts are modified in accordance with organizational policy, procedures, prerequisites, and criteria | _Pending_ | |
| A.03.01.01.b[04] | system accounts are disabled in accordance with organizational policy, procedures, prerequisites, and criteria | _Pending_ | |
| A.03.01.01.b[05] | system accounts are removed in accordance with organizational policy, procedures, prerequisites, and criteria | _Pending_ | |
| A.03.01.01.c.01 | authorized users of the system are specified | _Pending_ | |
| A.03.01.01.c.02 | group and role memberships are specified | _Pending_ | |
| A.03.01.01.c.03 | access authorizations (in other words, privileges) for each account are specified | _Pending_ | |
| A.03.01.01.d.01 | access to the system is authorized based on a valid access authorization | _Pending_ | |
| A.03.01.01.d.02 | access to the system is authorized based on intended system usage | _Pending_ | |
| A.03.01.01.e | the use of system accounts is monitored | _Pending_ | |
| A.03.01.01.f.01 | system accounts are disabled when the accounts have expired | _Pending_ | |
| A.03.01.01.f.02 | system accounts are disabled when the accounts have been inactive for <ODP[01]: time period> | _Pending_ | |
| A.03.01.01.f.03 | system accounts are disabled when the accounts are no longer associated with a user or individual | _Pending_ | |
| A.03.01.01.f.04 | system accounts are disabled when the accounts violate organizational policy | _Pending_ | |
| A.03.01.01.f.05 | system accounts are disabled when significant risks associated with individuals are discovered | _Pending_ | |
| A.03.01.01.g.01 | account managers and designated personnel or roles are notified within <ODP[02]: time period> when accounts are no longer required | _Pending_ | |
| A.03.01.01.g.02 | account managers and designated personnel or roles are notified within <ODP[03]: time period> when users are terminated or transferred | _Pending_ | |
| A.03.01.01.g.03 | account managers and designated personnel or roles are notified within <ODP[04]: time period> when system usage or the need-to-know changes for an individual | _Pending_ | |
| A.03.01.01.h | users are required to log out of the system after <ODP[05]: time period> of expected inactivity or when the following circumstances occur: <ODP[06]: circumstances> | _Pending_ | |

<details>
<summary>Assessment methods</summary>

**Examine:** access control policy and procedures; personnel termination or transfer policies and procedures; procedures for account management; list of active system accounts and the name of the individual associated with each account; system design documentation; list of conditions for group and role membership; system configuration settings; notifications of recent transfers, separations, or terminations of employees; list of recently disabled system accounts and the name of the individual associated with each account; list of user activities that pose significant organizational risks; access authorization records; account management compliance reviews; system monitoring and audit records; system security plan; privacy plan; system-generated list of accounts removed; system-generated list of emergency accounts disabled; system-generated list of disabled accounts; other relevant documents and records

**Interview:** personnel with account management responsibilities; system administrators; personnel with information security and privacy responsibilities; system developers

**Test:** processes for account management on the system; mechanisms for implementing account management

</details>

---

### 03.01.02 — Access enforcement

**Family:** Access control
**Source assessment procedure:** AC-03

#### Determination statements

| ID | Statement | Status | Evidence / notes |
|---|---|---|---|
| A.03.01.02[01] | approved authorizations for logical access to specified information are enforced in accordance with applicable access control policies | _Pending_ | |
| A.03.01.02[02] | approved authorizations for logical access to system resources are enforced in accordance with applicable access control policies | _Pending_ | |

<details>
<summary>Assessment methods</summary>

**Examine:** access control policy and procedures; procedures for access enforcement; system design documentation; system configuration settings; list of approved authorizations (in other words, user privileges); system audit records; system security plan; other relevant documents or records

**Interview:** personnel with access enforcement responsibilities; system administrators; personnel with information security responsibilities; system developers

**Test:** mechanisms for implementing the access control policy

</details>

---

### 03.01.20 — Use of external systems

**Family:** Access control
**Source assessment procedures:** AC-20, AC-20(01), AC-20(02)

#### Organization-defined parameter

| Parameter | Definition |
|---|---|
| A.03.01.20.ODP | security requirements to be satisfied on external systems prior to allowing the use of or access to those systems by authorized individuals are defined |

#### Determination statements

| ID | Statement | Status | Evidence / notes |
|---|---|---|---|
| A.03.01.20.a | the use of external systems is prohibited unless the systems are specifically authorized | _Pending_ | |
| A.03.01.20.b | the following security requirements to be satisfied on external systems prior to allowing the use of or access to those systems by authorized individuals are established: <ODP: security requirements> | _Pending_ | |
| A.03.01.20.c.01 | authorized individuals are permitted to use external systems to access the organizational system or to process, store, or transmit specified information only after verifying that the security requirements on the external systems as specified in the organization's system security plans have been satisfied | _Pending_ | |
| A.03.01.20.c.02 | authorized individuals are permitted to use external systems to access the organizational system or to process, store, or transmit specified information only after retaining approved system connection or processing agreements with the organizational entity hosting the external systems | _Pending_ | |
| A.03.01.20.d | the use of organization-controlled portable storage devices by authorized individuals on external systems is restricted | _Pending_ | |

<details>
<summary>Assessment methods</summary>

**Examine:** access control policy and procedures; procedures for the use of external systems; terms and conditions for the use of external systems; external systems security requirements; list of types of applications accessible from external systems; system configuration settings; system security plan; other relevant documents or records

**Interview:** personnel with responsibilities for defining terms, conditions, and security requirements for the use of external systems; personnel with information security responsibilities; system administrators

**Test:** mechanisms for implementing or enforcing terms, conditions, and security requirements for the use of external systems

</details>

---

### 03.01.22 — Publicly accessible content

**Family:** Access control
**Source assessment procedure:** AC-22

#### Determination statements

| ID | Statement | Status | Evidence / notes |
|---|---|---|---|
| A.03.01.22.a | authorized individuals are trained to ensure that publicly accessible information does not contain specified information | _Pending_ | |
| A.03.01.22.b[01] | the content on publicly accessible systems is reviewed for specified information | _Pending_ | |
| A.03.01.22.b[02] | specified information is removed from publicly accessible systems, if discovered | _Pending_ | |

<details>
<summary>Assessment methods</summary>

**Examine:** access control policy and procedures; procedures for publicly accessible content; list of users authorized to post publicly accessible content on organizational systems; training materials or records; records of publicly accessible information reviews; records of response to specified information discovered on public websites; system audit logs; security awareness training records; system security plan; other relevant documents or records

**Interview:** personnel with responsibilities for managing publicly accessible information posted on organizational systems; personnel with information security responsibilities

**Test:** mechanisms for implementing the management of publicly accessible content

</details>

---

## 3.05 Identification and authentication

The Identification and authentication controls support the unique identification of users, processes acting on behalf of users and devices. They also support the authentication or verification of the identities of those users, processes or devices as a prerequisite to allowing access to organizational systems.

### 03.05.01 — User identification, authentication, and re-authentication

**Family:** Identification and authentication
**Source assessment procedures:** IA-02, IA-11

#### Organization-defined parameter

| Parameter | Definition |
|---|---|
| A.03.05.01.ODP | circumstances or situations that require re-authentication are defined |

#### Determination statements

| ID | Statement | Status | Evidence / notes |
|---|---|---|---|
| A.03.05.01.a[01] | system users are uniquely identified | _Pending_ | |
| A.03.05.01.a[02] | system users are authenticated | _Pending_ | |
| A.03.05.01.a[03] | processes acting on behalf of users are associated with uniquely identified and authenticated system users | _Pending_ | |
| A.03.05.01.b | users are re-authenticated when <ODP: circumstances or situations> | _Pending_ | |

<details>
<summary>Assessment methods</summary>

**Examine:** identification and authentication policy and procedures; list of circumstances or situations requiring re-authentication; system design documentation; system configuration settings; system audit records; list of system accounts; system security plan; other relevant documents or records

**Interview:** personnel with identification and authentication responsibilities; personnel with system operations responsibilities; personnel with account management responsibilities; system developers; personnel with information security responsibilities; system administrators

**Test:** processes for uniquely identifying and authenticating users; mechanisms for supporting or implementing identification and authentication capabilities

</details>

---

### 03.05.02 — Device identification and authentication

**Family:** Identification and authentication
**Source assessment procedure:** IA-03

#### Organization-defined parameter

| Parameter | Definition |
|---|---|
| A.03.05.02.ODP | devices or types of devices to be uniquely identified and authenticated before establishing a connection are defined |

#### Determination statements

| ID | Statement | Status | Evidence / notes |
|---|---|---|---|
| A.03.05.02[01] | <ODP: devices or types of devices> are uniquely identified before establishing a system connection | _Pending_ | |
| A.03.05.02[02] | <ODP: devices or types of devices> are authenticated before establishing a system connection | _Pending_ | |

<details>
<summary>Assessment methods</summary>

**Examine:** identification and authentication policy and procedures; procedures for device identification and authentication; system design documentation; list of devices requiring unique identification and authentication; device connection reports; system configuration settings; system security plan; other relevant documents or records

**Interview:** personnel with responsibilities for device identification and authentication; personnel with information security responsibilities; system developers; system administrators

**Test:** mechanisms for supporting or implementing device identification and authentication capabilities

</details>

---

### 03.05.03 — Multi-factor authentication

**Family:** Identification and authentication
**Source assessment procedures:** IA-02(01), IA-02(02)

#### Determination statements

| ID | Statement | Status | Evidence / notes |
|---|---|---|---|
| A.03.05.03[01] | strong multi-factor authentication for access to privileged accounts is implemented | _Pending_ | |
| A.03.05.03[02] | strong multi-factor authentication for access to non-privileged accounts is implemented | _Pending_ | |

<details>
<summary>Assessment methods</summary>

**Examine:** identification and authentication policy and procedures; system design documentation; list of system accounts; system configuration settings; system audit records; system security plan; other relevant documents or records

**Interview:** personnel with system operations responsibilities; personnel with account management responsibilities; personnel with information security responsibilities; system developers; system administrators

**Test:** mechanisms for supporting or implementing a multi-factor authentication capability

</details>

---

## 3.08 Media protection

The Media protection controls support the protection of system media throughout their lifecycle. They help limit access to information on system media to authorized users and sanitize or destroy system media before disposal or release for reuse.

### 03.08.03 — Media sanitization

**Family:** Media protection
**Source assessment procedure:** MP-06

#### Determination statements

| ID | Statement | Status | Evidence / notes |
|---|---|---|---|
| A.03.08.03 | system media that contain specified information are sanitized prior to disposal, release out of organizational control, or release for reuse | _Pending_ | |

<details>
<summary>Assessment methods</summary>

**Examine:** media protection policy and procedures; procedures for media sanitization and disposal; applicable standards and policies that address media sanitization policy; system audit records; media sanitization records; system design documentation; system configuration settings; records retention and disposition policy; records retention and disposition procedures; system security plan; privacy plan; other relevant documents or records

**Interview:** personnel with media sanitization responsibilities; personnel with records retention and disposition responsibilities; personnel with information security and privacy responsibilities; system administrators

**Test:** processes for media sanitization; mechanisms for supporting or implementing media sanitization

</details>

---

## 3.10 Physical protection

The Physical protection controls support the control of physical access to systems, equipment, and the respective operating environments to authorized individuals. They facilitate the protection of the physical plant and support infrastructure for systems, the protection of systems against environmental hazards, and provide appropriate environmental controls in facilities containing systems.

### 03.10.01 — Physical access authorizations

**Family:** Physical protection
**Source assessment procedure:** PE-02

#### Organization-defined parameter

| Parameter | Definition |
|---|---|
| A.03.10.01.ODP | the frequency at which to review the access list detailing authorized physical access by individuals is defined |

#### Determination statements

| ID | Statement | Status | Evidence / notes |
|---|---|---|---|
| A.03.10.01.a[01] | a list of individuals with authorized access to the facility where the system resides is developed | _Pending_ | |
| A.03.10.01.a[02] | a list of individuals with authorized access to the facility where the system resides is approved | _Pending_ | |
| A.03.10.01.a[03] | a list of individuals with authorized access to the facility where the system resides is maintained | _Pending_ | |
| A.03.10.01.b | authorization credentials for facility access are issued | _Pending_ | |
| A.03.10.01.c | the physical access list is reviewed <ODP: frequency> | _Pending_ | |
| A.03.10.01.d | individuals from the physical access list are removed when access is no longer required | _Pending_ | |

<details>
<summary>Assessment methods</summary>

**Examine:** physical protection policy and procedures; procedures for physical access authorizations; authorized personnel access list; physical access list reviews; physical access termination records; authorization credentials; system security plan; other relevant documents or records

**Interview:** personnel with physical access authorization responsibilities; personnel with physical access to the facility where the system resides; personnel with information security responsibilities

**Test:** processes for physical access authorizations; mechanisms for supporting or implementing physical access authorizations

</details>

---

### 03.10.07 — Physical access control

**Family:** Physical protection
**Source assessment procedures:** PE-03, PE-05

#### Determination statements

| ID | Statement | Status | Evidence / notes |
|---|---|---|---|
| A.03.10.07.a.01 | physical access authorizations are enforced at entry and exit points to the facility where the system resides by verifying individual physical access authorizations before granting access | _Pending_ | |
| A.03.10.07.a.02 | physical access authorizations are enforced at entry and exit points to the facility where the system resides by controlling ingress and egress with physical access control systems, devices, or guards | _Pending_ | |
| A.03.10.07.b | physical access audit logs for entry or exit points are maintained | _Pending_ | |
| A.03.10.07.c[01] | visitors are escorted | _Pending_ | |
| A.03.10.07.c[02] | visitor activity is controlled | _Pending_ | |
| A.03.10.07.d | keys, combinations, and other physical access devices are secured | _Pending_ | |
| A.03.10.07.e | physical access to output devices is controlled to prevent unauthorized individuals from obtaining access to specified information | _Pending_ | |

<details>
<summary>Assessment methods</summary>

**Examine:** physical protection policy and procedures; procedures for physical access control; physical access control logs or records; inventory records of physical access control devices; system entry and exit points; records of key and lock combination changes; storage locations for physical access control devices; physical access control devices; list of security safeguards controlling access to designated publicly accessible areas within facility; system security plan; other relevant documents or records

**Interview:** personnel with physical access control responsibilities; personnel with information security responsibilities

**Test:** processes for physical access control; mechanisms for supporting or implementing physical access control; physical access control devices

</details>

---

## 3.13 System and communications protection

The System and communications protection controls support the monitoring, control and protection of the systems themselves and of the communications between and within the systems.

### 03.13.01 — Boundary protection

**Family:** System and communications protection
**Source assessment procedure:** SC-07

#### Determination statements

| ID | Statement | Status | Evidence / notes |
|---|---|---|---|
| A.03.13.01.a[01] | communications at external managed interfaces to the system are monitored | _Pending_ | |
| A.03.13.01.a[02] | communications at external managed interfaces to the system are controlled | _Pending_ | |
| A.03.13.01.a[03] | communications at key internal managed interfaces within the system are monitored | _Pending_ | |
| A.03.13.01.a[04] | communications at key internal managed interfaces within the system are controlled | _Pending_ | |
| A.03.13.01.b | subnetworks are implemented for publicly accessible system components that are physically or logically separated from internal networks | _Pending_ | |
| A.03.13.01.c | external system connections are only made through managed interfaces that consist of boundary protection devices arranged in accordance with an organizational security architecture | _Pending_ | |

<details>
<summary>Assessment methods</summary>

**Examine:** system and communications protection policy and procedures; procedures for boundary protection; list of key internal boundaries within the system; boundary protection hardware and software; system configuration settings; security architecture; system audit records; system design documentation; enterprise security architecture documentation; system security plan; other relevant documents or records

**Interview:** personnel with boundary protection responsibilities; personnel with information security responsibilities; system developers; system administrators

**Test:** mechanisms for implementing boundary protection capabilities

</details>

---

## 3.14 System and information integrity

The System and information integrity controls support the protection of the integrity of the system components and the data that it processes. They allow an organization to identify, report and correct data and system flaws in a timely manner, to provide protection against malicious code, and to monitor system security alerts and advisories, and to take appropriate actions in response.

### 03.14.01 — Flaw remediation

**Family:** System and information integrity
**Source assessment procedure:** SI-02

#### Organization-defined parameters

| Parameter | Definition |
|---|---|
| A.03.14.01.ODP[01] | the time period within which to install security-relevant software updates after the release of the updates is defined |
| A.03.14.01.ODP[02] | the time period within which to install security-relevant firmware updates after the release of the updates is defined |

#### Determination statements

| ID | Statement | Status | Evidence / notes |
|---|---|---|---|
| A.03.14.01.a[01] | system flaws are identified | _Pending_ | |
| A.03.14.01.a[02] | system flaws are reported | _Pending_ | |
| A.03.14.01.a[03] | system flaws are corrected | _Pending_ | |
| A.03.14.01.b[01] | security-relevant software updates are installed within <ODP[01]: time period> of the release of the updates | _Pending_ | |
| A.03.14.01.b[02] | security-relevant firmware updates are installed within <ODP[02]: time period> of the release of the updates | _Pending_ | |

<details>
<summary>Assessment methods</summary>

**Examine:** system and information integrity policy and procedures; procedures for flaw remediation; procedures for configuration management; list of recent security flaw remediation actions performed on the system; list of flaws and vulnerabilities that may potentially affect the system; test results from the installation of software and firmware updates to correct system flaws; installation and change control records for security-relevant software and firmware updates; system security plan; privacy plan; other relevant documents or records

**Interview:** personnel responsible for installing, configuring, or maintaining the system; personnel responsible for flaw remediation; personnel with configuration management responsibilities; personnel with information security and privacy responsibilities; system administrators

**Test:** processes for identifying, reporting, and correcting system flaws; processes for installing software and firmware updates; mechanisms for supporting or implementing the reporting and correction of system flaws; mechanisms for supporting or implementing the testing software and firmware updates

</details>

---

### 03.14.02 — Malicious code protection

**Family:** System and information integrity
**Source assessment procedure:** SI-03

#### Organization-defined parameter

| Parameter | Definition |
|---|---|
| A.03.14.02.ODP | the frequency at which malicious code protection mechanisms perform scans is defined |

#### Determination statements

| ID | Statement | Status | Evidence / notes |
|---|---|---|---|
| A.03.14.02.a[01] | malicious code protection mechanisms are implemented at system entry and exit points to detect malicious code | _Pending_ | |
| A.03.14.02.a[02] | malicious code protection mechanisms are implemented at system entry and exit points to eradicate malicious code | _Pending_ | |
| A.03.14.02.b | malicious code protection mechanisms are updated as new releases are available in accordance with configuration management policy and procedures | _Pending_ | |
| A.03.14.02.c.01[01] | malicious code protection mechanisms are configured to perform scans of the system <ODP: frequency> | _Pending_ | |
| A.03.14.02.c.01[02] | malicious code protection mechanisms are configured to perform real-time scans of files from external sources at endpoints or system entry and exit points as the files are downloaded, opened, or executed | _Pending_ | |
| A.03.14.02.c.02 | malicious code protection mechanisms are configured to block or quarantine malicious code, or take other mitigation actions in response to malicious code detection | _Pending_ | |

<details>
<summary>Assessment methods</summary>

**Examine:** system and information integrity policy and procedures; configuration management policy and procedures; procedures for malicious code protection; records of malicious code protection updates; system design documentation; system configuration settings; scan results from malicious code protection mechanisms; record of actions initiated by malicious code protection mechanisms in response to malicious code detection; system audit records; system security plan; other relevant documents or records

**Interview:** personnel responsible for malicious code protection; personnel with system installation, configuration, or maintenance responsibilities; personnel with information security responsibilities; system administrators

**Test:** processes for employing, updating, and configuring malicious code protection mechanisms; processes for addressing the detection of false positives and resulting potential impacts; mechanisms for supporting or implementing, employing, updating, and configuring malicious code protection mechanisms; mechanisms for supporting or implementing malicious code scanning and the execution of subsequent actions

</details>
