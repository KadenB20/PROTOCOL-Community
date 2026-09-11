# Install and update PROTOCOL

## First installation

1. Open [official releases](https://github.com/KadenB20/PROTOCOL-Community/releases).
2. Download the newest `PROTOCOL_<version>_x64-setup.exe`.
3. Run it and keep the default location unless you have a reason to change it.
4. Open PROTOCOL and create your workspace. Choose your units and time zone.
5. In Settings, hide sections you do not use. Start with your daily log or training.
6. Use Backup & Restore to create and check a backup.

Windows x64 and Microsoft Edge WebView2 are required. If WebView2 is missing, the
installer may download it. This is an installed application, not a portable app.

## Updating your existing installation

Create a backup, close PROTOCOL, and run the newer installer over your existing
installation. Do not uninstall first or change the installation location.
Your records are kept separately. Open Settings → Workspace & Data → About PROTOCOL
to confirm the new version.

Update checks are optional. They contact GitHub and do not upload your records.
Turning notices off does not affect manual checks or your ability to use the app.

## Windows warnings

These Community installers are unsigned. Windows may show an unknown
publisher, a warning, or a block depending on your device settings. Download only
from the official release page. Never disable Windows security to install the app.
If installation is blocked, leave it blocked and use the
[installation-warning report](https://github.com/KadenB20/PROTOCOL-Community/issues/new?template=installation_warning.yml).
The [warning guide](https://github.com/KadenB20/PROTOCOL-Community/blob/main/DOWNLOAD-SAFETY.md) distinguishes an unrecognised app from an
antivirus threat detection or a device-policy block. [Release checks](https://github.com/KadenB20/PROTOCOL-Community/blob/main/RELEASE-CHECKS.md)
record what was actually verified; they are not security certification.

For an optional integrity check, compare the installer with `SHA256.txt` from the
same release. PowerShell can show its checksum:

```powershell
Get-FileHash .\PROTOCOL_<version>_x64-setup.exe -Algorithm SHA256
```

Replace `<version>` with the version in the downloaded filename. A checksum detects
a changed or incomplete download; it does not replace publisher signing.

## Protect your progress

Use Backup & Restore regularly, especially before an update. Keep an additional
copy outside this PC. Backups include private records and are not encrypted.

Before upgrading the data format, PROTOCOL creates a recovery backup. If this
cannot be created and checked, the upgrade stops. A newer version may change the
data format: reinstalling an older version is not a supported way to undo that.
Keep the backup made before the update and report the problem.

Backup & Restore can validate a backup and test its contents in a separate folder.
That test does not replace your active records. Do not overwrite the active data
folder or delete database files to fix an update problem.

## Where your records live

Settings → Workspace & Data → Technical details shows the data folder for your
installation. The standard Windows folder is `%APPDATA%\ca.protocol.app`.
Uninstalling the app and deleting your records are separate actions. Do not remove
the data folder unless you intend to erase your records and have checked your backup.
