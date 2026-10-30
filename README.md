# ScholarBase Local

A desktop app for academics to keep their publication record in one place: import from ORCID, Google Scholar, Semantic Scholar and BibTeX, track citations, see your impact, and export polished publication lists and CVs. Everything stays on your computer.

**[Download the latest version →](https://github.com/shankardutt/scholarbase-releases/releases/latest)**

| Platform | File | Notes |
|----------|------|-------|
| Mac with Apple Silicon (M1 or later), macOS 12+ | `ScholarBase-Local-<version>-mac-apple-silicon.dmg` | Signed and notarized. Open the DMG and drag ScholarBase Local to Applications. |
| Mac with an Intel processor, macOS 11+ | `ScholarBase-Local-<version>-mac-intel.dmg` | Signed and notarized. |
| Windows 10/11 (64-bit) | `ScholarBase-Local-<version>-setup.exe` | Not code-signed yet: if "Windows protected your PC" appears, choose **More info → Run anyway**. |
| Linux (x86-64): Ubuntu 22.04+, Debian 12+, Fedora | `ScholarBase-Local-<version>-x86_64.AppImage` | `chmod +x` and run. It uses your system's WebKit: on Ubuntu/Debian `sudo apt install gir1.2-webkit2-4.1 libgirepository-1.0-1 libfuse2` (`libfuse2t64` on Ubuntu 24.04+); on Fedora `sudo dnf install webkit2gtk4.1 gobject-introspection fuse-libs`. |

Not sure which Mac you have? Apple menu → About This Mac: "Chip: Apple M…" is Apple Silicon, "Processor: … Intel" is Intel.

## What it does

- **Import** your publications from ORCID, Google Scholar, Semantic Scholar, a BibTeX file or a list of DOIs, with duplicate detection (including preprint and published versions of the same paper).
- **Citations per year and open access** for every paper with a DOI, from [OpenAlex](https://openalex.org), with "Save PDF to library" for free versions.
- **Metrics** — h-index, i10, citations in the last 5 years, h-index since any year, m-index — plus a "What changed" summary and a one-page **impact report** PDF.
- **Export** in APA, MLA, Chicago, Harvard, IEEE or Vancouver to Word, PDF, BibTeX, CSV, RIS (EndNote, Zotero, Mendeley), and Markdown or HTML for your website; generate a **CV**.
- **Daily refresh** of ORCID and OpenAlex data while the app is open, and a notice when a new version is out. Both can be turned off in Settings.

## Privacy

Your library is a SQLite database in your user data folder. The app talks to ORCID, OpenAlex, Semantic Scholar and CrossRef to fetch publication data, to Google Scholar only when you start a Google Scholar import, to an AI provider only if you add your own key, and to GitHub once a day to check for a new version (and to download it when you choose to install it). Nothing else is sent anywhere, apart from the details you enter when you register.

**Registering:** ScholarBase is free, but asks you to register the first time it opens. Your name, email, institution, role, country and the optional answers go to ScholarBase's developer, Shankar Dutt, who keeps them in a private Google Sheets spreadsheet to email your licence key and to learn who uses ScholarBase. They are never sold or shared. To have them removed, reply to the licence email. The key is checked on your computer; the app never contacts the registration service again.

## Updating

From 1.9.0 on, click the "Update available" pill in the app and choose **Install and restart**; the app verifies the download before installing it. Your data is kept. (From 1.7.0, download 1.9.0 once and install it over the old version.)

## Reporting a problem

[Open an issue](https://github.com/shankardutt/scholarbase-releases/issues/new/choose) with your version, computer and what happened. The app's log is in `~/Library/Application Support/ScholarBase-Local/logs` (macOS), `%APPDATA%\ScholarBase-Local\logs` (Windows) or `~/.local/share/ScholarBase-Local/logs` (Linux).
