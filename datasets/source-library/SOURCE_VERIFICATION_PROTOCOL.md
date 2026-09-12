# Source Verification Protocol

## 1. Purpose

This protocol defines the minimum evidence required to verify aviation regulatory sources used by the Aviation Safety Regulations project.

It prevents:

- Unofficial sources from being treated as controlling requirements
- Superseded documents from being used for audit decisions
- Guidance from being misclassified as mandatory regulation
- Approval status from being confused with approved scope
- Unverified information from being classified as compliant or non-compliant

## 2. Scope

This protocol applies to sources related to:

- AMO / Part-145 approval
- Aircraft maintenance
- Safety Management Systems
- Continuing Airworthiness
- Maintenance personnel
- Quality and compliance monitoring
- Audit findings
- Root Cause Analysis
- Corrective and Preventive Action
- Effectiveness verification

Covered authorities:

- ICAO
- CAAV
- FAA
- EASA
- CAAM
- CAAP
- MOLIT/KOCA
- JCAB

## 3. Verification Principles

1. The issuing authority or official legislation portal is the preferred source.
2. A search result is not regulatory evidence.
3. A document title alone does not confirm applicability.
4. The applicable provision must be read in context.
5. Mandatory requirements must be separated from guidance.
6. Approval status and approved scope must be verified separately.
7. Translation uncertainty must be recorded.
8. Missing information must remain visible.
9. A source must not be marked current without checking amendment status.
10. Regulatory applicability is not the same as organisational compliance.

## 4. Required Verification Fields

A source cannot receive `VERIFIED — CURRENT` status unless the following fields are completed:

| Field | Required |
|---|---|
| Source ID | Yes |
| Authority | Yes |
| Official document title | Yes |
| Document number | Yes |
| Regulatory classification | Yes |
| Revision or edition | Yes |
| Issue or publication date | Where available |
| Effective date | Yes |
| Amendment status | Yes |
| Applicable provision | Yes |
| Applicability | Yes |
| Official source URL | Yes |
| Verification date | Yes |
| Verified by | Yes |
| Open issue | Must be resolved or clearly controlled |

## 5. Source Classification

Each source must be classified as one of the following:

| Classification | Meaning |
|---|---|
| Law / Act | Primary legislation |
| Regulation | Mandatory regulatory requirement |
| Implementing Rule | Detailed mandatory implementation requirement |
| Approval Condition | Organisation-specific mandatory approval condition |
| AMC | Acceptable Means of Compliance |
| GM | Guidance Material |
| Advisory Circular | Authority guidance |
| Order / Inspector Policy | Internal or published authority oversight policy |
| User Guide / Work Instruction | Administrative implementation guidance |
| Certificate | Evidence of approval status |
| Scope / OpSpecs / Terms of Approval | Evidence of approved scope and limitations |
| Organisation Manual | Approved organisational system and procedures |
| Technical Standard | Recognised technical or industry standard |
| Research | Academic or professional analysis |
| Reference Only | Non-controlling supporting information |

## 6. Source Priority

| Priority | Source type | Permitted use |
|---|---|---|
| P0 | Official law, regulation, decision, certificate or scope record | Primary regulatory and approval evidence |
| P1 | Official AMC, GM, AC, order, user guide or authority instruction | Interpretation and implementation support |
| P2 | Recognised technical or industry standard | Technical criteria where applicable |
| P3 | Peer-reviewed research or professional analysis | Background and analytical support |
| P4 | General or unofficial source | Source discovery only |

A P4 source must not be used as the sole basis for an audit finding.

## 7. Verification Workflow

### Step 1 — Identify

Record:

- Authority
- Jurisdiction
- Document title
- Document number
- Regulatory subject

### Step 2 — Locate

Locate the source through:

1. Official legislation portal
2. Official authority website
3. Official regulatory database
4. Official certificate or approval database

If unavailable, record `NOT LOCATED`.

### Step 3 — Authenticate

Confirm:

- Issuing body
- Official URL or official record
- Document identity
- Language and translation status

### Step 4 — Confirm Currency

Check:

- Revision or edition
- Amendment history
- Effective date
- Repeal or supersession status
- Transitional provisions

### Step 5 — Classify

Determine whether the source is:

- Mandatory
- Approval-specific
- Acceptable means of compliance
- Guidance
- Technical standard
- Research
- Reference only

### Step 6 — Assess Applicability

Record:

- Covered organisation
- Covered activity
- Jurisdiction
- Aircraft or product scope
- Locations
- Conditions
- Exclusions
- Interfaces with other approvals

### Step 7 — Extract Relevant Provision

Record the exact:

- Article
- Section
- Paragraph
- Clause
- Appendix or form

Do not rely only on a summary.

### Step 8 — Record Evidence

Enter the verified information in:

```text
datasets/source-library/MASTER_SOURCE_REGISTER.md
