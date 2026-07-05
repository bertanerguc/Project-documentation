# ECUNOVAX

**Automotive dealer portal — Turkey & MENA region**

A full-stack B2B platform connecting automotive dealerships with buyers,
enabling inventory management, lead generation, and digital sales workflows.
Built and shipped by a solo founder. Currently live and generating revenue.

> **Note:** Source code is private — the platform is live in production.
> This repository serves as project documentation.
> Repository: [bertanerguc/Project-documentation](https://github.com/bertanerguc/Project-documentation)

---

## Overview

ECUNOVAX is an automotive dealer portal built for the Turkish and MENA market.
The platform enables dealerships to manage inventory, receive qualified leads,
and digitize their sales process — replacing phone-based and walk-in-only workflows.

**Status:** Live · Revenue generating · $20K+ in processed transactions

---

## Features

**For Dealerships**
- Inventory management dashboard — list, edit, and manage vehicle stock
- Lead management CRM — track inquiries, follow-ups, and conversions
- Analytics — views, inquiries, conversion rates by listing
- Multi-user access — sales team collaboration

**For Buyers**
- Advanced search & filtering — make, model, year, price, mileage, location
- Saved searches and favorites
- Direct dealer inquiry with response tracking

---

## Tech Stack

| Layer | Technology |
|---|---|
| Backend | Python · Django · Django REST Framework |
| Frontend | React · JavaScript · CSS |
| Database | PostgreSQL |
| Infrastructure | DigitalOcean · Nginx · Gunicorn |
| Storage | DigitalOcean Spaces (S3-compatible) |
| Auth | JWT · Django Auth |

---

## Architecture

```
┌─────────────────────────────────────────┐
│              React Frontend              │
│         (Dealer Dashboard + Buyer UI)    │
└──────────────────┬──────────────────────┘
                   │ REST API
┌──────────────────▼──────────────────────┐
│           Django REST Framework          │
│    (Auth · Inventory · Leads · Search)   │
└──────────────────┬──────────────────────┘
                   │
┌──────────────────▼──────────────────────┐
│              PostgreSQL                  │
│     (Dealers · Listings · Inquiries)     │
└─────────────────────────────────────────┘
         │                    │
  DigitalOcean            DigitalOcean
    Droplet                 Spaces
  (App Server)           (Image Storage)
```

---

## Key Metrics

- **$20K+** in processed dealer transactions
- **Bootstrapped** — zero external funding
- **Solo-built** — design, backend, frontend, DevOps
- **Live in production** on DigitalOcean infrastructure

---

## Lessons Learned

Building ECUNOVAX as a solo founder shaped the technical foundation
I now bring to Altitude Holdings:

- **Django at scale** — multi-tenant architecture, query optimization, caching
- **React complexity** — state management, real-time updates, mobile UX
- **DevOps reality** — CI/CD pipelines, server management, zero-downtime deploys
- **B2B product thinking** — dealer workflows are complex; simplicity wins
- **Revenue before perfection** — shipped v1 in 8 weeks, iterated from real feedback

---

## About the Builder

**Bertan Ergüç** — Co-Founder & CTO, Altitude Holdings

Full-stack developer with an MBA in Finance.
ECUNOVAX was my proof that I can build, ship, and generate revenue from zero.
Now applying the same approach to property intelligence at Altitude Holdings.

[LinkedIn](https://linkedin.com/in/bertan-erguc-b621b4195) ·
[GitHub](https://github.com/bertanerguc) ·
[Altitude Holdings](https://altitudeholdings.com)
