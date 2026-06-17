## ⟳ SESSION-START REFRESH — read first, every session (mandatory)

Before doing ANY work in this session:

1. **Hard-pull this repo** so you are on the latest canonical state:
       git pull origin main
2. **Re-read this CLAUDE.md top to bottom.** It may have changed since your last session.
3. **Pull the canonical standards once — one shallow clone, then read from it** (this is what realizes any new or changed standard automatically; the standards are single canonical copies, no local mirror to drift):
       rm -rf /tmp/hri-template && gh repo clone Hope-Rises-International/hri-template-repository /tmp/hri-template -- --depth 1
   **Fail closed:** this clone is the ONLY source of the rails (no mirror fallback). If it fails or `/tmp/hri-template/RESTRUCTURE-RULES.md` is absent, **STOP** and tell the operator — do not work without the rails. Then from `/tmp/hri-template`: **read `RESTRUCTURE-RULES.md` every session** (the canonical rails). Before writing **any** integration code, also read `hri-integration-standards.md` + `hri-stack-learnings.md` there. The session-start / session-end / comprehension protocols live in the same clone. If you see a standards doc you don't recognize, read it and tell the operator. (Architect sessions also read `hri-architect/CLAUDE.md`, the Operating Manual.)

**Mid-session:** do a SOFT check only —
       git fetch && git status -sb
— and tell the operator if you are behind. Do NOT hard-pull mid-session; it can clobber in-progress edits.

This block is mandatory and identical across every HRI repo. If it is missing from a repo's CLAUDE.md, add it and tell the operator — that repo had drifted off the rails.

---

# accord-strategy-explorer

Interactive Strategy & Operations framework — HRI leave-behind for the Accord Network AI webinar.
