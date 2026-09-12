# Privacy

Your training, nutrition, health records, photos, and other PROTOCOL data are
stored on your own Windows device. There's no PROTOCOL account or online service
that receives these records. The app has no ads or usage tracking, and it doesn't
automatically send crash reports.

## Local records and backups

PROTOCOL doesn't encrypt records, Vault files, or backups. Someone with access to
those files may be able to read them. Protect your Windows account and keep
backups somewhere private. If you save files in a synced folder, such as a cloud
drive, that service's privacy terms apply to those copies.

The data folder is shown in Settings → Workspace & Data → Technical details.
Use Backup & Restore to make and check backups. Uninstalling PROTOCOL doesn't
delete the folder containing your records.

## When the app uses the internet

Update notices are off by default. If you turn them on, PROTOCOL checks GitHub
for a new version at most once a day while the app is open. You can also use
**Check for updates** yourself. These checks don't send your name, training
records, or health data. GitHub receives your IP address and the time of the
request, as it would when you visit a website. Turning notices off stops
automatic checks.

If you choose an online food or exercise lookup, that service receives the search
terms, barcode, or item identifier needed to return the result. Website links,
support pages, and downloads open in your browser; the site's own privacy terms
apply there.

## Support and sharing

Versions with GitHub handoff keep problem and suggestion drafts, selected
screenshots, and diagnostic snapshots locally. A small local operation log keeps
at most 200 events for seven days. Events contain technical operation categories,
timestamps and success/failure states, not entered values, record contents, file
paths, credentials, or raw error messages. The snapshot can include app, Windows,
WebView and database-schema versions, theme, viewport dimensions and display scale.
Saved report snapshots remain until you delete the draft, even after the rolling
operation log expires. Deleting a draft does not remove ZIPs you previously exported.

You can inspect these details and exclude them before sharing. Screenshot files
are re-encoded locally to remove metadata and original filenames, but information
visible in the image is not automatically hidden. Crop or redact private content
before adding an image.

Opening the GitHub form sends the reviewed prefilled text to GitHub and may put
it in your browser history. It does not submit the issue or upload local files.
GitHub uploads attachments as soon as you select them there, even before you
submit the issue. Exporting a report ZIP only writes a local file. Reports do not
require a PROTOCOL account; submitting on GitHub requires a GitHub account.

Support drafts are separate from ordinary workspace backups. You can export them
as report ZIPs and delete local drafts in Product Notes. Local deletion does not
delete a public GitHub issue or an uploaded attachment.

Nothing is uploaded automatically with a support request. GitHub reports and any
screenshots you attach are public. Don't post a backup, database, bloodwork
report, private photo, address, password, access token, or another person's information.
Crop screenshots to the problem and remove identifying details first.

You choose what to export and share. Check the files and who you're sending them
to before sharing.

## Questions

Ask general privacy questions in the
[Community issue tracker](https://github.com/KadenB20/PROTOCOL-Community/issues).
For a security vulnerability, use the private reporting route in [SECURITY.md](SECURITY.md).
