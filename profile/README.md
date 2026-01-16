# Asymmetric.al

**Small inputs. Mountain-moving outputs.**

Asymmetric.al builds mission-critical software for organizations doing hard, meaningful work.  
Our platform reduces operational drag, unifies fragmented systems, and gives small teams disproportionate leverage.

This GitHub organization contains the core platform, supporting applications, and public-facing surfaces that together represent the Asymmetric.al ecosystem.

---

## What We’re Building

Asymmetric.al is a **multi-tenant, mission-focused software platform** built with a servant-first philosophy.

The platform enables organizations to:
- Operate admins, field workers, and supporters from a single system
- Maintain strict tenant isolation and data security
- Integrate payments, communications, analytics, and content workflows
- Scale responsibly without sacrificing clarity or control

The architecture is intentionally opinionated: strong defaults, fewer moving parts, and systems designed for long-term stewardship.

---

## Repository Overview

### `core`
**The primary production platform**

A Next.js, multi-tenant application that powers:
- Mission Control (operations and administration)
- Field-worker dashboards
- Donor and supporter portals
- Organization-specific public sites

**Key characteristics**
- Next.js App Router (RSC-first)
- Supabase (Postgres, Auth, Storage, RLS)
- Stripe for payments
- Playwright E2E testing (accessibility, performance, and reliability)
- Clear separation of features, providers, and infrastructure

This repository is the center of gravity for product development.

---

### `asymmetric.al`
**Public-facing website and interaction layer**

The official Asymmetric.al website and client-facing surface.  
This repo represents how the platform is introduced, explained, and experienced from the outside.

It is used to:
- Communicate the mission, product, and philosophy
- Showcase platform capabilities and integrations
- Provide interactive, lightweight experiences without full platform coupling
- Serve as a fast-moving surface for content, experimentation, and iteration

This codebase prioritizes clarity, speed, and approachability over deep backend integration.

---

## Architectural Principles

- **Multi-tenant by default**  
  A single deployment safely serving many organizations.

- **Data isolation is foundational**  
  Row-level security and explicit tenant boundaries are mandatory.

- **Small inputs → large leverage**  
  Automation and AI augmentation are used to amplify human effort.

- **Servant-first systems**  
  Software exists to reduce burden, not add it.

- **Production realism**  
  Testing, observability, and failure modes are part of design—not afterthoughts.

---

## Technology Stack (High Level)

- **Frontend:** React, Next.js, Vite
- **Backend:** Supabase (Postgres, Auth, Storage)
- **Payments:** Stripe
- **Email:** SendGrid
- **Observability:** Sentry
- **Testing:** Playwright (E2E, accessibility, performance)
- **Styling:** Tailwind, shadcn/ui
- **Runtime:** Bun / Node.js

---

## Who This Is For

- Engineers contributing to the Asymmetric.al platform
- Partners building integrations or extensions
- Internal teams operating and evolving mission infrastructure

This is not a general-purpose framework.  
It is a focused system built to solve specific, real-world problems well.

---

## Contributing

Each repository includes its own setup and development instructions.

Organization-wide expectations:
- Read the repo’s README before coding
- Never commit secrets
- Run linting and tests before opening a PR
- Favor clarity over cleverness

Formal contribution standards will evolve alongside the platform.

---

## Status

Asymmetric.al is under active development.  
Some repositories are production-grade; others are intentionally exploratory.

Expect iteration.

---

## Philosophy

> Build less.  
> Choose carefully.  
> Ship things that matter.

If you’re here, you’re likely building something important.  
We take that seriously.
