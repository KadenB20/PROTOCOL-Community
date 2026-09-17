# PROTOCOL Community release notes

# PROTOCOL 0.12.0 — New onboarding and workspace customization

Start with a workspace that fits your routine, customize it at your own pace, and return to setup whenever you need. This release overhauls onboarding, settings discovery, saved views and Vault, with clearer wording throughout the app.

## What's new

- **A new setup flow.** Choose your basic preferences and one of five starting presets, or select your own areas with Custom Setup. Start using PROTOCOL immediately or continue through optional settings, views, tracking setup and a final review. Resume later from Settings → Workspace & Data → Resume Setup.
- **Presets you can change deliberately.** Preview the exact changes before applying another preset, with your own adjustments preserved by default. Existing workspaces keep their configuration after updating. Full Workspace includes PED Planner visibility; its separate first-use acknowledgement still applies.
- **Settings that are easier to find.** Search individual controls and saved configurations, see current values, jump to the right editor and save options for later. Browsing a disabled area does not enable it.
- **Reusable Daily and review views.** Save Daily field order, visibility and spacing. Create Training, Recovery and Phase review views with chosen sections and date ranges, then return to the original records to make changes.
- **Portable configuration profiles.** Save, review, export and import workspace configurations. These contain configuration rather than personal records; review included view names and card titles before sharing. Applying an imported profile remains a separate action.
- **Restore during first launch.** In the Windows app, choose a PROTOCOL backup, review its checked contents and restore into an empty workspace before creating a new one.
- **A refreshed Vault.** Browse files, favorites, links and archived items in the updated workspace. Open images in the shared photo viewer with zoom and navigation; open other files in their Windows default app while keeping the stored original unchanged. Details and version history remain separately accessible.

## Improvements and fixes

- Setup opens the same working editors used throughout PROTOCOL and records successfully saved items. Failed setup-reference saves can be retried without recreating the item.
- Clearer labels and descriptions across setup, settings, nutrition, Training, Rehab, Health, phases and startup screens.
- More reliable links back to setup and to individual settings, including cold launches and return navigation.
- Visible weekly Daily fields appear before the first entry. Optional fields remain optional, and missing values remain distinct from recorded zero.
- Corrected Training frequency counts, clearer custom Rehab rating validation, and more complete Vault entry selection with recovery when loading fails.

## Updating

Create and check a backup in Backup & Restore before updating, and keep a separate copy. Close PROTOCOL, download the Windows installer below and run it over your current installation. Your workspace and saved records are retained; existing users are not automatically enrolled in setup or switched to a preset.

This release updates the database format from 46 to 47. PROTOCOL creates a recovery backup before migration. After migration, older app versions cannot open that database; keep the pre-update backup.

## Notes

- The Windows installer remains unsigned. Follow the [download safety guidance](https://github.com/KadenB20/PROTOCOL-Community/blob/main/DOWNLOAD-SAFETY.md).
- Records, photos and backups remain local and are not encrypted by PROTOCOL. Product Notes report drafts use their separate local support store.
- First-run restore requires the installed Windows app. The browser preview does not restore desktop backups.
- PROTOCOL remains free, with no account, subscription or automatic software installation.

[Download v0.12.0](https://github.com/KadenB20/PROTOCOL-Community/releases/tag/v0.12.0)

---

# PROTOCOL 0.11.0 — Check-in Photos and faster daily logging

Organize and compare check-in photos in their own workspace, copy saved Daily Tracker values across a week with Undo, and enter grocery purchases with clearer quantities and previews.

## Check-in Photos

- Open Check-in Photos under Tools to import, organize and compare photos. Dates, poses, sets, collections and phase links are optional.
- Browse a photo library or calendar, filter your collection, mark favorites and save views. Archive photos and restore them later.
- Compare two or four photos with alignment controls, overlays and a reveal slider. Save comparisons, export images or download the originals.
- Choose a bodybuilding division for pose references and import defaults, or use your own poses. Imported photos appear immediately, including undated photos and imports made while filters are active.
- Photos stay on your device. Originals remain unchanged, and referenced originals are protected from deletion through Vault. Existing legacy photo records are copied into the new workspace while their original history is retained.

## Daily Tracker

- Drag a saved value's corner handle across visible days to copy it. Supported cells include numeric measurements, ratings, sleep, resting heart rate, blood pressure and saved meal-plan selections.
- Use the keyboard or tap the handle to choose a range or fill empty cells only. Undo restores the previous values and protects edits made since the fill.
- Values and weekly totals update promptly while saving. Missing values remain distinct from zero, future days are excluded, and unrelated sleep details or extra foods are preserved.

## Groceries

- Purchase entry starts with quantity and a compatible unit or package, with optional total paid.
- A preview shows the purchase amount, what it adds to Pantry and the remaining shopping need. Storage details and other outcomes are available when needed.
- Shopping grouping is easier to find, and purchase actions remain visible at the bottom of the dialog.

## Updating and your data

Close PROTOCOL and run the new installer over your existing installation. Your workspace and files stay in their current location.

This update adds storage for Check-in Photos. Before changing an existing database, PROTOCOL creates and validates a recovery backup; a failed backup stops the update to your data. Keep your pre-update backups. Older app versions cannot open the updated database.

Check-in Photos metadata and originals are included in ordinary workspace backups. Product report drafts and their screenshots continue to use their separate local support store.

JPEG, PNG, WebP, GIF, BMP and AVIF imports use the existing 10 MB per-file limit. Convert HEIC photos before importing. Downloaded originals retain their original metadata; generated comparison and contact-sheet images do not include original EXIF or GPS metadata.

The Windows installer remains unsigned. See the installation and download-safety guides if Windows displays a warning.

[Download v0.11.0](https://github.com/KadenB20/PROTOCOL-Community/releases/tag/v0.11.0)

---

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
