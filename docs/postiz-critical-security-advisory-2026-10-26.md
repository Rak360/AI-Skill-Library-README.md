# Postiz Critical Security Advisory Review

**Reviewed:** 2026-10-26  
**Status:** Watchlist/security hold for any new deployment. This note is based on the upstream GitHub release and advisory pages; it is not a penetration test.

## What changed

On 2026-10-24, the GitHub Advisory Database published **CVE-2026-115931 / GHSA-h5r5-h782-vqvp**, rated Critical (CVSS 9.9), for Postiz. The report says an authenticated user could call unintended provider helper functions through the integrations endpoint. One helper could read files accessible to the server, potentially exposing environment secrets, session-signing material, database details, and connected-service credentials; another could stop the application. The advisory says affected and patched versions are currently **unknown**.

Sources:
- [GitHub Advisory Database: CVE-2026-115931](https://github.com/advisories/GHSA-h5r5-h782-vqvp)
- [Postiz upstream security policy](https://github.com/gitroomhq/postiz-app/security)
- [Postiz v2.25.2 release](https://github.com/gitroomhq/postiz-app/releases/tag/v2.25.2)
- [Upstream fix commit 9383f5b](https://github.com/gitroomhq/postiz-app/commit/9383f5be4d310c346e33a3748a9a7ded64c96fed)

## Release evidence and uncertainty

The official **v2.25.2** release was published on **2026-10-23** and its release notes explicitly say it addresses security vulnerability **PSA-2026-JNXM56**. The referenced upstream commit, dated 2026-10-23, restricts the integrations endpoint to approved provider methods. The GitHub advisory itself still reports affected/patched versions as unknown, so this review does **not** claim an independently verified safe version.

## Adoption decision

- Do not start a new production deployment until the maintainer's advisory and release fix are reconciled and the deployed build is confirmed to contain the fix.
- If operating a Postiz instance, compare the exact deployed commit with the upstream fix, upgrade to a confirmed patched release, restrict public registration and administrative access, and review server logs and integration activity.
- Because the reported impact can include secret exposure, if a potentially affected instance was publicly reachable, treat server environment secrets and connected-service credentials as potentially exposed: rotate relevant secrets/tokens after patching and investigate unexpected sessions, file access, and channel activity.
- Keep social-channel connections disconnected during testing. Use a non-sensitive test workspace and explicit human approval before any live publishing.
- Postiz uses the AGPL-3.0 license per its repository. Review current license obligations, hosted-service terms, channel permissions, and data retention separately; a license does not establish security or commercial suitability.

## Fit for this user

This is a server-oriented social publishing candidate, not an Android app to install locally. It remains on the evaluation/watchlist list only; no Postiz software was installed, no account was connected, and no live posts or ads were changed during this review.

**Next check:** Revisit the official advisory and release page before any future Postiz evaluation or deployment. Do not assume that a star count or a version label alone proves security.
