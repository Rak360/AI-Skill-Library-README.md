# Setup and Usage Guide

This repository is a prompt-and-workflow library. It does not install third-party tools into ChatGPT or onto your device by itself.

## 1. Start immediately: use the prompt skills
1. Open a skill in the `skills/` directory.
2. Copy its instructions into your preferred AI assistant or adapt them to your workflow.
3. Supply the campaign brief, verified facts, platform, format, language, audience, and CTA.
4. Review generated copy and assets before publishing.

For Supreme Balora Hospital & Aesthetics Care, follow the guardrails in `README.md`; treatment information, prices, devices, claims, and outcomes must be verified before publication.

## 2. Suggested tool adoption order

| Need | Suggested project | Notes |
|---|---|---|
| Video editing | Kdenlive or Shotcut | Desktop editor; install on your computer from official project instructions |
| Speech transcription | faster-whisper or WhisperX | Python setup and compatible hardware/dependencies may be needed |
| Image workflow | ComfyUI or InvokeAI | Requires compatible hardware/models; check model licenses and VRAM needs |
| Background removal | rembg | Python project; test output quality on your own images |
| Upscaling | Upscayl or Real-ESRGAN | Results vary by image; inspect for artifacts |
| Automated workflows | n8n, Flowise, or Langflow | Review hosting, license, credentials, and access controls before connecting accounts |

This list is a starting point, not a claim that tools are installed, tested on your device, or suitable for every workload.

## 3. Safe installation procedure
Before installing a project:
- Open the project's official repository and latest installation documentation.
- Check its license, latest release, known issues, dependencies, and system requirements.
- Prefer official releases and pinned versions; do not run copied shell commands blindly.
- Never paste API keys into public files or prompts; use environment variables or a secrets manager.
- Do not upload patient/customer records or sensitive business information to tools without authorization and suitable safeguards.
- Test using non-sensitive sample data first.
- Record version, install date, machine, license, and known limitations.

## 4. Publishing a finished creative
Use the workflow in `skills/creative-production-workflow.md`. Check the final copy, rights/consent, medical or legal approvals, platform policy, tracking links, crop, subtitles, and CTA. Publication to external ad/social accounts requires those accounts and suitable authorized access; a GitHub commit alone does not publish an ad or social post.

## 5. Local installation still requires a target environment
GitHub can store code and documentation. Actual installation requires a computer/server or an explicitly connected execution environment. This guide does not run third-party installers on your phone or computer.
