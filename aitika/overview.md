# Aitika – Div

> **Status:** Active Employment | Startup | Private Codebase  
> **Tech Stack:** Node.js • NestJS • GraphQL • Docker • Redis • BullMQ • Elasticsearch • Linux • CI/CD (GitHub Actions)  
> **Role:** Backend lead (3-person backend team) • Since Nov 2025

---

## Overview

Aitika is a startup building a commerce and marketplace platform with e-commerce at its core, evolving toward **marketplace** features (auctions, customer-submitted listings), plus integrations for **crypto payments** (Bitcoin, USDT, etc.), **blockchain/NFT** generation, **LLM-based legal contract** generation between parties, and **vision AI** for originality checks on custom products.

I joined as backend lead in a small backend team. The shop foundation (products, users, payments, multi-language, multi-currency, multiple payment methods) is fully implemented and in use; my focus has been on designing and implementing the most complex, high-value areas and on documentation and DevOps.

---

## Key Contributions

### E-commerce & Platform Foundation

- **E-commerce** - Products, users, payments, multi-language, multi-currency, and multiple payment gateways are implemented and functional.
- **Research & tooling** - Evaluated and adopted ready-made solutions for ~80% of shop needs, reducing custom code and delivery time.

### Auction & Listings (Design & Implementation)

- **Auction system** - Designed and implemented auctions, including concurrency handling and real-time updates.
- **Listing & verification** - Designed and implemented the Listing flow and related **finite state machines** for verification and visibility, with a path to integrate NFT minting and in-app transfers.

### Documentation & Onboarding

- **Client docs** - Admin and Android client documentation from day one.
- **Development guide** - For future maintainers and new devs: pain points, decisions and rationale, and what to be careful about.
- **Testing strategy** - Guidelines for future tests and priorities; documented how to use GraphQL introspection and which queries/mutations should be covered first (we moved fast and test coverage is still to be expanded).

### Integrations & UX

- **Deep links** - Android deep links so users return to the app after payment gateways or email confirmations instead of staying in the browser.

### DevOps & Infrastructure

- **CI/CD** - Full automated deployment with Docker and GitHub Actions.
- **Environments** - Separate servers and subdomains for dev, staging, and prod; Nginx, SSL (Certbot), GitHub Action user with minimal permissions and SSH-based deployment.

---

### 🔙 [Back to Project Index](../README.md)
