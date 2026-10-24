# Marketing Creative Repository Review — 2026-10-24

This is a discovery and triage record, not a security audit. Popularity is a discovery signal, not proof of quality. Re-check current release, license, dependency security, and commercial terms before deployment.

## High-priority candidate: reusable marketing skills

### coreyhaines31/marketingskills
- Source: https://github.com/coreyhaines31/marketingskills
- Use: copywriting, social content, Meta/Google/LinkedIn ads, ad creative iteration, analytics, conversion tracking, SEO.
- Evidence reviewed: repository README and version index on 2026-10-24. The project documents MIT licensing and support for agents such as OpenAI Codex and other Agent Skills-compatible environments.
- Setup: repository documents CLI/plugin installation for compatible coding agents; these commands do not install skills into the ChatGPT Android app.
- Commercial use: MIT license is permissive, subject to its terms and notices.
- Caveats: skills may assume a coding-agent environment or terminal. Review each instruction, platform policy, and brand fit. Adapt rather than blindly execute any actions.

## Social scheduling and publishing: evaluate, do not install on Android

### gitroomhq/postiz-app
- Source: https://github.com/gitroomhq/postiz-app
- Use: multi-platform social scheduling, collaboration, analytics, API and automation integrations.
- License: AGPL-3.0, confirmed in repository README.
- Maintenance/security evidence: release page showed v2.25.2 dated 2026-10-23 and noted that it addresses a security vulnerability PSA-2026-JNXM56; deployments should use a fixed current release and review the advisory before exposure.
- Setup: self-hosted Node.js/Next.js/NestJS/PostgreSQL/Temporal stack; not suitable for installation directly on a low-storage Android phone.
- Commercial use: AGPL obligations can affect modified/network-served deployments; obtain appropriate legal review for intended use.
- Decision: watchlist for a future server or managed deployment, not an immediate phone install.

## Analytics and experimentation: evaluate for web funnels

### PostHog/posthog
- Source: https://github.com/PostHog/posthog
- Use: web/product analytics, funnels, experiments, session replay and related diagnostics.
- License: repository states MIT expat except the `ee` directory, which has separate terms.
- Setup: hosted service is the lowest-friction route; self-hosting is advanced and requires Docker/server resources. Not an Android-local installation.
- Data/security: session replay and analytics may collect sensitive data if configured carelessly. Redact personal/medical data, define retention/access, and review consent requirements before use.
- Decision: useful only if website funnel analytics or experiments are a real current need.

## Visual generation

### ComfyUI
- Source: https://github.com/Comfy-Org/ComfyUI
- Use: node-based image/video generation workflows and API-backed pipelines.
- License: GPL-3.0 for the application repository; model weights and custom nodes may carry different terms.
- Setup: desktop/server with compatible dependencies and hardware. Not suitable for direct installation on the user's Android phone with under 5 GB free storage.
- Decision: retain in the future desktop/server list; do not install on the phone.

## Video automation

### MoneyPrinterTurbo
- Source: https://github.com/harry0703/MoneyPrinterTurbo
- Use: automated short video creation with scripts, voiceover, subtitles and B-roll.
- Evidence reviewed: official releases page showed v1.3.9 on 2026-10-21.
- License/security: confirm the current repository LICENSE, all provider/model terms, API costs, and dependency security before use; this review did not complete a full license or security audit.
- Setup: Python/WebUI and media dependencies; not an Android-local tool.
- Decision: watchlist only until full license and dependency checks are recorded.

## Trends and discovery sources
- GitHub marketing topic: https://github.com/topics/marketing
- Curated open-source marketing repository list: https://github.com/polnikale/awesome-marketing-repos-sequenzy
- Marketing skills repository: https://github.com/coreyhaines31/marketingskills

Use topic/star growth to discover candidates, then inspect actual repository files, releases, license, setup, data handling and policy fit. Do not copy third-party skills into this repository without verifying terms.

## Decisions on 2026-10-24
1. Adopt three locally written skills for Meta ad copy, Bangla/English content, and creative testing.
2. Link Marketingskills as an external reference, not claim it is installed in ChatGPT.
3. Keep Postiz, PostHog, ComfyUI and MoneyPrinterTurbo as staged evaluation candidates with the caveats above.
4. Do not install software on the user's phone; storage remains below 5 GB.
5. Do not create a separate GitHub repository in this run because the available GitHub connector actions do not expose a repository-creation operation. Changes are being organized in the existing repository.
