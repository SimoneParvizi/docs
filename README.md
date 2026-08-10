# blueaccademy-docs

This repository contains the Mintlify documentation site for BlueAccademy.

Production site:

- `https://docks.blueaccademy.com/`

Related repositories and URLs:

- Main product repo: `~/blueaccademy`
- Public docs index for LLMs: `https://docks.blueaccademy.com/llms.txt`

## What belongs here

This repo documents:

- What BlueAccademy currently supports
- How to install the contributor toolchain
- How to run the current stack locally
- How the main product repo is structured
- How the current application workflow behaves
- How to contribute to the docs site

This repo should not invent support for product areas that are still in progress.

## Current product status

The stable supported slice today is the flashcard system.

In progress:

- Guided terminal exercises

Not yet supported:

- CKAD-style simulations
- Broader end-to-end labs
- Chat
- Hosted sandbox orchestration

## Local docs development

Use an LTS Node release before installing the Mintlify CLI. Mintlify's CLI docs currently require Node.js `v20.17.0+` and recommend LTS versions.

Install the correct CLI package:

```bash
npm i -g mint
```

Do not install `mintlify` for local docs development here.

Verify the CLI:

```bash
mint version
```

Run the docs locally from this repository:

```bash
mint dev
```

The local preview runs at `http://localhost:3000`.

## Editing guidance

- Keep docs aligned with the current state of `blueaccademy`
- Prefer status accuracy over marketing language
- Avoid turning internal code paths into public promises
- Use Mintlify-friendly page structure and concise headings
- Treat the main repo README as lightweight and this site as the deeper reference

## Useful files

- `docs.json` for navigation and site config
- `index.mdx` for the docs homepage
- `flashcards/` for the current stable product slice
- `architecture/` for repo/runtime structure
- `contributing/` for contributor guidance

## Mintlify references

- Mintlify docs: `https://mintlify.com/docs`
