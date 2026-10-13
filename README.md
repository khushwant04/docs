# docs

A [Mintlify](https://mintlify.com) documentation site scaffold.

**Status:** this repository currently contains the unmodified Mintlify starter kit (a snapshot committed in November 2025 from
[mintlify/starter](https://github.com/mintlify/starter)). The pages, navigation, branding (`"name": "Mint Starter Kit"`,
Mintlify logos, support links) and the sample OpenAPI spec are all starter placeholders; no project-specific
documentation has been written yet.

## Structure

```
.
├── docs.json          # Site config: theme, colors, navigation, navbar, footer
├── index.mdx          # Landing page
├── quickstart.mdx
├── development.mdx
├── essentials/        # Starter pages showing Mintlify components
├── ai-tools/          # Starter pages for Cursor, Claude Code, Windsurf
├── api-reference/     # Sample API reference generated from openapi.json
├── snippets/          # Reusable MDX snippets
├── images/, logo/, favicon.svg
└── DV LAB-5th sem(2022).pdf   # Unrelated file (college lab manual), not part of the site
```

## Local preview

Requires Node.js.

```bash
npm i -g mint
mint dev          # run from the repo root, where docs.json lives
```

Open http://localhost:3000.

## Customizing

1. Update `name`, `colors`, `logo`, `navbar` and `footer` in `docs.json`.
2. Replace the starter pages and the navigation entries that point to them.
3. Replace `api-reference/openapi.json` with a real spec, or remove the API reference tab.

## Publishing

Install the Mintlify GitHub app from the Mintlify dashboard; pushes to the default branch then deploy automatically.

## License

`LICENSE` is the MIT license inherited from the Mintlify starter (Copyright (c) 2023 Mintlify).
