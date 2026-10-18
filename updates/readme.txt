LiteBrowser product updates

manifest.json is the public product-update manifest for LiteBrowser. It currently has no eligible product releases. Existing Chromium-version preview packages do not carry the independent product version/build contract and are intentionally excluded.

The browser checks this fixed HTTPS endpoint:
https://raw.githubusercontent.com/hikariCodeAi/litebrowser/main/updates/manifest.json

Product version, monotonically increasing build, channel, Chromium version, release notes and each platform's exact HTTPS Release asset URL, byte size, SHA-256, minimum OS and installation type are required. Upload and verify an audited full package before adding it to this manifest. stable clients do not consume preview releases. SHA-256 verifies package integrity; publisher trust currently comes from the fixed HTTPS GitHub repository, rather than a separately signed manifest.

Performance scope and limitations:
https://github.com/hikariCodeAi/litebrowser/blob/main/docs/performance-report.md
