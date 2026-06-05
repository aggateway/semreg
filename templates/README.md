## Excel templates

Place a custom Excel template here named `default_sheets.xlsx` and it will be picked up automatically by the CI pipeline (pre-configured in the GitHub Actions workflows).

Use this to provide contributors with a pre-formatted workbook — for example, with a help sheet or an about sheet describing AgGateway semreg conventions.

Templates may not contain any of the sheets that voc4cat-tool generates dynamically (e.g. the concept sheet). See the [voc4cat-tool documentation](https://nfdi4cat.github.io/voc4cat-tool/migration-to-v1.0.html#step-4-generate-v1-0-excel-template) for details.

As of voc4cat-tool v1.0.0, templates are optional — the pipeline will issue a warning if none is found but will continue normally.
