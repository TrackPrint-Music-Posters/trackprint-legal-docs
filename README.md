# TrackPrint legal documents

The Impressum (legal notice, DDG), Datenschutzerklärung (privacy policy,
DSGVO/GDPR) and Nutzungsbedingungen (terms of use) for TrackPrint, the album
poster app for iPhone, iPad and Mac, in German and English. The German terms
of use are the binding version. This repo is the only copy: the app links
here from Settings ▸ About, the website's footer links here, and the privacy
policy URL in App Store Connect points here too.

## Published at

GitHub Pages serves `main` from the repo root:

| Document | German | English |
|---|---|---|
| Impressum | [impressum.de.html](https://trackprint-music-posters.github.io/trackprint-legal-docs/impressum.de.html) | [impressum.en.html](https://trackprint-music-posters.github.io/trackprint-legal-docs/impressum.en.html) |
| Datenschutzerklärung | [datenschutzerklaerung.de.html](https://trackprint-music-posters.github.io/trackprint-legal-docs/datenschutzerklaerung.de.html) | [datenschutzerklaerung.en.html](https://trackprint-music-posters.github.io/trackprint-legal-docs/datenschutzerklaerung.en.html) |
| Nutzungsbedingungen | [nutzungsbedingungen.de.html](https://trackprint-music-posters.github.io/trackprint-legal-docs/nutzungsbedingungen.de.html) | [nutzungsbedingungen.en.html](https://trackprint-music-posters.github.io/trackprint-legal-docs/nutzungsbedingungen.en.html) |

The app opens the English pages. Their addresses live in one place in the app
repo, `TrackPrint/Legal/LegalLinks.swift`. If a file is renamed or the site
moves, change that file in the same release, and the footer links in
[trackprint-webpage](https://github.com/TrackPrint-Music-Posters/trackprint-webpage).

## Editing

- **Keep both languages in sync.** Any sentence changed in one language
  changes in the other in the same commit, and the sections stay in the same
  order.
- Update the "Stand" / "Last updated" date in both files of a document when
  its content changes.
- **Keep the documents true to the app.** The privacy policy names every
  place data leaves the device: Apple Music (MusicKit), MusicBrainz and the
  Cover Art Archive, iCloud (CloudKit), the feedback function on Vercel and
  GitHub, and this site on GitHub Pages. A release that adds a service, a
  request or a stored value updates the policy before it ships, together with
  the app's privacy manifest and the App Privacy label in App Store Connect.
- Each file is a standalone page: a short shared header (charset, viewport,
  `style.css`, language switch) around the document text. Edit only the text
  between the language switch and `</main>`.
- The privacy policy is adapted from text made with Datenschutz-Generator.de
  (Dr. Thomas Schwenke) and the Impressum follows eRecht24. Keep the generator
  attribution at the end of the privacy policy; the free generator licence
  requires it. For that reason this repo has no open-source licence.
- `.nojekyll` makes Pages serve the files exactly as committed.
