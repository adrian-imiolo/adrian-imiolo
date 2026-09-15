### Adrian Imioło — Full-Stack Developer (TypeScript) · Electrical Engineer

Electrical engineer with seven years in power plants, a gas terminal and wind-industry manufacturing; today I lead engineering change management at KK Group and build software alongside it. Self-taught in web development since 2022. Since January 2026 I ship complete products solo in TypeScript, with tests and CI, and in 2026 I did a three-month software engineering internship at LoveStack. I work in an AI-assisted workflow — Claude Code and Codex daily. Based in Szczecin, Poland.

---

#### 🛒 Sznyt Design — online shop, built solo

**[Live demo](https://shop-sznyt-design.vercel.app/)** · **[Source](https://github.com/adrian-imiolo/shop_sznyt_design)** · [sznytdesign.pl](https://www.sznytdesign.pl/) (placeholder until launch)

Since January 2026. A complete online shop for a designer picture-frame maker: product pages and cart, Stripe payments by card, BLIK and P24, InPost locker delivery, automatic emails at each step, and a phone-first admin panel.

- Try the full checkout in the demo — the storefront is in Polish, so add any frame to the basket and pay with Stripe test card `4242 4242 4242 4242`; no real money moves
- An order is recorded only once Stripe confirms the payment, never on a button click; stock decrements atomically in the same transaction, so a retried webhook cannot oversell
- Admin panel designed phone-first, because that is where the owner actually works
- No Shopify or WooCommerce — no monthly platform fees, and full control over how the brand is presented
- Launch on sznytdesign.pl is deferred until the real frames, photos and copy exist; the demo is the current public artifact

`React 19` `TypeScript` `Express` `Prisma` `PostgreSQL` `Stripe` `Clerk` `Tailwind CSS` `Vitest` `Playwright` `GitHub Actions`

---

#### 🎈 Twoja Dekoracja — site for an event-decoration business

**[twoja-dekoracja.pl](https://www.twoja-dekoracja.pl/)** · **[Source](https://github.com/adrian-imiolo/twoja-dekoracja)**

Live since September 2026. Portfolio and enquiry site for a Szczecin event-decoration business — weddings, birthdays and christenings — built for local search visibility.

- Portfolio, enquiry form and local SEO, built to do one job well
- Statically generated, so pages load instantly and hosting stays free
- Playwright suite runs against a real production build; without an email key the enquiry route writes to the server log, so CI needs no secrets

`Next.js` `React 19` `TypeScript` `Tailwind CSS` `Zod` `Resend` `Vitest` `Playwright` `GitHub Actions`

---

#### 📱 LoveStack — AI dating-coach app, live on the iOS App Store

**[App Store](https://apps.apple.com/app/lovestack-rizz-dating-coach/id6762365050)** · **[lovestack.com](https://lovestack.com)**

Software Engineering Intern · April – July 2026 · five-person engineering team

- **Owned the real-time AI video avatar end to end** — a lifelike character users hold a live, spoken conversation with. Ran the vendor research, wrote the spec, and implemented HeyGen's LiveAvatar with Gemini Live over LiveKit — including handling the user interrupting mid-sentence, and making sure sessions shut down cleanly and release the microphone. Built and demoed internally; not released publicly.
- **Built creator discovery and scoring** for the team's internal marketing tool: integrated a third-party social data API, added per-run cost controls, and covered it with tests against recorded responses.

The app is public; the code isn't.

`TypeScript` `React` `Convex` `Capacitor (iOS)` `LiveKit / WebRTC` `Gemini Live` `OpenAI` `Vercel AI SDK` `HeyGen` `RevenueCat` `Vitest`

---

#### Tech stack

- **Core:** TypeScript, JavaScript, SQL, HTML5, CSS3
- **Frontend:** React 19, Next.js, Tailwind CSS, Zod, Vite
- **Backend & data:** Node.js, Express, PostgreSQL, Prisma, Convex, REST, webhooks
- **AI & real-time:** Gemini Live, OpenAI, Vercel AI SDK, LiveKit / WebRTC, HeyGen; AI-assisted workflow with Claude Code, Codex, MCP
- **Platform & tooling:** Stripe, Clerk, Resend, RevenueCat, Capacitor (iOS), Git, GitHub Actions, Vitest, Playwright, Vercel

#### Engineering career

MEng in Electrical Engineering, Wrocław University of Science and Technology. Since 2018: protection testing and commissioning at KOGENERACJA's CHP plants, high-voltage operations at PSE, electrical engineering at the Grupa Azoty Polyolefins gas terminal, and since February 2025 leading engineering change management at KK Group across Denmark, Poland and India.

📫 adrian.imiolo11@gmail.com · [LinkedIn](https://www.linkedin.com/in/adrian-imiolo) · Polish native · English C1 · German A2
