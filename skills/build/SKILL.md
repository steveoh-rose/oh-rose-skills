---
name: build
description: Implements or changes UI code. Use when the user asks to build, code, fix, refactor or ship a component, page or style change, including metadata and forms.
---

# Build

Make the smallest change that solves the problem.

## Before changing code

1. Inspect the repo: framework, dependencies, routes, conventions, scripts.
2. Identify the pages, components, styles, content and interactions affected.
3. Look for existing tokens, components and utilities first.

## Rules

- Semantic HTML. Abstract only when reuse is genuine.
- No new dependency without a clear need.
- No raw values where a token exists. No parallel token system.
- Keep content separate from presentation where the architecture allows.
- Size media to avoid layout shift. Keep control dimensions stable across states.
- Respect `prefers-reduced-motion`. Keep visible focus.
- No analytics, tracking or third-party scripts without approval.
- No secrets or private data in client code.
- Do not assume the CMS, host, analytics or form service. Check.
- Forms: clear labels, plain errors, input kept after errors, clear success. No mailing list signup without consent.
- Pages: accurate title, description, social metadata, descriptive headings and links.

## Verify

Run lint, types, tests and build if they exist. Exercise the real interaction by keyboard and in a browser. Then run `review`.

## Output

What changed and where, what was verified and how, what was not verified, assumptions made.

## References

- [references/pre-flight.md](references/pre-flight.md): repo, scope, build, forms, pages and after-build checklists

For animation, use `motion`. Before adding a dependency, use `libraries`.
