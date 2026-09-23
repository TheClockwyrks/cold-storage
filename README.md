# cold-storage

Large generated media for The Test Cabinet, checked out as the `cold-storage`
submodule at the root of `the-test-cabinet`.

The tree mirrors the superproject's, so a test-case version's baseline
validation media lives at
`test-cases/<type>/<difficulty>/<slug>/<version>/validation-baseline/<engine>/<variant>/`.
`tcab capture-baselines` and `tcab publish-reference` write it, and backend
ingest reads it.

History is never rewritten: every superproject commit pins a commit here.
