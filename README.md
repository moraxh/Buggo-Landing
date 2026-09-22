# Buggo landing page

The hand-drawn home of [Buggo](https://github.com/moraxh/Buggo), a bug investigator for developers and coding agents. Buggo turns a bug report into a ranked list of files worth inspecting. The suspects are leads, not a confirmed diagnosis.

This repository contains the website, built with [Astro](https://astro.build/). The CLI and MCP server live in the [main Buggo repository](https://github.com/moraxh/Buggo).

The detective artwork, paper texture, case file, and small details give the page its comic-book feel. The cat testimonials are jokes, deliberately fictional. The investigation shown in the case file comes from the real run documented in Buggo's README.

## Run locally

Requires Node.js 22 or later and pnpm.

```bash
pnpm install
pnpm dev
```

Open the local URL printed by Astro. To create a static build:

```bash
pnpm build
pnpm preview
```

## Project structure

- `src/pages/index.astro`: page content and scroll interactions
- `src/styles/global.css`: layout, typography, paper treatment, and motion
- `public/images/`: detective artwork, texture, and investigation demo
- `public/testimonies/`: the fictional reviewers

## Try Buggo

```bash
npm install -g @moraxh/buggo
buggo config set-key <your-openrouter-key>
buggo investigate "describe your bug" --repo /path/to/your/repo
```

See the [Buggo README](https://github.com/moraxh/Buggo#readme) for the CLI, JSON output, and MCP setup.
