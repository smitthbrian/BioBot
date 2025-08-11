# BioBot — Project Overview

## Context
Interns were initially tasked with collecting employee website bios using spreadsheets. The team saw an opportunity to improve efficiency, reduce errors, and streamline approvals.

## Goals
- Automate the workflow end-to-end.
- Improve data integrity and formatting consistency.
- Add approval and rejection tracking.
- Reduce manual work for administrators.

## Phases & Pivots
1. **Microsoft Stack MVP** — Early version using Microsoft Forms and Power Automate.
2. **GCP Prototype** — Addressed licensing limits and allowed image uploads.
3. **AWS + Command Center Sandbox** — Expanded capabilities, added DynamoDB storage, Lambda publishing to Drupal, SES email approvals, and S3 for image handling.

## Technical Architecture
- **GCP version:** Form → Cloud Function → Test Drupal Site.
- **AWS version:** CC Sandbox Form → DynamoDB (bio data) → Lambda (publish to Drupal) → S3 (images) → SES (approvals/rejections) → Cognito (secure submissions).

## Challenges & Solutions
- **Licensing costs for Microsoft connectors** → Switched to GCP/AWS stack.
- **Image uploads blocked by Google login requirements** → Added image upload option for approvers.
- **Limited website access** → Created Drupal dummy site for testing.

## Expected Impact
- Faster turnaround from submission to publication.
- Consistent, structured, auditable data.
- Reduction in copy/paste errors.
- Secure and scalable process.

## Next Steps
- Add timestamp as sort key for DynamoDB.
- Implement S3 image upload and Lambda attachment handling.
- Expand SES approval capabilities (multi-approver, rejection handling).
- Improve validation and feedback for submitters.
- Enable updates for existing bios.