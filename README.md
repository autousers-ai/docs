# Autousers — Developer Docs

Source of [docs.autousers.ai](https://docs.autousers.ai) — the public developer reference for Autousers, the AI-driven UX evaluation platform.

[![Docs site](https://img.shields.io/badge/docs.autousers.ai-live-9CFF00)](https://docs.autousers.ai)
[![License](https://img.shields.io/badge/content-proprietary-lightgrey)](#license)

---

## What this repo is

A snapshot of the published documentation tree, mirrored from the upstream Autousers monorepo. Everything you read on `docs.autousers.ai` lives here as Markdown / MDX, plus the `docs.json` configuration file.

The site itself is built with [Mintlify](https://mintlify.com) and rebuilds automatically on every push to `main`.

## Structure

```
.
├── docs.json                       # Mintlify configuration (nav, theme, OpenAPI)
├── introduction.mdx                # Overview of the API surface
├── quickstart.mdx                  # Mint a key, make your first call
├── authentication.mdx              # Four auth paths, scope vocabulary
├── errors.mdx                      # Error envelope + request-id correlation
├── pagination.mdx                  # Cursor pagination
├── rate-limits.mdx                 # Per-tier limits + headers
├── idempotency.mdx                 # Idempotency-Key on POSTs
├── versioning.mdx                  # API versioning policy
├── concepts/                       # Data-model deep dives
├── webhooks/                       # Event delivery + signing + replay
├── integrations/                   # MCP, CLI, Figma, Chrome, SDKs, recipes
└── changelog.mdx                   # Per-release notes
```

API reference pages (`/api-reference/*` on the live site) are auto-rendered by Mintlify from [`https://app.autousers.ai/api/v1/openapi.json`](https://app.autousers.ai/api/v1/openapi.json) and aren't kept here as MDX.

## Reading

The published reader at [docs.autousers.ai](https://docs.autousers.ai) is the canonical surface. Read these files only if you need the raw source (e.g. for offline access or to feed an AI assistant context).

## Contributing

This repository is an **automatically-generated mirror** of the upstream Autousers monorepo. Direct pushes here are overwritten on the next mirror sync.

- **Found a bug or have a suggestion?** [Open an issue](https://github.com/autousers-ai/docs/issues) — we review every one.
- **Need to talk to support?** Email [contact@autousers.ai](mailto:contact@autousers.ai) or join us at [autousers.ai/help](https://autousers.ai/help).
- **Want to integrate?** The [REST API reference](https://docs.autousers.ai/api-reference), the [`@autousers/cli`](https://www.npmjs.com/package/@autousers/cli) command-line tool, and the [`@autousers/mcp`](https://www.npmjs.com/package/@autousers/mcp) MCP server are the right entry points today. Typed TypeScript and Python SDKs are on the roadmap.

## Sister repos

| Repo                                                        | What it is                                         |
| ----------------------------------------------------------- | -------------------------------------------------- |
| [`autousers-ai/mcp`](https://github.com/autousers-ai/mcp)   | Official MCP server (`@autousers/mcp`)             |
| [`autousers-ai/cli`](https://github.com/autousers-ai/cli)   | Official command-line interface (`@autousers/cli`) |
| [`autousers-ai/docs`](https://github.com/autousers-ai/docs) | This repo — docs.autousers.ai source               |

## License

Documentation content is © Autousers, all rights reserved.

Code samples embedded in the MDX files are released under the **MIT license** for use in your own integrations — verbatim copy is welcomed and encouraged.

---

Built with ❤️ by the Autousers team. Site rendered by [Mintlify](https://mintlify.com).
