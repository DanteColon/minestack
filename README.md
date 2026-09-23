# Minestack

Windows desktop app for managing local Minecraft Java servers.

[Download the latest public release](https://github.com/DanteColon/minestack/releases/latest)

## Getting started

1. Download the Windows x64 installer from the release's **Assets** section. GitHub's source-code archives are not the desktop app.
2. Install Java for your Minecraft version. Minecraft 1.21.x requires Java 21; other versions may differ.
3. Install and open Minestack, then import an existing server folder or create one. Review and accept the Minecraft EULA before running server software.
4. Keep backups of your worlds. Stop the server before creating or restoring a backup.

Version 1.2.7 connects directly to official server providers and Modrinth; a localhost backend is not needed. New servers default to `%APPDATA%\Minestack\servers`. Older releases may behave differently; read the notes for your version.

## Releases and verification

This repository distributes installers and release notes. Website, backend and desktop source development are maintained separately. Candidates remain drafts until reviewed and tested.

Where provided, compare the installer SHA-256 hash with `SHA256SUMS.txt` from the same release:

```powershell
Get-FileHash -Algorithm SHA256 -LiteralPath .\Minestack-Setup-1.2.7.exe
```

Signing status is recorded in new release notes. An unsigned installer may display an unknown-publisher warning; do not assume every download is Authenticode signed.

## Reporting problems

[Open an issue](https://github.com/DanteColon/minestack/issues/new) with the Minestack, Windows, Java and Minecraft server versions, reproduction steps, and relevant logs. Remove IP addresses, authentication tokens and other private information before posting.

Minestack is independent and is not an official Minecraft product or affiliated with Mojang or Microsoft.
