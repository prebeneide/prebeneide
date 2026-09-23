# Hi 👋 I'm Preben

Front-end developer from Noroff, graduated with an A in the final project exam and
portfolio assessment. I build products and take them the whole way — data model, APIs,
real-time audio and video, payments, App Store release and operations — for my own
products and for clients.

Most of what I build lives in private repositories, so the contribution graph on this page
shows the volume rather than the code: **2,152 contributions over the past year, across
125 active days.** Happy to walk through any of it, or share code on request.

## Selected work

| Project | What it is | Built with |
|---|---|---|
| **AIQINITY** | SaaS platform where companies describe what they need in a chat and get a working internal application with its own domain, billing and hosting. Includes a desktop agent written in Rust with a sandbox, a hash-chained audit log and keys in the OS keychain. | Rust, Tauri, Next.js, TypeScript, Supabase, Stripe |
| **Resepsjon.ai** | AI agent that answers incoming calls for businesses. Real-time audio on a self-hosted server, answers from the customer's own documents with RAG, and escalates to a human when it shouldn't answer alone. | Next.js, TypeScript, LiveKit, Twilio, RAG |
| **[TreatMeHome](https://apps.apple.com/no/app/treatmehome/id6762602518)** | Marketplace app for home-based services. Booking, Stripe payments, and a map that handles thousands of live points without stalling. iOS, Android and web from one codebase. | Flutter, Riverpod, Supabase, Stripe |
| **[Roomr](https://apps.apple.com/no/app/roomr-just-knock-hang-out/id6761539251)** | Social app where friends each have a virtual room. Real-time audio and video over WebRTC, with native call handling through CallKit and ConnectionService. | Flutter, Node.js, PostgreSQL, WebRTC, LiveKit |
| **[Steppin](https://github.com/prebeneide/GetSteppin)** | Activity app for iOS and Android reading motion data straight from the device sensors. Daily goals, friends, leaderboards and charts. Source is public. | React Native, Expo, TypeScript, Supabase |
| **mAIdoctor** | Health app where the conversation remembers the user's history over time, with structured programmes and PDF reports to bring to a doctor's appointment. | React Native, Expo, TypeScript, Supabase |

## AIQINITY — describe it, and it gets built

You write what you need in plain language. The platform asks what it still needs to know,
writes the code, runs it against a real database and puts it online. Below: a webshop with
28 products, categories, search, cart and an admin panel — built and then refined in the
same conversation.

<img src="bilder/nordfisk-nettbutikk.png" alt="AIQINITY building a fishing tackle webshop with categories, search and cart">

<p>
<img src="bilder/autoelite-bilbutikk.png" width="49%" alt="A car dealership site built from a one-line brief">
<img src="bilder/massageme-massasjeklinikk.png" width="49%" alt="A clinic landing page with a booking form">
</p>

The stack is Next.js and TypeScript on Supabase, with Stripe for billing and per-customer
domains. The part I'm most proud of is the desktop agent: about 3,100 lines of Rust that
let you talk to your own Mac from your phone and have it carry out tasks, with a sandbox
around what it may touch, keys in the OS keychain, and a SHA-256 hash-chained audit log
sealed with HMAC, so every action can be verified afterwards.

## Resepsjon.ai — an AI agent that answers the phone

<img src="bilder/resepsjon.png" alt="Resepsjon.ai — AI customer service agent">

Incoming and outgoing calls through Twilio, real-time audio on a LiveKit server I run
myself, and answers drawn from the customer's own documents with RAG. The hard part was
never getting it to answer. It was deciding what it must not handle alone, and handing the
call to a human in time.

## On the App Store

### TreatMeHome — book a service, get it done at home

<p>
<img src="https://is1-ssl.mzstatic.com/image/thumb/PurpleSource221/v4/0c/c3/e6/0cc3e65b-40fa-eef8-43ab-b79814bcb34d/IMG_8789.PNG/400x0w.png" width="170" alt="Browse and filter services">
<img src="https://is1-ssl.mzstatic.com/image/thumb/PurpleSource221/v4/ee/f2/4a/eef24a2b-cb40-569f-f1d9-1277be9c5913/IMG_8792.PNG/400x0w.png" width="170" alt="Provider profile with live map">
<img src="https://is1-ssl.mzstatic.com/image/thumb/PurpleSource211/v4/2c/9b/79/2c9b7963-801d-54ff-775f-536f59237756/IMG_8795.PNG/400x0w.png" width="170" alt="Pick a date and a time slot">
<img src="https://is1-ssl.mzstatic.com/image/thumb/PurpleSource211/v4/fa/03/25/fa032558-0d27-da6e-05cd-cd644317ea1c/IMG_8798.PNG/400x0w.png" width="170" alt="Booking summary and payment">
</p>

Built from idea to published app: Flutter for iOS, Android and web, Supabase for data and
auth, Stripe for payments, and a clustered map that stays smooth with thousands of points.

### Roomr — knock on a friend's door

<p>
<img src="https://is1-ssl.mzstatic.com/image/thumb/PurpleSource221/v4/94/6c/6b/946c6ba4-3a89-220f-6e40-7ab76411f194/IMG_7943.PNG/400x0w.png" width="170" alt="Your friends' rooms">
<img src="https://is1-ssl.mzstatic.com/image/thumb/PurpleSource221/v4/46/39/53/4639533e-6eec-7e55-2dd7-f6c40a74738a/IMG_7979.PNG/400x0w.png" width="170" alt="Someone knocks to come in">
<img src="https://is1-ssl.mzstatic.com/image/thumb/PurpleSource211/v4/8b/d5/08/8bd50808-2f86-d2d8-9303-3a8b57e5dce3/IMG_7967.PNG/400x0w.png" width="170" alt="Live audio and video in a room">
<img src="https://is1-ssl.mzstatic.com/image/thumb/PurpleSource221/v4/4e/15/f1/4e15f110-baf7-5c48-afec-5f3abf27ad83/IMG_7959.PNG/400x0w.png" width="170" alt="Open or lock your own room">
</p>

Version 1.0: open and locked rooms, knocking, presence and notifications, with real-time
audio and video over WebRTC and native call handling through CallKit and ConnectionService.

## Tech

**Frontend** — TypeScript, JavaScript, React, Next.js, Vue, HTML, CSS, SCSS, Tailwind, Bootstrap, Styled Components, shadcn/ui, responsive and mobile-first

**Mobile** — React Native, Expo, Expo Router, Flutter, Riverpod, CallKit and ConnectionService, push notifications

**Backend & data** — Node.js, Fastify, Express, REST APIs, GraphQL, Supabase, PostgreSQL, MongoDB, Firebase, Stripe, NextAuth, Python

**AI & real-time** — OpenAI, Anthropic Claude, RAG, WebRTC, LiveKit, Twilio

**Systems** — Rust, Tauri, WebContainers, xterm.js, CodeMirror 6, SHA-256 and HMAC

**E-commerce & CMS** — Shopify (Admin, themes, apps, Storefront API, headless), WooCommerce, WordPress, headless CMS

**Tooling & deployment** — Git, GitHub, Vercel, Netlify, VS Code, monorepos

## Background

I've been building for the web since my teens and writing code since 2020. Before the
code came hundreds of websites and online stores, for clients and for my own business
ideas. Most of it has been built alongside full-time work outside the industry.

I rarely meet a problem I think is impossible. It's usually about finding another way in,
and I don't stop until I've found it.

## 📫 Contact

**prebenfjeldsbo@gmail.com**
