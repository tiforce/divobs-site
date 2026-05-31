# Billing Outsourcing Brief v0.1

DRAFT - legal and owner review required before any billing implementation.

## Purpose

This brief is for an external Stripe / SaaS billing vendor who may be asked to evaluate a future billing architecture for Divergence Observatory.

This document is preparation only. It does not approve implementation, live payments, checkout, subscription logic, APIs, authentication, databases, analytics, market data ingestion, LLM calls, or any external service integration.

## Project Summary

Divergence Observatory is a non-advisory market structure observatory. It is currently a static website with documentation and draft legal placeholder pages.

The project is compliance-first. Any future billing system must preserve the non-advisory boundary and must not change the product into an investment advisory service, trading signal service, stock recommendation service, portfolio advice service, or financial promotion promising outcomes.

## What Divergence Observatory Is

Divergence Observatory is intended to provide informational and educational market-structure context, including:

- divergence
- hidden stress
- cross-asset structure
- regime shifts
- volatility conditions
- macro/geopolitical transmission
- non-personalized educational and structural context

## What Divergence Observatory Is Not

Divergence Observatory is not:

- an investment advisory service
- a trading signal service
- a stock recommendation service
- a portfolio advice service
- a brokerage, exchange, fund, or asset manager
- a system for telling users what financial decision to make

It must not provide investment advice, personalized financial advice, buy/sell/hold recommendations, price targets, trade alerts, investment signals, individual stock recommendations, portfolio advice, or promises of profit or performance.

## Current Stage

The current project stage is static site only.

Current status:

- no live billing
- no Stripe integration
- no checkout flow
- no subscription logic
- no customer portal
- no invoice or receipt handling
- no payment webhooks
- no authentication
- no database
- no analytics
- no API calls
- no external services

## Future Billing Goal

The future goal is to evaluate a safe test-mode billing architecture only.

Any future vendor discussion should focus on how billing could be designed, documented, tested, reviewed, and approved before any production launch.

No production billing should be implemented without separate explicit approval from the project owner after legal, privacy, and compliance review.

## Required Future Components To Discuss

The vendor may be asked to discuss a future test-mode architecture for:

- Stripe Checkout test mode
- Stripe Billing test mode
- Customer Portal
- subscription lifecycle
- cancellation flow
- refund policy handling
- invoice / receipt handling
- webhook design
- environment variable handling
- test mode vs live mode separation
- production-readiness checklist
- privacy and customer data handling
- legal-page coordination, including Tokushoho / Specified Commercial Transactions Act disclosures if applicable

## Non-Advisory Requirements

The vendor must not introduce investment-advisory wording, trading-signal positioning, financial promotion language, urgency to act, outcome promises, or personalized suitability language.

Future billing copy must remain focused on access to informational and educational materials, not better financial outcomes or transaction decisions.

## Implementation Boundary

For the current engagement stage:

- Do not implement production billing.
- Do not add Stripe code.
- Do not add checkout.
- Do not add subscription logic.
- Do not add webhooks.
- Do not add API calls.
- Do not add authentication.
- Do not add databases.
- Do not add analytics or user tracking.
- Do not add market data ingestion.
- Do not add LLM calls.
- Do not add external services.

Any implementation work must be separately scoped, reviewed, and approved before it begins.

## Production-Readiness Checklist Topics

Before any future production launch, the project should complete:

- legal review of all billing and access copy
- legal review of terms, privacy, disclaimer, and Tokushoho pages
- privacy review for customer data handling
- Stripe test-mode verification
- cancellation flow verification
- refund policy review
- invoice and receipt handling review
- webhook failure and retry review
- environment variable and secret handling review
- production key handling process
- support workflow review
- owner approval for production launch

## Vendor Deliverable Expectation

At the planning stage, the preferred vendor deliverable is a written architecture and implementation plan, not production code.

The plan should identify:

- recommended Stripe products
- test-mode flow diagrams
- data handled by each component
- webhook events needed
- cancellation and refund behavior
- environment variables and secrets required
- files likely to change in a future implementation
- legal and privacy review dependencies
- production launch blockers

