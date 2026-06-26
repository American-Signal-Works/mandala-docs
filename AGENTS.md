# Documentation project instructions

## About this project

- This is the Mintlify documentation site for the Backdesk system.
- Pages are MDX files with YAML frontmatter.
- Configuration lives in `docs.json`.
- Use the Mintlify MCP server, `https://mcp.mintlify.com`, when available.
- Use the Mintlify docs MCP server, `https://www.mintlify.com/docs/mcp`, to query Mintlify usage details when available.

## Terminology

- Use "Backdesk" for the product.
- Use "workspace" for the user-facing product concept.
- Use "page", "dashboard", "collection", "connection", and "system collection" consistently with the app.

## Style preferences

- Use active voice and second person ("you").
- Keep sentences concise, one idea per sentence.
- Use sentence case for headings.
- Bold UI element names, for example: Click **Settings**.
- Use code formatting for file names, commands, paths, and code references.
- Describe current behavior from source, not hoped-for behavior from older specs.

## Content boundaries

- Keep docs source-backed and current with the Backdesk repository.
- Do not document roadmap items as shipped behavior.
- Label caveats clearly when implementation differs from older product specs.

## Docs impact routing

- App/routes/shell changes: update `system/architecture.mdx`.
- DB/RLS/storage changes: update `system/data-model.mdx`.
- Auth/middleware/session changes: update `system/auth.mdx`.
- Collections/blocks/views changes: update `system/collections.mdx`.
- Imports/connections/parsers changes: update `system/imports.mdx`.
- Route handler/API shape changes: update `system/api.mdx`.
- Env/CI/tests/ops changes: update `system/operations.mdx`.
- Setup/workflow changes: update `development.mdx`.

## Validation

Before publishing, run:

```bash
npx mintlify@latest validate
npx mintlify@latest broken-links
```
