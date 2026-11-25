# Agent Notes

- When modifying any userscript in this repository, always increment the `@version` header in the edited script.
- Use the next patch version by default unless the change clearly requires a different versioning step.
- For new userscripts, create only the `.user.js` file. Do not add a legacy non-`.user.js` shim unless the user explicitly asks for it.
- The integrated browser does not run Tampermonkey/Violentmonkey automatically, so live userscript testing requires manual script injection.
- When testing message-detail flows, watch for page localization and verify the behavior in both English and Czech labels/texts, not just one language variant.

## Screenshots for README and docs

- Every screenshot in `docs/images/` must be anonymized. Before taking it, replace in the page DOM (not on the server) the user's name and photo, people's names, ticket keys and worklog texts, file and attachment names, message/document IDs, EIC codes, internal host names, IP addresses, certificates and artifact URLs with neutral placeholders (e.g. `Jan Novák`, `ABC-123`, `example.com`, `report-2026.pdf`).
- Use a public or test environment (e.g. T1), never production data. Leave out views that show secrets or infrastructure (request headers, certificates, IPs) even when anonymized.
- Do not publish a screenshot that still shows real personal or customer data; check the saved PNG before adding it to the README.
