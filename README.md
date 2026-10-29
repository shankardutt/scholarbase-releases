# ScholarBase Local

A desktop app for academics to keep their publication record in one place: import from ORCID, Google Scholar, Semantic Scholar and BibTeX, track citations, see your impact, and export polished publication lists and CVs. Everything stays on your computer.

**[Download the latest version →](https://github.com/shankardutt/scholarbase-releases/releases/latest)**

| Platform | File | Notes |
|----------|------|-------|
| macOS 12 or later, Apple Silicon (M1 or later) | `ScholarBase-Local-<version>.dmg` | Signed and notarized. Open the DMG and drag ScholarBase Local to Applications. |
| Windows 10/11 (64-bit) | `ScholarBase-Local-<version>-setup.exe` | Not code-signed yet: if "Windows protected your PC" appears, choose **More info → Run anyway**. |
| Linux (x86-64) | `ScholarBase-Local-<version>-x86_64.AppImage` | `chmod +x` and run. Needs GTK 3, WebKit2GTK 4.1, FUSE 2 (`libfuse2t64` on Ubuntu 24.04) and glibc 2.39+ (Ubuntu 24.04, Fedora 40 or newer). |

## What it does

- **Import** your publications from ORCID, Google Scholar, Semantic Scholar, a BibTeX file or a list of DOIs, with duplicate detection (including preprint and published versions of the same paper).
- **Citations per year and open access** for every paper with a DOI, from [OpenAlex](https://openalex.org), with "Save PDF to library" for free versions.
- **Metrics** — h-index, i10, citations in the last 5 years, h-index since any year, m-index — plus a "What changed" summary and a one-page **impact report** PDF.
- **Export** in APA, MLA, Chicago, Harvard, IEEE or Vancouver to Word, PDF, BibTeX, CSV, RIS (EndNote, Zotero, Mendeley), and Markdown or HTML for your website; generate a **CV**.
- **Daily refresh** of ORCID and OpenAlex data while the app is open, and a notice when a new version is out. Both can be turned off in Settings.

## Privacy

Your library is a SQLite database in your user data folder. The app talks to ORCID, OpenAlex, Semantic Scholar and CrossRef to fetch publication data, to Google Scholar only when you start a Google Scholar import, to an AI provider only if you add your own key, and to GitHub once a day to check for a new version. Nothing is sent anywhere else.

## Updating

Download the new version and install it over the old one; your data is kept. Settings → Data management → Download backup makes a copy first if you want one.
