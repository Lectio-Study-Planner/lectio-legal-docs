# Lectio legal documents

The Impressum (legal notice, DDG) and Datenschutzerklärung (privacy policy,
DSGVO/GDPR) for the Lectio semester planner, in German and English. This repo
is the only copy: the app links here from Settings ▸ About, and the privacy
policy URL in App Store Connect points here too.

## Published at

GitHub Pages serves `main` from the repo root:

| Document | German | English |
|---|---|---|
| Impressum | [impressum.de.html](https://lectio-study-planner.github.io/lectio-legal-docs/impressum.de.html) | [impressum.en.html](https://lectio-study-planner.github.io/lectio-legal-docs/impressum.en.html) |
| Datenschutzerklärung | [datenschutzerklaerung.de.html](https://lectio-study-planner.github.io/lectio-legal-docs/datenschutzerklaerung.de.html) | [datenschutzerklaerung.en.html](https://lectio-study-planner.github.io/lectio-legal-docs/datenschutzerklaerung.en.html) |

The app opens the English pages. Their addresses live in one place in the app
repo, `Lectio/Legal/LegalLinks.swift`. If a file is renamed or the site moves,
change that file in the same release.

## Editing

- **Keep both languages in sync.** Any sentence changed in one language changes
  in the other in the same commit, and the sections stay in the same order.
- Update the "Stand" / "Last updated" date in both privacy-policy files when
  their content changes.
- Each file is a standalone page: a short shared header (charset, viewport,
  `style.css`, language switch) around the document text. Edit only the text
  between the language switch and `</main>`.
- The privacy policy was generated with Datenschutz-Generator.de and the
  Impressum with eRecht24. Keep the generator attribution at the end of the
  privacy policy; the free generator licence requires it. For that reason this
  repo has no open-source licence.
- `.nojekyll` makes Pages serve the files exactly as committed.
