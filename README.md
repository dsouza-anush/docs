# Heroku AI Documentation

This repository hosts the product documentation for the Heroku AI platform. The site covers model provisioning, API usage, CLI workflows, and integrations so teams can build and run AI features on Heroku.

## Directory guide

- `quickstart.mdx` – first-call walkthrough for the inference API
- `inference-api/` – REST and SDK guides, model catalog details, pricing, and CLI reference
- `heroku-inference/` – AI Studio and Model Context Protocol (MCP) runtime guides
- `tool-use/` – instructions for connecting external toolchains to MCP servers
- `vector-database/` – PostgreSQL + pgvector setup guidance
- `ai-integrations/` – examples for popular frameworks and partner libraries

## Preview the docs

The site is built with Mintlify. Install the CLI globally, then run a local preview from the `docs/` directory:

```bash
npm install -g mint
mint dev
```

Your preview is available at `http://localhost:3000`. Changes are hot-reloaded while the dev server runs.

## Contribution workflow

1. Create a feature branch for your update.
2. Edit or add MDX files; keep frontmatter (`title`, `description`) up to date.
3. Run `mint dev` to verify navigation links and embedded components.
4. Open a pull request and include screenshots or notes for reviewer validation.

## Support

For questions about the Heroku AI product or this documentation, reach out through the Heroku support portal or your account representative. For updates to the site generator, consult the Mintlify release notes before upgrading the CLI.
