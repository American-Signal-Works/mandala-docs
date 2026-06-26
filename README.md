# Backdesk docs

This repository contains the Mintlify documentation site for the current Backdesk system.

## Development

Run commands from the repository root, where `docs.json` is located:

```bash
npx mintlify@latest validate
npx mintlify@latest broken-links
npx mintlify@latest dev
```

The local preview runs at `http://localhost:3000`.

## Content map

- `index.mdx` introduces the current system.
- `development.mdx` covers local setup and workflow.
- `system/*.mdx` documents architecture, data model, auth, collections, imports, API routes, and operations.
- `docs.json` controls Mintlify navigation and site settings.

## Maintenance

Update docs in the same change as the code or system behavior they describe. Before publishing, run:

```bash
npx mintlify@latest validate
npx mintlify@latest broken-links
```
