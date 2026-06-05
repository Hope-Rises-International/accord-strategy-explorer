## ⟳ SESSION-START REFRESH — read first, every session (mandatory)

Before doing ANY work in this session:

1. **Hard-pull this repo** so you are on the latest canonical state:
       git pull origin main
2. **Re-read this CLAUDE.md top to bottom.** It may have changed since your last session.
3. **Re-read the canonical rails** that govern every HRI architect and builder session:
       gh api "repos/Hope-Rises-International/hri-template-repository/contents/RESTRUCTURE-RULES.md?ref=main" --jq '.content' | base64 -d
   (Architect sessions: also read hri-architect/CLAUDE.md and its RESTRUCTURE-RULES mirror.)

**Mid-session:** do a SOFT check only —
       git fetch && git status -sb
— and tell the operator if you are behind. Do NOT hard-pull mid-session; it can clobber in-progress edits.

This block is mandatory and identical across every HRI repo. If it is missing from a repo's CLAUDE.md, add it and tell the operator — that repo had drifted off the rails.

---

# accord-strategy-explorer

Interactive Strategy & Operations framework — HRI leave-behind for the Accord Network AI webinar.
