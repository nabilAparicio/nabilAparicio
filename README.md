# Nabil Aparicio

**Senior Full-Stack Developer** — Panama City, UTC−5 · Remote contractor for US clients

I own product verticals end to end: web, mobile, and the platform underneath. TypeScript across the stack — React and Next.js on the web, React Native and Expo on mobile, services on Cloudflare Workers. Writing software since 2021.

[LinkedIn](https://www.linkedin.com/in/nabil-aparicio)

---

### What I build

Most of my current work is client-owned or private, so it is described here rather than linked.

**Multi-tenant HR & payroll SaaS** — sole author of the Next.js 16 web client (420 unit tests, 19 Playwright specs) and the Expo SDK 54 mobile app. Owned the API contract against a separate backend team across 81 endpoints. Built the realtime tier on Cloudflare Durable Objects: one Durable Object per tenant, so tenant isolation is structural rather than policy-enforced; HMAC-SHA256 on the internal channel with a replay window; and a delivery-report back-channel so push notifications fire only to users who were genuinely offline.

**Parametric quoting engine** — React 19 / Vite SPA, types generated from the backend's OpenAPI schema, ~2,693 tests. Engine-first by design: price comes from a deterministic engine and the LLM never computes or persists it.

**Three MCP servers on Cloudflare** — ~46,000 lines of TypeScript under ~1,480 tests. Each runs its own OAuth 2.1 authorization server instead of shipping a static key, with D1 persistence and Workers AI embeddings for semantic search.

**Data normalization pipeline** — 335 Excel workbooks spanning 2014 to 2026 across 23 distinct format families, into a medallion architecture with byte-for-byte reproducible runs. Every money-bearing row is either emitted or quarantined with a reason, and coverage floors in the test suite break the build on a data-losing regression.

### On AI

I build systems that use models, and I am deliberate about where a model is allowed to decide. Prices come from a deterministic engine, never an LLM. Extracted legal rules carry a verbatim source quote or they do not ship. Ambiguity gets flagged, never resolved. The scarce part is not using models — it is verification discipline over what they produce.

### Public work

- **[react-native-adaptive-bottom-sheet](https://github.com/nabilAparicio/react-native-adaptive-bottom-sheet)** — gesture-driven adaptive bottom sheet for React Native with keyboard avoidance. MIT, published to npm.
- **[itzelahernandez.com](https://itzelahernandez.com/en/)** — bilingual Astro site on Cloudflare Workers, with content verified against primary sources.

### Stack

`TypeScript` `React` `Next.js` `React Native` `Expo` `Node.js` `Hono` `Cloudflare Workers` `Durable Objects` `D1` `PostgreSQL` `Python` `pandas` `Astro` `Vite` `Tailwind` `Git`

---

Based in Panama City (UTC−5), fully overlapping US business hours.
Native Spanish · English C2 (EF SET 94/100).
