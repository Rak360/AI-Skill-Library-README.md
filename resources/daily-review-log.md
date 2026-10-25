# Resource Review Log

## 2026-10-23 — Initial scheduled-curation setup

### Changes published
- Added GitHub Actions validation workflow for required library files and non-empty Markdown files.
- Added a safe setup and adoption guide.
- Added reusable image prompt and short-form video script templates.
- Added a dated emerging-resource review to the resource catalog.

### Resources evaluated
- Marketing Skills — MIT license checked; promising for adapting marketing workflow instructions.
- LazyEdit — Apache-2.0 license checked; potentially useful but operationally complex and not installed or tested.
- ArtCraft — surfaced in a recent trend scan; root license not found during quick check, so watchlist only.
- Anthropic Skills — surfaced in a recent trend scan; root license not found during quick check, so watchlist only.
- ComfyUI — retained as a key visual-generation candidate; model and custom-node licenses must be checked separately.

### Validation and limitations
- New and updated files were fetched from GitHub after commit to verify they exist.
- GitHub Actions workflow file was verified in the repository, but a successful workflow run has not yet been confirmed.
- No third-party software was installed on the user's device, and no external social/ad account was connected.
- Future reviews should make a commit only when there is a meaningful, verified improvement; do not create cosmetic daily commits.


## 2026-10-23 — Prioritized setup and test plan

### Changes published
- Added `docs/prioritized-tool-setup-and-test-plan.md` with P0–P4 priorities, official setup routes, acceptance tests, safety/licensing checks, a scorecard, and staged adoption status.
- Linked the plan from the repository README.

### Validation and limitations
- The roadmap was fetched from GitHub after commit to verify publication.
- It does not assert that any desktop software has been installed.
- Hardware-heavy local AI tools remain pending until the target device's OS, RAM, GPU/VRAM, and disk capacity are known.


## 2026-10-23 — Android-first setup plan

### Changes published
- Added `docs/android-first-setup-plan.md` for the user's Android device profile (8 GB RAM or less, integrated graphics).
- Prioritized low-friction mobile workflows, included setup sources and acceptance tests, and marked beta open-source editors as optional trials.
- Added explicit privacy, permissions, medical-claim review, and non-sensitive test-data safeguards.
- Linked the Android-first plan from the README.

### Validation and limitations
- The new guide, README, and log were fetched from GitHub after commit.
- No app was installed on the user's phone; device version, storage, and installed apps remain unknown.


## 2026-10-23 — Low-storage mobile workflow

### Changes published
- Added `docs/android-first-weekly-workflow.md` with a lightweight daily and weekly routine designed for a low-storage Android device.
- Added `templates/content-tracker-template.csv` with non-sensitive production tracking columns.
- Linked both from the README.

### Safety notes
- The tracker is a template only; do not put patient details, lead personal data, or confidential information into this public repository.
- No new app was installed. The workflow prioritizes browser tools and existing apps until storage is freed.


## 2026-10-24 — Marketing creative development skills and repository review

### Changes published
- Added a Meta/Facebook ad copywriting skill.
- Added a Bangla/English marketing content-writing skill.
- Added a creative testing planner for paid-social campaigns.
- Added a dated repository review covering marketing skills, social scheduling, analytics, visual generation and video automation.
- Linked the new skills and review from README and resource catalog.

### Evidence and limitations
- Current repository pages, READMEs, release notes and license statements were reviewed for the listed candidates.
- Postiz v2.25.2 release notes mention a security fix; check the upstream advisory before deployment.
- No third-party tool was installed and no social/ad account was connected.
- A separate GitHub repository was not created because the available connector actions do not expose repository creation; changes are in this existing repository.


## 2026-10-24 — ChatGPT marketing app and connector setup guide

### Changes published
- Added `docs/chatgpt-marketing-apps-setup.md` covering Canva, ChatGPT Ads Manager, Metricool, Runway, and Windsor.ai.
- Included current app-catalog status, intended use, first acceptance tests, account permission review, privacy, and live-action approval safeguards.
- Linked the guide from README.
- Updated the daily review automation prompt to include ChatGPT apps/connectors and to distinguish available, installed, and connected states.

### Validation and limitations
- Guide and README were fetched from GitHub after publication.
- Canva appeared installed in the app catalog. Ads Manager, Metricool, Runway, and Windsor.ai were offered as connection candidates; their accounts are not confirmed connected.
- No third-party account was connected and no live ad/post was changed or published in this step.


## 2026-10-24 — Social-publishing candidate and CI coverage improvement

### Research
- Checked the official TryPost repository metadata and release page. It showed AGPL-3.0, 725 stars and 195 forks at review time, a push on 2026-10-23, and latest release v2.0.0 published 2026-10-10.
- Evaluated its MCP/REST publishing approach as a potential future workflow bridge; no account or production deployment was tested.
- Confirmed the latest previously recorded GitHub Actions run completed successfully before this change.

### Changes published
- Added TryPost to the resource catalog and dated repository review with its license, activity, setup and approval-gate caveats.
- Added a social-publishing section to the README.
- Expanded CI required-file checks to include the Meta ad copywriter, Bangla/English writer, creative testing planner, ChatGPT connector guide, and dated review.

### Safety and limitations
- TryPost remains an evaluation candidate, not installed or connected.
- AGPL-3.0 network-service obligations and hosted terms need review before deployment.
- No production social/ad account was connected, no live content was published, and no patient or customer data was added.
- The new workflow run must be checked after the commit; its success is not assumed.


## 2026-10-25 — Marketing skills and medical-aesthetic ad safety

### Research
- Rechecked the official `coreyhaines31/marketingskills` repository, MIT license, and `VERSIONS.md`; the latest listed release line is 2.13.0 (2026-10-19), including a dedicated conversion-tracking skill.
- Rechecked the official `m-bain/whisperX` repository and BSD-2-Clause license. It remains useful for word-level subtitle timing and speaker labels, but its Python/PyTorch/model stack is not suitable for direct installation on the user's low-storage Android device.
- Reviewed Meta's official Advertising Standards hub as the policy starting point. Because live policy pages may change and were not fully retrievable in this run, the checklist explicitly requires checking current policy wording before launch.

### Changes published
- Added `docs/medical-aesthetic-meta-ads-preflight.md` covering neutral claims, adult targeting where required, patient consent, authentic before/after media, landing-page consistency, privacy, tracking, and clinical/policy sign-off.
- Linked the checklist from README and added dated source notes to the resource catalog.
- Added the checklist to the CI required-file check.

### Validation and limitations
- The repository is public and the connected GitHub integration has push permission.
- After this commit, check the GitHub Actions result; do not assume CI passes until the run is completed.
- No third-party software was installed; no ChatGPT app was newly connected; no Facebook/Instagram account, live campaign, or post was modified.
- The scheduled run's push/email notifications are currently unavailable in this run context; the report is delivered here.
