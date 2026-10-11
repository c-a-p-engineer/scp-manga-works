# AGENTS.md — SCP Manga Works

## Purpose
This repository is the **workspace for an unofficial, serialized SCP manga**. It stores story continuity, reusable cast information, text manga names, and generated/reviewed manga images. It is not the Manga Blueprint Studio implementation repository.

## Read order
1. Read this `AGENTS.md` on the current `master` before making changes.
2. Read `README.md` and `episodes/README.md` for current scope and the canonical episode list.
3. If changing a specific episode, read that episode's `README.md` and its existing name/images.
4. If writing/compiling manga Blueprints or generating comic images, check the **current** `master` of `c-a-p-engineer/manga-blueprint-studio`, beginning with its `AGENTS.md` and `.agents/skills/manga-blueprint/SKILL.md`, then their required sources of truth.
5. Do not rely on old cached versions of Studio rules.

## Ownership
- `series/`: continuing series premise, chronology and continuity.
- `characters/`: recurring character definitions, including whether still provisional.
- `episodes/README.md`: **single human-maintained episode list and status index**.
- `episodes/EP###_SCP-<number>/`: episode-specific work, including `name/` (text names) and `images/drafts/` / `images/final/`.
- Generated outputs belong in this repository, **not** Studio fixtures/examples or the generic `manga-blueprint-works` repository, unless the user explicitly directs otherwise.

## Episode policy
- Each episode is independently identifiable by `EP001`, `EP002`, etc. The associated SCP number is separate from the episode number.
- One-page entries use `P001` in file names; manga defaults to Japanese RTL reading and vertical Japanese lettering unless the work says otherwise.
- Keep planning, draft generations, and accepted final art separate. Do not mark a generated image final without review.
- Changes to an episode's status require corresponding updates to `episodes/README.md`.
- Do not silently finalize character names, appearance, dialogue, storyline, or lore choices flagged provisional.
- Verify each featured SCP's current primary article before writing a final name, especially containment rules and observable behavior.

## Image storage
- Store selected useful generation candidates under `images/drafts/`; accepted artwork under `images/final/`.
- Prefer one canonical final file per page (`P001.png`) and revision-tagged drafts (`P001-v01.png`).
- PNGs around 2MB are acceptable initially. Avoid committing throwaway iterations or caches. Deleting tracked PNGs does **not** remove their Git history.
- No automatic Git LFS, external paid storage, workflows, or new Actions without separately checking permission and tradeoffs.

## Attribution
SCP-based derivative manga must carry the source article title, original author, source URL and CC BY-SA 3.0 attribution/license. See `CREDITS.md` and each episode's credits. Do not reuse original SCP page images or other third-party media without checking their **separate** rights.

## GitHub Actions
Do not create new workflows or introduce new uses without prior approval. Existing validation workflows may be used within the user's standing permission, but artwork-generation workflows have their own stricter Studio/Works production boundaries.

## Completion
For documentation/index updates: verify all links and recorded states against the committed `master`. For manga: additionally follow the Studio handoff, visual review, and per-page acceptance contracts.
