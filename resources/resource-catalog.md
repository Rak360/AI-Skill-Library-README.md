# Resource Catalog

This is an index, not a statement that every project is installed, fully free, or approved for commercial use.

## Image and visual production
- ComfyUI — https://github.com/Comfy-Org/ComfyUI
- InvokeAI — https://github.com/invoke-ai/InvokeAI
- Hugging Face Diffusers — https://github.com/huggingface/diffusers
- rembg — https://github.com/danielgatis/rembg
- Real-ESRGAN — https://github.com/xinntao/Real-ESRGAN
- Upscayl — https://github.com/upscayl/upscayl
- Krita AI Diffusion — https://github.com/Acly/krita-ai-diffusion

## Social publishing and scheduling
- TryPost — https://github.com/trypostit/trypost (AGPL-3.0; MCP/REST; cloud and self-hosted options; evaluate account permissions and terms before use)
- Postiz — https://github.com/gitroomhq/postiz-app (AGPL-3.0; **security hold for new deployments** pending confirmation of the fix for critical CVE-2026-115931 / PSA-2026-JNXM56; see [security review](../docs/postiz-critical-security-advisory-2026-10-26.md))

## Video
- Kdenlive — https://github.com/KDE/kdenlive
- Shotcut — https://github.com/mltframework/shotcut
- Remotion — https://github.com/remotion-dev/remotion
- MoneyPrinterTurbo — https://github.com/harry0703/MoneyPrinterTurbo

## Audio transcription and subtitles
- faster-whisper — https://github.com/SYSTRAN/faster-whisper
- WhisperX — https://github.com/m-bain/whisperX
- Subtitle Edit — https://github.com/SubtitleEdit/subtitleedit

## Workflow automation and evaluation
- n8n — https://github.com/n8n-io/n8n
- Flowise — https://github.com/FlowiseAI/Flowise
- Langflow — https://github.com/langflow-ai/langflow
- Langfuse — https://github.com/langfuse/langfuse
- Ragas — https://github.com/vibrantlabsai/ragas

## Prompting and learning
- Prompts.chat — https://github.com/f/prompts.chat
- OpenAI Cookbook — https://github.com/openai/openai-cookbook
- Generative AI for Beginners — https://github.com/microsoft/generative-ai-for-beginners

## Review record
For each adopted resource, record date reviewed, version/commit, license, install method, API/model costs, hardware needs, security review, and commercial-use notes.

## Emerging resources reviewed — 2026-10-23

These are curated candidates based on a current popularity scan and direct repository checks. Popularity is only a discovery signal; it is not proof of quality, safety, or commercial suitability.

### Recommended to evaluate first
- [Marketing Skills](https://github.com/coreyhaines31/marketingskills) — MIT-licensed reusable marketing skills covering areas such as copywriting, SEO, CRO, email, ads, and launches. **Use case:** adapt relevant instructions into this library after reviewing each skill for platform and brand fit.
- [LazyEdit](https://github.com/lachlanchen/LazyEdit) — Apache-2.0 local-first video workflow for transcription, subtitles, captions, metadata, and publishing handoff. **Use case:** evaluate for a future desktop/server workflow, not as a simple one-click install. It has a substantial dependency stack and should be tested in an isolated environment with sample media first.

### Watchlist — verify before adoption
- [ArtCraft](https://github.com/storytold/artcraft) — a desktop creative environment for AI image/video workflows that appeared in a recent GitHub trend scan. A root license file was not found in the quick check; do not assume commercial-use permission. Review the current repository and all model/dependency licenses before use.
- [Anthropic Skills](https://github.com/anthropics/skills) — reusable skills and document-oriented workflows worth reviewing for inspiration. A root license file was not found in the quick check; verify current licensing and any skill-specific terms before copying or adapting files into a commercial workflow.
- [ComfyUI](https://github.com/Comfy-Org/ComfyUI) — remains a core candidate for configurable image/video generation workflows. Review the license of each model and custom node separately; model licenses can differ from the application license.

### Review method
- Review date: 2026-10-23.
- Evidence used: recent GitHub trend listings and direct repository metadata/file checks.
- Limitations: star counts and trend rankings change rapidly; no full security audit, local installation, or production benchmark was performed.
- Before adoption: inspect recent commits/releases, open issues, license, dependencies, model terms, hardware requirements, credential handling, and commercial-use rights.

## Marketing and social publishing reviewed — 2026-10-24

- [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) — MIT; reusable copywriting, social, paid ads, ad-creative, analytics and conversion-tracking skills. Compatible coding-agent installation is documented upstream; this does not install into the ChatGPT Android app.
- [gitroomhq/postiz-app](https://github.com/gitroomhq/postiz-app) — AGPL-3.0; social scheduling and analytics. Release v2.25.2 (2026-10-23) notes a security fix for PSA-2026-JNXM56; review the advisory and use a fixed current release before any deployment. Self-hosted stack is not suitable for direct Android install.
- [PostHog/posthog](https://github.com/PostHog/posthog) — MIT expat except the `ee` directory with separate terms; analytics, funnels and experiments. Self-hosting is advanced; review session replay, consent, data redaction and retention.
- [Comfy-Org/ComfyUI](https://github.com/Comfy-Org/ComfyUI) — GPL-3.0 application; model and custom-node licenses differ. Desktop/server candidate only, not Android local.
- [harry0703/MoneyPrinterTurbo](https://github.com/harry0703/MoneyPrinterTurbo) — release v1.3.9 observed 2026-10-21; short-video automation candidate. Full license, dependency, provider and model checks remain required before adoption.
- See [the dated review and caveats](marketing-creative-repository-review-2026-10-24.md).

## Social publishing candidate checked — 2026-10-24

- [trypostit/trypost](https://github.com/trypostit/trypost) — an AI-agent-oriented social scheduler with MCP and REST API options. Official repository metadata showed AGPL-3.0, 725 stars and 195 forks at review time, with a push on 2026-10-23; its latest GitHub release was v2.0.0 (published 2026-10-10).
- **Why it matters:** possible future bridge between content drafting, approval queues and multi-channel publishing.
- **Caveats:** AGPL-3.0 network-service obligations may matter for modified self-hosted deployments; review the current cloud terms, supported channels, API scopes, data retention and account permissions. No security audit or live-account test was performed.
- **Decision:** shortlist for a non-sensitive trial only. Do not connect production accounts or publish live content until permissions and approval controls are verified.


## Marketing skill and transcription update — 2026-10-25

- [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills) — official repository currently shows MIT licensing and active maintenance. Its `VERSIONS.md` records the 2.13.0 update dated 2026-10-19, including a dedicated `conversion-tracking` skill (1.0.0), while ads, analytics, copywriting, social and ad-creative skills have recent version entries. **Use:** compare upstream changes with this library and selectively adapt workflows; do not assume upstream skills are installed into ChatGPT. Keep the MIT notice if copying substantial portions, and review each update before use.
- [m-bain/WhisperX](https://github.com/m-bain/whisperX) — official repository shows BSD-2-Clause licensing, approximately 24.8k stars at review time, and current work on context-aware batching. **Use:** word-level timestamps and speaker labeling for subtitle workflows. **Constraint:** Python/PyTorch and model dependencies make it a desktop/server candidate, not a recommended Android installation on a low-storage device. Check the license/terms of any diarization or alignment models separately.
- Added [Medical-aesthetic Meta ads preflight checklist](../docs/medical-aesthetic-meta-ads-preflight.md) to operationalize policy, claims, age, consent, landing-page and tracking checks. It is a review aid, not a guarantee of ad approval; verify the live Meta policy before launch.

**Review limits:** This was a source/document review, not a security audit, benchmark, installation, or live-account test. No social accounts were connected and no ads or posts were changed.


## Security update — 2026-10-26

- **Postiz:** GitHub published critical CVE-2026-115931 (CVSS 9.9) on 2026-10-24. The v2.25.2 release published 2026-10-23 says it addresses PSA-2026-JNXM56, and the referenced commit restricts provider-function execution; however, the advisory's affected/patched version fields remain unknown. Do not deploy based on version number alone. Review the [full security note](../docs/postiz-critical-security-advisory-2026-10-26.md) and verify the exact patched commit before use.
- This is a source review, not a security audit. Postiz is not installed or connected in the user's ChatGPT or social accounts.
