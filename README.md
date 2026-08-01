### Adrian Imioło — Software Engineer, Full Stack / AI

TypeScript, React, Node. I build and ship whole products end-to-end — frontend, backend, data model, payments, deployment. Based in Szczecin, Poland.

---

#### 🛒 Sznyt Design — solo e-commerce platform

**[Live demo](https://shop-sznyt-design.vercel.app)** · **[Source](https://github.com/adrian-imiolo/shop_sznyt_design)**

A custom e-commerce platform built and operated end-to-end by one developer. No Shopify, no WooCommerce.

**You can complete a real checkout in the demo** — Stripe **test mode**, card `4242 4242 4242 4242`. No real money moves. The order is recorded by the Stripe webhook in Postgres and read back on the confirmation page.

- Stripe webhook is the single source of truth for payment state; `stripeSessionId` is the idempotency key
- Stock decrements atomically inside a database transaction, only on payment confirmation
- 219 unit tests + a DB-backed integration suite that runs in CI **with zero repository secrets** — auth, payments and mail are injected into the app factory, so CI exercises real routing, real queries and real transaction boundaries
- A real legal constraint shapes the data model: the shop trades under Polish *działalność nierejestrowana*, so there is no VAT invoice, no NIP field, and a quarterly revenue-cap tracker in the admin
- Architecture decisions (ADRs), domain model and operational runbooks live alongside the code

`React 19` `TypeScript` `Express 5` `Prisma` `PostgreSQL` `Stripe` `Clerk` `Tailwind` `Vitest` `Playwright` `GitHub Actions`

---

#### 📱 LoveStack — AI iOS app, live on the App Store

**[App Store](https://apps.apple.com/app/lovestack-rizz-dating-coach/id6762365050)** · **[lovestack.com](https://lovestack.com)**

Software engineer, part-time, Jan 2025 – Jul 2026.

- **Owned** the flagship real-time AI video "talking avatar" end-to-end, pre-release — a lifelike persona you talk to live, from multi-vendor evaluation through a working build. LiveKit/WebRTC video, HeyGen lip-sync, Gemini Live voice.
- **Part of the team** building a live consumer AI product — React frontend, Convex backend, iOS via Capacitor — plus AI content generation and the subscription/entitlement layer.

The app is public; the code isn't. Happy to go deep on the architecture in conversation.

`TypeScript` `React` `Convex` `Capacitor` `LiveKit/WebRTC` `Gemini` `OpenAI` `RevenueCat` `Vitest`

---

📫 adrian.imiolo11@gmail.com · [LinkedIn](https://www.linkedin.com/in/adrian-imiolo)
