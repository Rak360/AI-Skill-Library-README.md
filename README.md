# AI Creative Skill Library

A practical, modular library for digital marketing and creative production: ad concepts, video scripts, image prompts, storyboards, editing workflows, subtitles, and safe marketing automation.

> This repository contains reusable prompt/workflow instructions and a resource catalog. It does not install software into ChatGPT or train an AI model.

## Included skills

- [Video Script Writer](skills/video-script-writer.md)
- [Creative Image Prompt Engineer](skills/creative-image-prompt-engineer.md)
- [Performance Ad Creative Strategist](skills/performance-ad-creative-strategist.md)
- [Medical Content Reviewer](skills/medical-content-reviewer.md)
- [Creative Production Workflow](skills/creative-production-workflow.md)
- [Open-source resource catalog](resources/resource-catalog.md)

## Setup guide

- [Setup, safe installation, and publication guide](docs/setup-guide.md)
- [Prioritized tool setup and test plan](docs/prioritized-tool-setup-and-test-plan.md)
- [Android-first digital marketing setup plan](docs/android-first-setup-plan.md)
- [Marketing image prompt templates](templates/image-prompt-templates.md)
- [Short-form video script template](templates/short-form-video-script-template.md)

## Recommended open-source resources

### Images and creative production
- [ComfyUI](https://github.com/Comfy-Org/ComfyUI) — node-based generative workflows
- [InvokeAI](https://github.com/invoke-ai/InvokeAI) — self-hosted image generation and editing
- [Hugging Face Diffusers](https://github.com/huggingface/diffusers) — diffusion model library
- [rembg](https://github.com/danielgatis/rembg) — background removal
- [Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN) — image restoration/upscaling
- [Krita AI Diffusion](https://github.com/Acly/krita-ai-diffusion) — AI-assisted Krita workflows

### Video and subtitles
- [Kdenlive](https://github.com/KDE/kdenlive) — open-source video editor
- [Shotcut](https://github.com/mltframework/shotcut) — cross-platform video editor
- [faster-whisper](https://github.com/SYSTRAN/faster-whisper) — speech-to-text
- [WhisperX](https://github.com/m-bain/whisperX) — transcription and word-level alignment
- [Subtitle Edit](https://github.com/SubtitleEdit/subtitleedit) — subtitle creation and synchronization

### Automation and evaluation
- [n8n](https://github.com/n8n-io/n8n) — workflow automation; source-available/fair-code, not OSI-approved open source
- [Flowise](https://github.com/FlowiseAI/Flowise) — visual LLM workflow builder
- [Langflow](https://github.com/langflow-ai/langflow) — visual AI workflow builder
- [Langfuse](https://github.com/langfuse/langfuse) — LLM observability
- [Ragas](https://github.com/vibrantlabsai/ragas) — LLM/RAG evaluation
- [Prompts.chat](https://github.com/f/prompts.chat) — reusable prompt examples
- [OpenAI Cookbook](https://github.com/openai/openai-cookbook) — API examples and guides

## Supreme Balora Hospital & Aesthetics Care creative guardrails

- Brand direction: premium, clean, medical, elegant, trustworthy, educational.
- Palette: burgundy `#7A1F2B`, white, light neutral backgrounds; Inter or Plus Jakarta Sans.
- Use realistic, modest, respectful people and clinically accurate devices/environments.
- Do not invent treatment specifications, devices, results, session counts, prices, or guarantees.
- Medical claims must receive qualified clinical review. Avoid guaranteed or permanent results claims.
- Before/after images must be authentic, consented, and presented honestly.
- Verify logos, flags, uniforms, device details, and on-image text manually.
- Protect patient/customer data. Never place confidential data into public tools without authorization and appropriate safeguards.

## Security and licensing

- Never commit API keys, passwords, tokens, patient data, or `.env` files.
- Use least-privilege permissions; avoid blanket admin access for tools.
- Review repository license, model license, dependencies, install scripts, and maintenance status separately.
- “Free,” “open source,” “free tier,” and “commercially usable” are not interchangeable.
- Human-review content before publication.

## Adoption order

1. Start with the prompt templates in this repository.
2. Use an existing editor such as Kdenlive or Shotcut.
3. Add transcription tools only if they solve a recurring bottleneck.
4. Test local image-generation tools only with suitable hardware.
5. Add automation for a specific, repeatable workflow.
6. Verify current license, setup, costs, and security before production use.

This catalog does not mean every project is installed or tested. ChatGPT integration requires compatible features and deliberate configuration.
