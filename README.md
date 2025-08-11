# BioBot — Employee Bio Website Automation

> Streamlining employee biography collection, approval, and publication through automation.

This repository is a **sanitized, portfolio-style** overview of BioBot, a project developed during the InfusionPoints Summer 2025 internship program.  
It focuses on replacing a slow, manual Microsoft Teams + Excel process with a fully digital workflow leveraging GCP and AWS services.

> **Presentation Access:**  
> The full BioBot project presentation (PowerPoint) contains additional diagrams, architecture details, and implementation notes.  
> It is stored securely and kept private due to file size and confidentiality considerations.  
> I can present during interviews or portfolio reviews upon request.

## Problem
The previous bio collection process involved manual input, back-and-forth follow-ups, and inconsistent formatting. This led to delays, data gaps, and increased admin workload.

## Solution
- Digital bio submission forms via GCP prototype and AWS-native ambitions (Command Center Sandbox).
- DynamoDB for storage, Lambda for publishing to Drupal test sites.
- Approval/rejection stage with audit trail.
- Future plans for image handling via S3 and email approvals via SES.

## Impact
- Faster submission-to-publication time.
- Consistent, structured data.
- Reduced manual workload for administrators.
- Improved accuracy by removing copy/paste errors.
- Secure submissions with AWS Cognito (CC version).

## Tech & Tools
- **AWS:** DynamoDB, Lambda, SES, S3, Cognito
- **GCP:** Forms, Cloud Functions
- **Drupal:** Test and dummy site integration
- **Microsoft 365:** Legacy MVP version

## What's in this repo
- `docs/project_overview.md` — Detailed case study of the project phases, pivots, and technical architecture.
- `docs/lessons_learned.md` — Key takeaways from the project.
- `SECURITY.md` — Sanitization and privacy statement.

> No client data, production code, or sensitive credentials are included in this repository.
