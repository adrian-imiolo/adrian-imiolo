### Adrian Imioło — Software Engineer, Full Stack / AI

TypeScript, React, Node. I build and ship whole products end-to-end — frontend, backend, data model, payments, deployment. Based in Szczecin, Poland.

---

#### 📱 LoveStack — AI iOS app, live on the App Store

**[App Store](https://apps.apple.com/app/lovestack-rizz-dating-coach/id6762365050)** · **[lovestack.com](https://lovestack.com)**

Software engineer, Sep 2024 – Jul 2026.

- **Owned** the real-time AI video "talking avatar" end-to-end — a lifelike persona you talk to live. Multi-vendor evaluation across video, lip-sync and voice, then integration into a working build: LiveKit/WebRTC video, HeyGen lip-sync, Gemini Live voice. Built and demoed internally; not released publicly.
- **Part of the team** building a live consumer AI product — React frontend, Convex backend, iOS via Capacitor — plus AI content generation and the subscription/entitlement layer.

The app is public; the code isn't. Happy to go deep on the architecture in conversation.

`TypeScript` `React` `Convex` `Capacitor` `LiveKit/WebRTC` `Gemini` `OpenAI` `RevenueCat` `Vitest`

---

#### 🛒 Sznyt Design — solo e-commerce platform

**[Live demo](https://shop-sznyt-design.vercel.app)** · **[Source](https://github.com/adrian-imiolo/shop_sznyt_design)**

A custom e-commerce platform built and operated end-to-end by one developer. No Shopify, no WooCommerce.

**You can complete a real checkout in the demo** — Stripe **test mode**, card `4242 4242 4242 4242`. No real money moves. The order is recorded by the Stripe webhook in Postgres and read back on the confirmation page. The storefront is in Polish; add any product to the basket and check out to see the payment path.

- Stripe webhook is the single source of truth for payment state; `stripeSessionId` is the idempotency key
- Stock decrements atomically inside the same database transaction that marks the order paid — a retried or out-of-order webhook cannot double-fulfil or oversell
- A DB-backed integration suite runs in CI **with zero repository secrets** — auth, payments and mail are injected into the app factory, so CI exercises real routing, real queries and real transaction boundaries
- A real legal constraint shapes the data model: the shop trades under Polish *działalność nierejestrowana*, so there is no VAT invoice, no NIP field, and a quarterly revenue-cap tracker in the admin
- Architecture decisions (ADRs), domain model and operational runbooks live alongside the code

`React 19` `TypeScript` `Express 5` `Prisma` `PostgreSQL` `Stripe` `Clerk` `Tailwind` `Vitest` `Playwright` `GitHub Actions`

---

📫 adrian.imiolo11@gmail.com · [LinkedIn](https://www.linkedin.com/in/adrian-imiolo)
