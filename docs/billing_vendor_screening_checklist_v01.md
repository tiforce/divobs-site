# Billing Vendor Screening Checklist v0.1

DRAFT - for vendor evaluation only.

## Purpose

Use this checklist to evaluate external vendors who may help design or implement a future billing / subscription system for Divergence Observatory.

This checklist does not approve live billing, Stripe integration, checkout, subscription logic, APIs, authentication, databases, analytics, market data ingestion, LLM calls, or external services.

## Project Boundary Questions

- Does the vendor understand that Divergence Observatory is a non-advisory market structure observatory?
- Can the vendor explain the difference between informational educational access and investment advisory positioning?
- Will the vendor avoid investment advice, buy/sell/hold recommendations, price targets, trade alerts, investment signals, stock recommendations, portfolio advice, and performance promises?
- Will the vendor avoid changing access copy into financial promotion language?
- Will the vendor wait for explicit approval before implementing any production billing?

## Stripe Checkout Experience

- Has the vendor implemented Stripe Checkout before?
- Can the vendor explain the difference between test mode and live mode?
- Can the vendor provide examples of test-mode checkout workflows they have built?
- Can the vendor explain how checkout success and cancellation URLs should be handled?
- Can the vendor describe how they prevent accidental use of live keys during testing?

## Stripe Billing / Subscription Experience

- Has the vendor implemented Stripe Billing subscriptions before?
- Can the vendor explain subscription lifecycle states?
- Can the vendor describe trial, active, past_due, canceled, and unpaid states?
- Can the vendor explain how subscription changes are handled?
- Can the vendor design the system without implying access to advisory or trading content?

## Customer Portal Experience

- Has the vendor configured Stripe Customer Portal before?
- Can the vendor explain what customers can manage in the portal?
- Can the vendor configure cancellation options safely?
- Can the vendor explain how plan changes, invoices, and payment methods are handled?
- Can the vendor document the portal configuration for handover?

## Webhook Reliability

- Which Stripe webhook events does the vendor expect to use?
- How will webhook signatures be verified?
- How will webhook retries and duplicate events be handled?
- How will failed webhook processing be monitored and recovered?
- How will the vendor document webhook event handling?

## Test Mode vs Live Mode Separation

- Can the vendor keep test mode and live mode fully separated?
- Will the vendor use test keys only until production approval?
- Can the vendor document a safe production switch process?
- Can the vendor identify all live-mode launch prerequisites?
- Does the vendor refuse to request production keys before they are needed?

## Environment Variables And Secret Handling

- How will Stripe keys and webhook secrets be stored?
- Which environment variables will be required?
- How will secrets be shared during development?
- How will production secrets be protected?
- Will the vendor avoid committing secrets or credentials to the repository?

## Cancellation And Refund Flows

- Can the vendor document cancellation behavior?
- Can the vendor document refund handling?
- Can the vendor explain how invoices and receipts are handled after cancellation or refund?
- Can the vendor coordinate wording with legal review?
- Can the vendor avoid creating access promises that exceed approved copy?

## Japanese Tokushoho / Legal-Page Coordination

- Does the vendor understand that Tokushoho / Specified Commercial Transactions Act disclosures may be required for paid services?
- Will the vendor coordinate with legal counsel before production launch?
- Will the vendor avoid publishing incomplete legal pages?
- Can the vendor identify billing copy that must be reviewed?
- Can the vendor support cancellation, refund, price, seller, and contact disclosure requirements if legally required?

## Privacy And Customer Data Handling

- What customer data will be collected?
- Where will customer data be stored?
- Which third parties will receive customer data?
- How will customer data deletion or correction requests be handled?
- Will the vendor avoid analytics or user tracking unless explicitly approved?

## Security Practices

- Does the vendor use least-privilege access?
- Does the vendor use secure secret handling?
- Does the vendor document deployment and rollback steps?
- Does the vendor avoid storing unnecessary payment data?
- Does the vendor follow Stripe security recommendations?

## Documentation Quality

- Will the vendor provide architecture documentation?
- Will the vendor provide setup instructions?
- Will the vendor provide test instructions?
- Will the vendor document required environment variables?
- Will the vendor document webhook behavior?
- Will the vendor document operational handover steps?

## Handover Process

- Will the vendor provide a clear handover checklist?
- Will the vendor identify all changed files?
- Will the vendor identify all external dashboard settings?
- Will the vendor provide test accounts or test scenarios?
- Will the vendor provide production launch blockers?

## Red Flags

- Vendor wants to implement live payments immediately.
- Vendor asks for production Stripe keys too early.
- Vendor proposes investment signal or trading alert language.
- Vendor proposes buy/sell/hold, target price, or stock-pick language.
- Vendor proposes analytics or user tracking without approval.
- Vendor does not document cancellation handling.
- Vendor does not document refund handling.
- Vendor cannot explain test mode vs live mode separation.
- Vendor wants to store unnecessary payment data.
- Vendor wants to skip legal, privacy, or Tokushoho review.
- Vendor frames paid access as better financial outcomes, privileged market insight, or transaction guidance.

## Initial Vendor Decision

Before selecting a vendor, confirm:

- non-advisory boundary understood
- test-mode-only planning accepted
- production billing approval required
- legal and privacy review dependencies accepted
- documentation and handover expectations accepted

