# AI SaaS Architecture

**Phase:** 4 (AI Product Company / SaaS)
**Status:** Active Execution Playbook

---

## 1. Architectural Philosophy
In Phase 4, you are moving away from custom client builds (Phase 1-3) into a multi-tenant, scalable, highly available SaaS infrastructure.
The goal is to serve 10,000 users as easily as 10 users, with a heavy emphasis on AI integration costs and latency.

## 2. The Tech Stack
- **Frontend:** Next.js (React), TailwindCSS.
- **Backend:** Node.js / Serverless functions.
- **Database:** PostgreSQL (Supabase or AWS RDS) with Row-Level Security (RLS) for multi-tenancy.
- **AI Infrastructure:** LangChain or custom prompt orchestration, Pinecone/Weaviate for vector storage.
- **Auth:** Clerk or Supabase Auth.
- **Payments:** Stripe Billing (Metered/Usage-based).

## 3. Multi-Tenancy Rules
- Every database table must have a `workspace_id` or `tenant_id`.
- Data must never leak between tenants. RLS must be enabled on the database layer, not just the application layer.

## 4. AI-Specific Architecture Rules
1. **Asynchronous by Default:** LLM calls take time. Never block the main thread. Use background queues (e.g., BullMQ, Inngest, or AWS SQS) for any AI task taking longer than 3 seconds. 
2. **Cost Tracking:** Tag every OpenAI/Anthropic API call with the `workspace_id`. You must know exactly how much each tenant costs you in AI compute to protect your margins.
3. **Caching:** Do not send the exact same prompt to OpenAI twice. Cache common AI responses in Redis to save money and reduce latency.
4. **Provider Agnostic:** Do not hardcode "OpenAI" deeply into your system. Use an abstraction layer so you can swap to Claude, Llama, or Gemini in minutes if an API goes down or changes pricing.

## 5. Scalability Strategy
1. **Database first:** 80% of scaling issues are slow database queries. Build proper indexes early.
2. **Edge caching:** Cache static assets and generic responses at the edge (Vercel/Cloudflare).
3. **Queue everything:** Offload heavy lifting (webhooks, email sending, AI generation) to worker queues.
