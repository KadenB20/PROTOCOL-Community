# Install and update PROTOCOL

## Requirements

PROTOCOL is a Windows desktop app and needs 64-bit Windows (x64) and Microsoft
Edge WebView2. If WebView2 isn't installed, the installer may download it for you,
so keep an internet connection available during setup.

Install PROTOCOL before using it; it isn't a portable app that runs from a USB drive.

## First installation

1. Open [official releases](https://github.com/KadenB20/PROTOCOL-Community/releases).
2. Download the newest `PROTOCOL_<version>_x64-setup.exe`.
3. Open the installer and follow the setup steps. The default location is fine.
4. Open PROTOCOL and create your workspace. Choose your units and time zone.
5. In Settings, hide sections you do not use. Start with your daily log or training.
6. Use Backup & Restore to create and check a backup.

## Updating your existing installation

1. Back up your records, then close PROTOCOL.
2. Run the newer installer and keep the same installation location. **Don't uninstall first.**
3. Open **Settings → Workspace & Data → About PROTOCOL** to check the new version.

Your records are stored separately from the app and are kept when you update.

You can check for updates in About PROTOCOL or turn on update notices. These
checks contact GitHub but don't upload your records. With notices off, you can
still check for updates yourself and keep using the app normally.

## Windows warnings

The installer doesn't have a code-signing certificate, so Windows may show an
unknown-publisher warning or block it. Download only from the official release
page, and don't disable Windows security to install it.

See [Windows warnings](https://github.com/KadenB20/PROTOCOL-Community/blob/main/DOWNLOAD-SAFETY.md)
for help with the message you're seeing. If your antivirus detects a threat,
leave the file blocked and
[report the warning](https://github.com/KadenB20/PROTOCOL-Community/issues/new?template=installation_warning.yml).

To check whether your download matches the original file, compare its checksum
with `SHA256.txt` from the same release. Run this in PowerShell from the folder
containing the installer:

```powershell
Get-FileHash .\PROTOCOL_<version>_x64-setup.exe -Algorithm SHA256
```

Replace `<version>` with the version in the downloaded filename. Compare the full
result with `SHA256.txt`. If they differ, don't run the file. A matching checksum
confirms you have the same file, not that the software is safe.

Antivirus results and installation test details are listed under
[release checks](https://github.com/KadenB20/PROTOCOL-Community/blob/main/RELEASE-CHECKS.md).

## Protect your progress

Use **Backup & Restore** regularly, especially before an update. Keep another copy
somewhere private outside this PC. Backups contain your personal records and aren't
encrypted, so anyone with access to the files may be able to read them.

Some updates change how records are stored. Before making that change, PROTOCOL
creates and checks a recovery backup. If that fails, the change won't go ahead.
Reinstalling an older app version won't undo a change to your records. If an
update fails, keep your backup and report the problem instead.

**Backup & Restore** can also test a backup in a separate folder without replacing
your current records. Don't overwrite your data folder or delete database files
to try to fix an update problem.

## Where your records live

Settings → Workspace & Data → Technical details shows the data folder for your
installation. The standard Windows folder is `%APPDATA%\ca.protocol.app`.
Uninstalling PROTOCOL doesn't delete this folder. Only remove it if you intend to
erase your records and have checked that your backup works.
