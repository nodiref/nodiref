# NodiRef · Referral Engine as a Service ⚡️

Add a production-ready referral program to your SaaS in **under 5 minutes**.  
NodiRef is API-first, fraud-resistant, and completely free for small and side-projects.

<p align="center">
  <a href="https://nodiref.com">Website</a> ·
  <a href="https://docs.nodiref.com/docs/platform">Docs</a> ·
  <a href="https://docs.nodiref.com/docs/api/introduction">API Docs</a> ·
  <a href="https://docs.nodiref.com/docs/platform/setup">Quick Start</a>
</p>

---

## Key Features

| Feature | What it means for you |
| ------- | -------------------- |
| **API-First & Developer Friendly** | Control every aspect of your referral program via a fully documented REST API or JavaScript SDK. |
| **Drop-in Integration** | Two endpoints (or one script tag) and you’re live—maintenance on us. |
| **Reward Management System** | Create flexible rule sets to grant fixed or percentage-based rewards, complete with caps and webhooks for payouts. |
| **Partner Management** | On-board influencers, customers, or friends; track performance by project or campaign. |
| **Fraud Detection** | Automatic flagging of suspicious conversions with rich IP, device, and geo metadata so you stay in control. |
| **Actionable Analytics** | Detailed stats for every referral, partner, and campaign—no extra setup needed. |
| **Generous Free Tier** | Side-projects get 1 project, 20 partners, 5 monthly conversions, and fraud protection—no credit card required. |

---

## Quick Start

> **1. Sign up & grab your API key**  
> Create a free account at <https://app.nodiref.com> and copy your **Project ID** and **Secret API Key**.
>
> **2. Import the JavaScript SDK on your front** (client-side)  
> ```html
> <script
>   src="https://cdn.nodiref.com/nodiref-sdk.js"
>   async
> ></script>
> <script>
>   nodiRef("identify", "PARTNER_ID"); // Optional: identify logged-in partner
> </script>
> ```
>
> **3. Track events**  
> ```js
> // Click (handled automatically if you pass the referral code)
> nodiRef("track", "click", "REFERRAL_CODE");
>
> // New user signed up
> nodiRef("referral", "USER_EXTERNAL_ID");
>
> // Conversion (purchase or subscription)
> nodiRef("track", "conversion", {
>   referral_id: "REFERRAL_ID",
>   event_type: "purchase",
>   payload: { amount: 49, currency: "USD", product_id: "PRO_123" }
> });
> ```
>
> **4. Configure rewards**  
> In the dashboard: **Settings → Reward Rule Sets** → New Rule Set, then define triggers & rewards (fixed or percentage).
>
> **5. Go live!**  
> Share the generated referral links with your partners and watch conversions roll in.

To get more detailed specifics, you can check our [documentation](https://docs.nodiref.com/docs/platform).

---

## Core Concepts

| Concept | Summary |
| ------- | ------- |
| **Project** | Top-level container for settings (API keys, landing domain, default reward rules). |
| **Partner** | The advocate promoting your product; each partner can have multiple links. |
| **Referral Link** | Unique link with a referral code pointing to your landing page. |
| **Conversion** | A monetizable action (purchase, subscription, etc.) performed by a referred user. |
| **Reward Rule Set** | Logic that determines when and how rewards are issued. |

See the [docs](https://docs.nodiref.com) for detailed payloads, status flows, and advanced configuration.

---

## Pricing

We offer a forever-free version for small and side projects.

---

## Roadmap

We’re feedback-driven—open an issue to up-vote or propose a feature!

---

> Made with ☕ in Europe — © 2025 NodifyIt · All rights reserved.
