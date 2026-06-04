**Submit vocabulary additions and edits by dropping an Excel file into this folder and opening a pull request.**

## How to contribute

1. Download the current vocabulary Excel file from the latest published build:
   `https://aggateway.github.io/semreg/dev/semreg.xlsx`
2. Edit the file — add or update concepts within your assigned ID range (see `idranges.toml`).
3. Rename the file `semreg.xlsx` (the stem must match the vocabulary name exactly).
4. Copy the file into this folder, commit it to a new branch, and open a pull request against `main`.

## What happens next

The CI pipeline (`ci-pr.yml`) will automatically:

- Validate your Excel file and ID range assignments.
- Convert valid entries to Turtle (`.ttl`) files under `vocabularies/semreg/`.
- Commit the generated Turtle files back to your pull request branch.
- Remove the Excel file from the pull request.
- Upload an annotated Excel file and log as a [workflow artifact](https://docs.github.com/en/actions/managing-workflow-runs/downloading-workflow-artifacts) — check this if there are validation errors.

## ID ranges

| Range     | Owner / Topic                      |
|-----------|------------------------------------|
| 1000–1999 | PLSS (Public Land Survey System)   |
| 2000–2999 | WMO (World Meteorological Org.)    |
| 3000–3999 | USDA                               |
| 4000–4999 | EPA                                |
| 5000–5999 | MODUS                              |
| 6000–6999 | WG35                               |
| 7000–9999 | Reserved                           |
