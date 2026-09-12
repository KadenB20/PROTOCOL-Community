# PROTOCOL Community release notes

# PROTOCOL 0.10.1 Community

This patch adds a way to prepare problem reports and suggestions inside PROTOCOL,
then share them through the public Community issue tracker.

## What changed

- Choose a problem report or suggestion when writing a product note, or start one
  from Product Notes. Existing personal notes can become report drafts.
- Save and reopen reports locally, including up to three screenshots added by
  choosing files, pasting, or dropping them.
- Inspect optional technical details and a short operation log. These contain
  version information and operation outcomes, without record contents, personal
  file paths, or raw exception messages.
- Review what you will share, export a report ZIP, and open a prefilled GitHub
  form. Long reports have a complete-copy fallback.
- Keep the resulting GitHub issue link with your local report. Opening GitHub
  does not claim that a report has been submitted or fixed.
- Prepare reports from error screens, including startup failures.

## Sharing a report

GitHub reports and uploaded files are public. Review the text and screenshots,
extract the exported ZIP, then attach the selected files and submit in your
browser. A GitHub account is required. PROTOCOL does not upload attachments or
submit reports automatically.

Reports and screenshots are separate from ordinary workspace backups. Export a
report ZIP to keep a portable copy. Deleting a local draft does not delete a
public issue or an attachment already uploaded to GitHub.

## Updating from 0.10.0

Create a backup, close PROTOCOL, and run the 0.10.1 installer over your existing
installation. Keep the same location; do not uninstall first. Check the version
in Settings → Workspace & Data → About PROTOCOL after opening it.

This patch does not change the workspace data format. Personal notes and existing
training, nutrition, health, and recovery records remain in their current store.

The Windows x64 installer is unsigned. Use the official Community download and
read the linked Windows warning guidance if your device displays a warning.

[Download v0.10.1](https://github.com/KadenB20/PROTOCOL-Community/releases/tag/v0.10.1)

---

# PROTOCOL 0.10.0 Community

The first public Community release brings your training, nutrition, recovery, and
progress together in a free Windows app. Your records stay on your PC, with no
account or subscription needed.

## What is new

- A wider desktop workspace for planning your weeks and reviewing each phase.
- Expanded bodybuilding foods and simpler meal, grocery, and pantry workflows.
- Updated training, health, recovery, and PED record screens.
- Fill plans across selected days or weeks and review the changes in your Timeline.
- Choose measurement display units while keeping the original recorded values.
- Public downloads and release notes in PROTOCOL Community.
- Optional update notices and a Check for updates button in About PROTOCOL.
- A checked recovery backup before the app updates your data format.

## Installing this version

Create a backup, close PROTOCOL, and run the new installer over your existing
installation. Keep the same location and do not uninstall first. Check the version
in Settings → Workspace & Data → About PROTOCOL after opening it.

Existing 0.9.1 users need to install this version manually. You can then turn on
update notices. PROTOCOL will never install an update or restart in the background.

## Before you update

This version updates the data format. Keep your pre-update backup. Reinstalling an
older version will not undo that change.

This is the first Community release for Windows x64. The installer is unsigned, so Windows
may show an unknown publisher or security warning. Use only the official download.
Records and backups are not encrypted. Health and PED features are for recording
your own information and plans, not treatment or dosing advice.

If something gets in the way of your training log or planning, report it in the
Community issue tracker. Include your version and steps to repeat the problem,
without attaching private records.

[Download v0.10.0](https://github.com/KadenB20/PROTOCOL-Community/releases/tag/v0.10.0)
