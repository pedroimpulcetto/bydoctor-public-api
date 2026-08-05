# Documentation project instructions

## About this project

- Public developer documentation for the ByDoctor public API and webhooks, published at `https://docs.bydoctor.com.br` (built on [Mintlify](https://mintlify.com)).
- Pages are MDX files with YAML frontmatter. Configuration lives in `docs.json`.
- `openapi.json` is a **generated build artifact** from `api-bydoctor`'s
  `python manage.py generate_public_openapi --output` — never hand-edit it.
  If the reference looks wrong, fix the serializer/filter in `api-bydoctor`
  and regenerate.

## Terminology

- Prose, headings, and navigation labels are **pt-BR** — the audience is
  Brazilian clinic software vendors and in-house developers.
- Code identifiers, HTTP header names, JSON field names, and status values
  stay in English — they are the wire contract, not copy.
- Match the app's UI labels exactly, e.g. "Minha Clínica" (capital C).

## Style preferences

- Use active voice and second person ("você").
- Keep sentences concise — one idea per sentence.
- Code formatting for file names, commands, paths, headers, and field names.
- Verify claims against the `api-bydoctor` backend source before writing them
  — do not guess at field shapes, defaults, or status codes.

## Content boundaries

- Document only the public contract exposed under `/api/public/v1/` and its
  webhooks. No internal admin/private API surface.
