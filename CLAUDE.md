# Project Context

This repository is `kusamau`'s fork of [jsPlumb Community Edition](https://github.com/jsplumb/community-edition)
(upstream `jsplumb/community-edition`), the free, dual-licensed connectivity library. It is kept as a
standalone repo so it can be updated/patched independently and reused across projects (e.g. Sentinel's
Klapaucius canvas).

## License compliance — read before making any change here

The original jsPlumb code is dual-licensed under **MIT and GPLv2** (full text in
[`jsPlumb-LICENSE.txt`](./jsPlumb-LICENSE.txt)). This fork elects to use and distribute its own changes
under **MIT** (the repo owner's choice — see `README.md`'s "This fork" note). These rules apply to *any*
future update in this repo, by any session or contributor:

1. **Never remove, alter, or relicense `jsPlumb-LICENSE.txt`**, or any copyright/license header embedded
   in the original source files. If a file needs a header and doesn't have one, add one — never delete an
   existing one.
2. **Don't change `package.json`'s `"license"` field** (`"(MIT OR GPL-2.0)"`) without the repo owner's
   explicit sign-off — that field describes the *original* code's terms, not just this fork's election.
3. **Keep the fork clearly attributed** as based on jsPlumb Community Edition (see `README.md`'s "This
   fork" section) — don't edit that notice away in a later pass.
4. **Syncing/upgrading from upstream**: when pulling in a newer upstream jsPlumb release or patch, keep
   the update as an isolated, clearly-described change (e.g. its own commit/PR) rather than folding it
   silently into unrelated work, so the fork's relationship to upstream — and which lines are "original
   jsPlumb" vs. "this fork's own code" — stays traceable.
5. **New code added to this fork** (patches, features, integration glue) should be MIT-compatible. Don't
   pull in GPL-only or other copyleft-incompatible dependencies/snippets without flagging it to the repo
   owner first — that could complicate the fork's MIT election over the whole tree.
6. **This is not legal advice.** These are working notes based on the repo owner's own review with a
   colleague, not a legal opinion. If a planned change raises a real licensing question (e.g. redistributing
   a modified build, relicensing a specific file, using this code in a commercial product), flag it to the
   repo owner rather than deciding unilaterally.

## Standards

No project-specific coding standards recorded yet beyond the license rules above — this fork otherwise
follows upstream jsPlumb Community Edition's existing code style and structure.
