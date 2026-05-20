# sicg-icon-library

Icon and illustration asset library for Social Interest Consulting Group's
"Drawing Studio". This is an **asset repository**, not a code project — it
holds raster artwork, not source code or a build pipeline.

## Contents

- ~204 `.png` files in the repository root, one icon/illustration per file.
- `README.md` — one-line description.
- No source code, no build step, no dependencies, no tests.

## Naming conventions

Filenames are lowercase, hyphen-separated, and describe the subject
(`kebab-case`). Observed groupings:

- **Generic UI / object icons**: `arrow-right.png`, `calendar.png`,
  `magnifying-glass.png`, `gear-single.png`, `folder-open.png`, etc.
- **People / roles**: `doctor.png`, `nurse.png`, `social-worker.png`,
  `business-woman.png`, `firefighter.png`, etc.
- **Domain-specific (behavioral health / SMHRF / consulting)**: prefixes
  like `smhrf-*` (e.g. `smhrf-administrator.png`), `consumer-*`
  (e.g. `consumer-arrival-gurney.png`), `consultation-*`, `rsa-*`,
  and assessment icons (`qualitative-assessment-icon.png`).

When adding a new asset, follow the existing pattern: lowercase
`kebab-case`, descriptive name, `.png` extension, placed in the repository
root. Use an existing prefix when the icon belongs to one of the domain
groupings above.

## Working with this repo

- There is nothing to install, build, or run.
- Changes are purely file additions/removals/renames of `.png` assets.
- Keep filenames stable — downstream projects (e.g. `sivc-web`) may
  reference these assets by name.
- Git history shows assets are added in bulk ("Add files via upload"
  commits); preserve that simple add-only workflow.

## Notes for AI assistants

- Do not attempt to add tooling, package manifests, or CI to this repo
  unless explicitly asked — it is intentionally just an asset store.
- This repo is binary-asset-heavy; avoid bulk operations that rewrite or
  re-encode the PNGs.
