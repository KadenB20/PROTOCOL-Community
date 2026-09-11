# Windows warnings and download checks

PROTOCOL's Windows installer doesn't currently have a code-signing certificate.
Windows calls this an unsigned app and may warn or block it. The steps below
depend on which message you're seeing.

## Start with the official download

Download from [PROTOCOL Community Releases](https://github.com/KadenB20/PROTOCOL-Community/releases).
Check the owner and repository name: `KadenB20/PROTOCOL-Community`.
Don't download repackaged copies or installers sent by strangers. Only use the
official release page, and don't turn off security software to install the app.

Each release includes the installer, notes on what's changed, and `SHA256.txt`
for checking the download. I publish changes as new versions rather than replacing
an existing installer. [Release checks](RELEASE-CHECKS.md) lists antivirus results
and installation tests for each version.

The VirusTotal badge links to the scan report for the version shown beside it.
Results can change as antivirus tools update. A scan isn't a safety certificate;
check the report's SHA-256 against your download if you want to confirm it's the
same file.

## Which message are you seeing?

### Windows says the app is unrecognised

SmartScreen may show an unrecognised-app or unknown-publisher warning when it
doesn't have enough information to trust a download. That isn't the same as an
antivirus detecting malware. Check where the file came from, its name, and its
checksum before deciding whether you trust it. If you're unsure, leave it blocked
and ask for help.

New unsigned versions have to build their own reputation, so an update can trigger
a warning even if an earlier version didn't. There's no fixed number of downloads
or date when these warnings stop.
[Microsoft explains SmartScreen reputation](https://learn.microsoft.com/en-us/windows/apps/package-and-deploy/smartscreen-reputation).

### Antivirus names a threat or quarantines a file

Leave the file blocked. Do not restore it, add an exclusion or disable antivirus.
[Report the detection](https://github.com/KadenB20/PROTOCOL-Community/issues/new?template=installation_warning.yml)
with the antivirus name, exact threat name, PROTOCOL version and a cropped screenshot.
Do not assume a detection is a false positive just because the installer is unsigned.

The exact threat name helps me investigate the file and contact the antivirus
company if the detection is incorrect. A previous clean scan doesn't make a new
warning a false positive.

### Smart App Control or your organisation blocks the app

Smart App Control can block unsigned, unrecognised apps and doesn't offer an
exception for a single app. PROTOCOL may not run with those settings; don't turn
off that protection to install it. If this is a work or school computer, ask your
IT administrator about the block.
[Microsoft's Smart App Control FAQ](https://support.microsoft.com/en-us/windows/security/threat-malware-protection/smart-app-control-frequently-asked-questions).

## Compare the checksum

Download `SHA256.txt` from the same release. In PowerShell, run this from the folder
containing the installer, replacing `<version>` with its actual version:

```powershell
Get-FileHash .\PROTOCOL_<version>_x64-setup.exe -Algorithm SHA256
```

Compare every character with `SHA256.txt`; letter case does not matter. If they
differ, do not run that file. Download again from the official release or report
the mismatch.

A matching checksum means you have the same file as the published download. It
doesn't prove the program is harmless. Antivirus results apply to the file and
scan date shown, not every future version or every antivirus product.

## What installation does

PROTOCOL installs for your Windows user account. It needs Microsoft Edge WebView2
and may download it during setup if it's missing. Your records are stored
separately from the app. You choose when to download and install updates; PROTOCOL
won't do that in the background. See [installation and recovery](INSTALL.md) and
[privacy](PRIVACY.md).

Support reports are public. Do not attach a database, backup, bloodwork report,
private photo, password, or access token. A cropped screenshot of the warning is
enough to start.
