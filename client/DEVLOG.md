## Day 1 — 2026-05-07

**Hours worked:** 6.5

**What I did:**

- Read the full assignment carefully and broke the project down into product, engineering, and business requirements instead of treating it like only a coding task.
- Researched the core problem Credex is solving: startups and engineering teams overspending on AI subscriptions, API usage, and overlapping tooling without visibility into optimization opportunities.
- Studied existing tools in adjacent categories including SaaS spend management, AI cost monitoring, and subscription optimization platforms to understand what already exists and where this product can differentiate.
- Researched pricing structures and official pricing pages for:
  - Cursor
  - GitHub Copilot
  - Claude
  - ChatGPT
  - OpenAI API
  - Anthropic API
  - Gemini
  - Windsurf/v0
- Started building `PRICING_DATA.md` with official source URLs and verification dates for every pricing number used in the audit engine.
- Identified early optimization patterns and audit logic opportunities:
  - Teams paying for enterprise/admin plans with very small seat counts
  - Overlapping coding assistants (Cursor + Copilot simultaneously)
  - Companies paying API costs when subscription plans would be cheaper
  - Redundant subscriptions across research/writing workflows
  - Opportunities where discounted infrastructure credits could reduce recurring API spend
- Defined the product positioning as a lightweight “AI Spend Auditor” focused on fast recommendations and shareable audit results instead of deep infrastructure analytics.
- Initialized the project repository and configured:
  - Next.js (App Router)
  - TypeScript
  - Tailwind CSS
  - ESLint
- Installed initial dependencies and tooling:
  - React Hook Form
  - Zod
  - Supabase client
  - Resend
  - Lucide React
  - clsx + tailwind-merge
  - Vitest
- Created the initial project structure:
  - `/app`
  - `/components`
  - `/lib`
  - `/tests`
  - `/types`
- Created all required evaluation markdown files at the repository root:
  - README.md
  - ARCHITECTURE.md
  - DEVLOG.md
  - REFLECTION.md
  - TESTS.md
  - PRICING_DATA.md
  - PROMPTS.md
  - GTM.md
  - ECONOMICS.md
  - USER_INTERVIEWS.md
  - LANDING_COPY.md
  - METRICS.md
- Drafted the initial architecture and data flow for how a user input becomes:
  - audit recommendations
  - savings calculations
  - AI-generated summaries
  - shareable public reports
- Created the first version of the audit engine structure and started outlining recommendation rules for plan downgrades, tool consolidation, and credit-based optimization opportunities.
- Added GitHub repository setup and started organizing commits using conventional commit naming.
- Planned the 7-day implementation roadmap to prioritize:
  1. audit engine
  2. result UX
  3. backend + shareability
  4. AI summaries
  5. documentation and testing

**What I learned:**

- AI tooling spend is highly fragmented across subscriptions and APIs, making it difficult for startups to understand their actual monthly AI costs.
- Many AI pricing models are optimized for larger organizations, which creates inefficient spending patterns for smaller startups using enterprise or team plans too early.
- The strongest value of this product is not “AI recommendations,” but financially defensible procurement reasoning.
- Existing products mainly focus on enterprise SaaS management or API observability, while there is still room for a lightweight, startup-focused AI spend optimization tool with viral/shareable UX.
- The assignment heavily emphasizes entrepreneurial thinking, product judgment, documentation quality, and decision-making process — not just frontend implementation.

**Blockers / what I'm stuck on:**

- Defining credible thresholds for when team or enterprise plans become justified across different vendors.
- Deciding how aggressive the audit recommendations should be without reducing user trust.
- Finding a clean way to model “tool overlap” without making recommendations feel subjective or opinion-based.

**Plan for tomorrow:**

- Build the spend input form UI
- Add form persistence using localStorage
- Create typed pricing schemas and audit engine models
- Implement the first set of recommendation rules
- Begin writing automated tests for the audit logic



## Day 2 — 2026-05-08

- took a day off because of tommorow is my semester exam  i will continue from day 3 night 