---
id: mem_1431269c
vertical: engineering
memory_type: action
action_type: procedure
level: tactical
primitive: procedure
engineering_domains:
  - code_structure
  - runtime_behavior
  - review_preference
subjects:
  - responsive UI
  - project cards
  - desktop/mobile behavior
symbols: []
tags:
  - responsive
  - mobile-unchanged
  - desktop-limit
status: active
confidence: medium
authority: reviewed
owner: arcanist
applies_to: []
context_hint: Any time a page shows a different number of cards or items on desktop vs mobile and the request mentions only one platform.
source_pr_urls:
  - https://github.com/Varun901/varun901.github.io/pull/9
source_session_ids:
  - 65993af2-405f-4125-943d-bffb5c63c88a
evidence: []
enforcement: none
supersedes: []
contradicts: []
created_at: 2026-06-11
updated_at: 2026-06-11
---

When changing a project-card preview limit, update only the desktop/web branch and leave the mobile rendering logic unchanged unless the user explicitly asks to change both.
