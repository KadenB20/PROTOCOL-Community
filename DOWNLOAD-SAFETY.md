# Windows warnings and download checks

PROTOCOL Community is unsigned. That means Windows cannot verify its publisher
through a trusted signing certificate. This page helps you identify a warning;
it does not ask you to ignore one.

## Start with the official download

Download from [PROTOCOL Community Releases](https://github.com/KadenB20/PROTOCOL-Community/releases).
Check the owner and repository name: `KadenB20/PROTOCOL-Community`.
Avoid repackaged copies, unsolicited attachments and instructions to turn off
security software. GitHub hosting is not a security endorsement.

Each release has a versioned installer, release notes and `SHA256.txt`. New builds
get new versions; the published installer is not silently replaced.
[Release checks](RELEASE-CHECKS.md) lists the evidence available for each version.

The README's VirusTotal badge opens the report for the version named beside it.
Check that the report's SHA-256 matches your download. Results can change as
security engines update; the badge is a report link, not an antivirus endorsement.

## Which message are you seeing?

### Windows says the app is unrecognised

SmartScreen can warn because a download has not established a reputation. That
message alone is not an antivirus finding, but it is not proof of safety either.
Confirm the official source, filename and checksum before deciding whether you
trust the download. If you are unsure, leave it blocked and ask for help.

Unsigned updates must build their own file reputation. There is no promised
number of downloads or date when warnings will stop.
[Microsoft explains SmartScreen reputation](https://learn.microsoft.com/en-us/windows/apps/package-and-deploy/smartscreen-reputation).

### Antivirus names a threat or quarantines a file

Leave the file blocked. Do not restore it, add an exclusion or disable antivirus.
[Report the detection](https://github.com/KadenB20/PROTOCOL-Community/issues/new?template=installation_warning.yml)
with the antivirus name, exact threat name, PROTOCOL version and a cropped screenshot.
Do not assume a detection is a false positive just because the installer is unsigned.

The maintainer can investigate the exact file and dispute an incorrect detection
with the vendor. Microsoft offers a developer submission process, not blanket
preapproval. [Microsoft's developer guidance](https://learn.microsoft.com/en-us/defender-xdr/developer-faq).

### Smart App Control or your organisation blocks the app

Some Windows settings do not permit an unsigned, unrecognised application.
Smart App Control currently has no exception for one individual app. This release
may not be usable on that device; do not weaken its protection to install it.
On a managed device, ask your IT administrator rather than changing policy.
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

A matching checksum shows that your file matches the published download. It does
not prove the program is harmless or replace publisher signing. A dated antivirus
scan has limits too: it describes that file and scan, not all future versions or
every security product.

## What installation does

PROTOCOL uses a per-user Windows installer. Microsoft Edge WebView2 is required;
the installer may download it if it is missing. Your records live separately from
the application. Updates are optional and user-installed, not silent background
replacements. See [installation and recovery](INSTALL.md) and [privacy](PRIVACY.md).

Support reports are public. Do not attach a database, backup, bloodwork report,
private photo or credentials. A cropped warning is enough to start.
