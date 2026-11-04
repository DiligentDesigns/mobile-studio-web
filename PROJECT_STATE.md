# Mobile Studio Web — project-state and continuity proposal

**Product ID:** DAW; **surface:** separate browser prototype, not automatically equivalent to native Studio Noir. **Status of this document:** proposed in `foundation/project-state-v1`, not merged. Snapshot from `main` at `9ed91453cd7c1eac9d00fedf537822cd8f76650f`; refresh actual HEAD each session.

## Start every new conversation

Read the private [Foundation START_HERE](https://github.com/DiligentDesigns/Software-company-foundation/blob/foundation/continuity-v1/START_HERE.md), the DAW native repository's `PROJECT_STATE.md` proposal, this file, repository `README.md`, current `index.html`, latest commits and test logs. Source claims and behavior must be checked independently; the web and native prototypes have different implementation and release status.

## Source and acceptance

- The existing `index.html` identifies itself as Mobile Studio v0.5.0-alpha with take lanes and a touchscreen-oriented browser UI.
- The repository `README.md` describes a mobile-first multitrack recording, editing and musical timing **interactive web prototype**. That description does not certify native mobile hardware, long-session audio or professional recording alignment.
- Authoritative shared DAW product engine is being developed separately in private `DiligentDesigns/mobile-studio-daw` branch `migration/studio-noir-foundation` (draft PR #1). Neither repo may silently overwrite the other, nor claim compatibility simply because UI labels look alike.
- Last browser owner-approved stable release: **not verified**. Cross-platform project schema, sync, end-to-end audio and browser/desktop feature parity: **not verified**.

## Protected behavior and wiring

```text
browser UI -> client-side state/actions -> WebAudio/browser media where implemented
               |-> project representation -> exports/persistence as implemented
Native Studio Noir has independent C++/Core Audio source and separate hardware test gates.
```

This is orientation only; inspect `index.html` and explicit source functions before changing pathways, and document actual working behavior rather than inferring it from this diagram. Preserve accessible touch controls, original media, future project schema versioning, and record/stop/close/reopen reliability.

## Next action

Inventory current actual browser features, tests and persistence/export behavior against native DAW; record missing parity and stable IDs before attempting shared project compatibility or source merging. Introduce focused web CI on a dedicated PR. Keep existing browser demo unchanged until the acceptance matrix is approved.

**Rollback/handoff:** retain source commit, keep a branch for every experimental change, report PASS/FAIL/SKIP/NOT_RUN and link to verifiable preview/device evidence. Never claim native hardware checks from browser tests. For a new session, inspect the foundation registry and native DAW state before implementing features.
