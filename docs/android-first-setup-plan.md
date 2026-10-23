# Android-First Digital Marketing Setup Plan

**Reviewed:** 2026-10-23  
**Device profile supplied by user:** Android phone, 8 GB RAM or less, integrated graphics. Exact Android version and free storage are not yet known.

## Recommendation

Use cloud/browser AI for heavy generation, and keep editing projects modest on-device. Do not try to install desktop tools such as Kdenlive, Shotcut, ComfyUI, InvokeAI, or Python transcription stacks directly onto this phone. These are not normal Android app installs and may be too resource-intensive or require a separate computer/server.

## Priority stack

| Priority | Tool | Purpose | Setup route | Acceptance test |
|---|---|---|---|---|
| P0 | ChatGPT + this repository's skills | Scripts, ad copy, campaign ideas, image prompts, QA checklists | Open `skills/` and `templates/` files in GitHub; copy the relevant template into ChatGPT | Produce one 30-second script and one image prompt; check spelling, approved facts, CTA, and medical-claim safety |
| P1 | Canva | Static ads, social posts, covers, simple video and presentations | Install/update only through Google Play's official Canva listing or use canva.com in browser | Create one 1080x1350 post and one 1080x1920 story using approved brand assets; export and inspect text/crop |
| P1 | VN **or** CapCut | Short-form video editing; choose one to start | Use the official Google Play listing or official publisher site; availability/features can vary by region | Edit a 20–30 second sample, add captions and brand text, export 1080p MP4, inspect audio sync and watermark |
| P1 | Google Drive + Sheets | Asset storage, content calendar, lead/reporting work | Use official Google Play apps and sign into the approved work account | Upload a non-sensitive sample, open it on another device/browser, and verify folder permissions and a simple tracking sheet |
| P1 | Meta Business Suite | Manage Facebook/Instagram pages, inbox and scheduled content where supported | Install from Google Play; connect only the authorized business portfolio and grant minimum necessary access | Draft a test post or use a non-public draft; verify correct page/account, CTA, image crop, and scheduling timezone before publishing |
| P1 | YouTube Studio (if used) | Manage channel content, comments and analytics | Install from Google Play using the official publisher | Open analytics and verify the correct channel; do not share login credentials |
| P2 | LibreCuts (open-source, beta) | Local trimming, joining, overlays and SRT subtitle placement | Review official project and F-Droid listing before optional installation | On a copy of a non-sensitive clip, trim, add text/SRT, export, then inspect output; beta may contain bugs |
| P2 | Open Video Editor (open-source) | Basic local trim, scale, rotate, filters, and conversion | Prefer F-Droid's verified build over random APK download; inspect current release before use | Convert a short sample, confirm orientation, audio, resolution, and playback in a second app |
| P3 | Cloud AI image/video tools | Heavy image generation or advanced AI processing | Use browser/app only after reviewing current service privacy, costs, and commercial terms | Generate one non-sensitive test asset; check quality, cost, export limits, and usage rights |

## Important project links

- Canva video editor and export guidance: https://www.canva.com/video-editor/
- LibreCuts source (MIT; beta): https://github.com/tharunbirla/LibreCuts
- LibreCuts F-Droid listing: https://f-droid.org/en/packages/com.tharunbirla.librecuts/
- Open Video Editor F-Droid listing: https://f-droid.org/en/packages/io.github.devhyper.openvideoeditor/
- Main skill library: https://github.com/Rak360/AI-Skill-Library-README.md

LibreCuts is currently beta; treat it as an optional trial, not the only production editor. For open-source Android apps, prefer the official F-Droid listing/source and check permissions, latest version, release notes, and license. Avoid downloading APKs from unknown mirror sites.

## First 45-minute setup session

1. **5 minutes — check device:** Android version, free storage, and which apps are already installed. Keep at least several GB free for video projects when possible.
2. **10 minutes — organize storage:** create folders `Marketing/00_Briefs`, `01_Scripts`, `02_Source`, `03_Exports`, `04_Approved`, and `05_Reports` in the approved Drive account.
3. **10 minutes — make a content tracker:** columns: date, brand, campaign, platform, format, status, owner, approved facts/source, CTA/link, reviewer, publish date, results.
4. **10 minutes — test a static creative:** use a non-sensitive brief and official logo; export one post and inspect text readability at phone size.
5. **10 minutes — test a short video:** edit a 20–30 second non-sensitive sample; export 1080p, check audio sync, spelling, safe margins, and file size.

## 1080p video export checklist

- Use 9:16 for Reels/Shorts and 4:5 or 1:1 for feed creatives when appropriate.
- Start with 1080p and 30 fps unless the source or platform need something else.
- Close background apps before export and avoid editing long 4K projects on a low-memory device.
- Keep original source media until the export has been checked.
- Play the exported file from beginning to end, check subtitles, audio, logos, spelling, and mobile-safe margins.
- Use non-sensitive sample media for initial testing.

## Security and brand safety

- Do not share passwords, one-time codes, recovery codes, or API keys in chat or in GitHub.
- Give social apps access only to the correct business assets and only the permissions needed.
- Never upload patient records, identifiable clinical images, private lead sheets, or confidential customer information to an AI service without authorization and appropriate safeguards.
- For Supreme Balora Hospital & Aesthetics Care, use approved brand assets and verified treatment facts. Medical claims require qualified clinical review; do not invent results, session counts, device specs, or guarantees.
- Do not auto-publish a medical ad just because an AI workflow generated it. Keep a human approval step.

## Status

- [x] Android-first plan documented in GitHub.
- [ ] Check Android version and available storage.
- [ ] Confirm which editing/design apps are already installed.
- [ ] Complete the static creative acceptance test.
- [ ] Complete the 20–30 second video export test.
- [ ] Trial an open-source editor only if the main editor is insufficient.
- [ ] Consider automation only after the manual workflow is stable.

This document is a setup plan; it does not claim that any app has been installed on the user's device.


## Low-storage mode: under 5 GB free

**Current device profile:** Android 13 or newer; less than 5 GB free storage; integrated graphics.

### Before installing anything
1. Do not install a video editor, subtitle tool, or open-source APK until you have checked free space again.
2. Open **Settings → Storage** and identify the largest categories. Labels vary by Android manufacturer.
3. In **Files by Google**, review the cleanup suggestions. Delete only items you recognize and no longer need; verify backups before deleting photos/videos.
4. In **Settings → Apps → [app] → Storage & cache → Clear cache**, clear cache for apps with unusually large temporary data. Do **not** tap Clear storage/data unless you understand that it can remove local app data and sign-in state.
5. Remove old exported videos, duplicate downloads, offline media, and unused apps only after reviewing them. Do not delete unknown folders or app/system files.
6. If possible, move original media to an approved cloud account or computer and verify the copies open before removing local copies.
7. Restart the phone and re-check free space.

Google's official guidance: https://support.google.com/android/answer/7431795 and Files by Google: https://support.google.com/files/answer/9848742.

### Installation gate
- **Below 2 GB free:** do not install a new creative app. Use the browser for lightweight tasks and free space first.
- **2–5 GB free:** keep installed apps to a minimum. Use browser-based design and AI, edit only short 720p/1080p clips, and keep offline downloads limited.
- **After reaching at least 5–8 GB free:** consider one app at a time; this is a practical buffer recommendation, not an Android requirement. Re-check the actual Play Store download size and extra working space first.

### Low-storage test sequence
1. Use ChatGPT and the existing GitHub templates in the browser; confirm a prompt/script can be copied and used without downloading large files.
2. Open Canva in browser or its already-installed app; create one small non-sensitive draft. Do not install the app solely for this test while storage is constrained.
3. Export one short test image only if there is enough free space; verify it appears in the intended folder.
4. Test video editing only after confirming enough free space for both source footage and the export. Start with a 10–20 second 720p sample; move to 1080p only if the phone remains stable.
5. Record app name, available space before/after, export time, crashes/heat, and result quality.
6. If the phone heats up, crashes, or reports insufficient space, stop the test; do not repeatedly retry large exports.

### Do not do these
- Do not download APKs from random sites or install several editors at once.
- Do not delete backed-up-looking files until you verify the backup and can open it.
- Do not clear app storage/data for WhatsApp, Drive, Canva, or other work apps as a first troubleshooting step.
- Do not attempt to run ComfyUI, InvokeAI, Kdenlive, Shotcut, or local Python AI models directly on this phone as if they were normal Android apps.
- Do not upload patient records, identifiable clinical photos, lead lists, passwords, or tokens to public AI tools.

### Current next action
Free and verify storage first. Then test the existing browser workflow; install no new app until the device has adequate free space and a clear need for that app.
