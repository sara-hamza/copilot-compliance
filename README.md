# copilot-compliance

## What it does

Compliance Reviewer: obligations, risks, dates, ambiguities and questions for legal from policies, contracts and procedures.

Part of the **department-copilots** suite: local-only copilots where the employee provides the input, Claude analyses it on the machine, and the employee decides what to do. No CRM, NMS, email or system integrations.

## Install

```bash
claude plugin marketplace add sara-hamza/department-copilots
```

```bash
claude plugin install compliance@department-copilots
```

Drop in a contract, policy or procedure (PDF, DOCX or pasted text) and get back a structured review: obligations, risks, dates, responsibilities, ambiguities, missing information and questions for legal, every item with a clause or page reference.

| Command | Use when |
|---|---|
| `/compliance:review <paste or drop the document>` | Full review: OBLIGATIONS / RISKS / DATES / RESPONSIBILITIES / AMBIGUITIES / MISSING INFORMATION / QUESTIONS FOR LEGAL |
| `/compliance:obligations <paste or drop the document>` | Obligations register table only (Clause, Obligation, Owner, Due/Trigger, Evidence) |
| `/compliance:questions <paste or drop the document>` | Review questions only, grouped by topic, for the drafter or counterparty |

Requires `copilot-common` (document-reader for PDFs and DOCX).

This is not legal advice. Outputs are for review by qualified staff. The reviewer organises what the document says and flags what to check; it does not decide whether to sign, accept or waive anything.

Reference knowledge lives in `skills/compliance-reviewer/references/`. the company's risk appetite thresholds, approval limits and the legal contact are marked `CUSTOMISE`.
