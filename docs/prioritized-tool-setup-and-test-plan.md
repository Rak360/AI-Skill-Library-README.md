# Prioritized Tool Setup and Test Plan

**Last reviewed:** 2026-10-23  
**Purpose:** Increase output quality and speed for digital marketing work without installing too many tools, exposing customer data, or creating an unstable workflow.

This is a staged plan, not a claim that software has already been installed. Install tools on a supported computer/server, then mark each test as passed only after running it on that environment.

## Executive recommendation

Start with the lowest-friction tools that improve daily production. Do not begin with a complex local AI stack until the computer's operating system, RAM, GPU/VRAM, free disk space, and typical project volume are known.

| Priority | Tool / workflow | Why it comes here | Setup route | Minimum acceptance test |
|---|---|---|---|---|
| P0 | This prompt/skill library | Immediate reuse; no install required | Copy templates from `skills/` and `templates/` | Generate one brief, script, image prompt, and QC checklist; verify no invented facts |
| P1 | Kdenlive **or** Shotcut (choose one) | Immediate video editing/subtitles/export; avoid learning two editors at once | Official downloads: https://kdenlive.org/download/ or https://shotcut.org/download/ | Import a 20–30 sec sample, add Bangla/English text, export MP4, check audio sync, font rendering, and mobile readability |
| P1 | Subtitle Edit | Faster subtitle correction and export | Official project: https://github.com/SubtitleEdit/subtitleedit | Import a short transcript or media sample; correct Bangla/English spelling; export SRT; verify timestamps and UTF-8 text in a second player |
| P1 | Upscayl **or** rembg (only as needed) | Simple image quality or background-removal tasks | https://github.com/upscayl/upscayl or https://github.com/danielgatis/rembg | Test on 3 non-sensitive images; inspect edges, face details, artifacts, and output dimensions |
| P2 | faster-whisper | Batch transcription when repeated video work makes it worthwhile | https://github.com/SYSTRAN/faster-whisper | Transcribe a 1–2 minute sample with Bangla/English speech; measure time; manually check names, numbers, medical terms, and punctuation |
| P2 | ComfyUI **or** InvokeAI (choose one first) | Flexible image-generation workflows, but higher setup/model/hardware burden | https://github.com/Comfy-Org/ComfyUI or https://github.com/invoke-ai/InvokeAI | Generate 3 test images using properly licensed models; check repeatability, anatomy, image dimensions, speed, VRAM/RAM, and model terms |
| P3 | n8n | Automate repetitive brief intake, file naming, reminders, and reporting after the manual process is stable | https://github.com/n8n-io/n8n | Build a test workflow using dummy data; verify retries, failure alerts, credential storage, duplicate prevention, and logs. Check current license and deployment terms first |
| P3 | Langfuse | Observe/debug AI workflows only after API-based workflows exist | https://github.com/langfuse/langfuse | Log a test run with dummy content; ensure no secrets or patient data are captured; confirm access controls and retention |
| P4 | Diffusers / WhisperX / Remotion / Flowise / Langflow | Specialized or overlapping tools; adopt only when a clear gap exists | Links in `resources/resource-catalog.md` | Write a one-sentence use case and compare setup cost, performance, maintenance, and license against existing tools before adoption |

**License note:** n8n is source-available/fair-code rather than OSI-approved open source. Check the current license and intended use before deployment. Each model, custom node, extension, and dependency may have separate terms.

## Setup procedure for every tool

1. **Check fit:** identify the task this tool will improve and the current bottleneck.
2. **Check environment:** record OS/version, CPU, RAM, GPU/VRAM, disk space, and admin rights.
3. **Check source:** use only the official project site/repository and current installation instructions.
4. **Review trust:** inspect license, latest release/commit, dependencies, open issues, permissions, and known security concerns.
5. **Isolate:** prefer a dedicated virtual environment/container or a non-critical test machine for developer tools.
6. **Install deliberately:** follow the official instructions; pin versions where practical; do not run unreviewed scripts as administrator/root.
7. **Use sample data:** never start with patient records, personal data, ad account exports, access tokens, or confidential creative.
8. **Run the acceptance test:** record pass/fail, runtime, output quality, resource usage, and failure notes.
9. **Compare:** keep the tool only if it is measurably better than the existing workflow.
10. **Document:** record install date, version, license, machine, test result, owner, and rollback/uninstall method.

## Test scorecard

Score each dimension from 1 (poor) to 5 (excellent). Do not adopt a tool into production if security/license is unclear.

| Dimension | What to measure |
|---|---|
| Output quality | Visual fidelity, script usefulness, transcript accuracy, or export quality |
| Speed | Minutes saved per comparable task |
| Reliability | Repeatability, crash/error rate, and recovery |
| Resource use | RAM/VRAM, disk space, cloud/API spend |
| Ease of use | Steps required and learning burden |
| Security and rights | License clarity, data handling, dependencies, permissions |
| Business impact | Whether it improves turnaround time, cost, quality, or measurable campaign outcomes |

## Supreme Balora production safeguards

- Keep the premium, clean, medical, elegant, trustworthy, educational brand direction and approved burgundy/white palette.
- Use only approved service names, prices, devices, credentials, and treatment facts.
- A generated visual is not proof of a real clinical result. Before/after imagery must be authentic, consented, and presented honestly.
- Have qualified clinical review for medical claims before publication; avoid guaranteed, permanent, or unsupported duration claims.
- Never upload patient/customer data to external tools without authorization and suitable safeguards.
- Review current platform policies, consent/rights, subtitles, logos, flags, and on-image text before publishing.

## Current status

- [x] Prompt and workflow templates exist in this repository.
- [x] GitHub Actions file validation workflow added; a successful run must be confirmed separately.
- [ ] Record target computer's OS/RAM/GPU/VRAM before choosing local AI tools.
- [ ] Install and test one video editor.
- [ ] Test subtitle workflow on non-sensitive Bangla/English sample media.
- [ ] Evaluate image utility only if needed.
- [ ] Evaluate local image generation after hardware/model-license checks.
- [ ] Add automation only after a repetitive workflow has a stable manual version.

## Device information needed before hardware-heavy installs

Before choosing ComfyUI, InvokeAI, or local transcription models, record:
- Operating system and version
- RAM
- GPU model and VRAM (or confirm no dedicated GPU)
- Free disk space
- Whether the work must run on Android, Windows, macOS, or Linux
- Whether cloud/API use is acceptable and what monthly cost ceiling applies

Do not guess these values. If they are unavailable, stay with the low-risk P0/P1 tools and browser-based workflows.
