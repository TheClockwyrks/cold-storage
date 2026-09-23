# cold-storage

Large generated media for The Test Cabinet, checked out as the `cold-storage`
submodule at the root of `the-test-cabinet`.

The tree mirrors the superproject's, so a test-case version's baseline
validation media lives at
`test-cases/<type>/<difficulty>/<slug>/<version>/validation-baseline/<engine>/<variant>/`.
`tcab capture-baselines` and `tcab publish-reference` write it, and backend
ingest reads it.

History is never rewritten: every superproject commit pins a commit here.

The superproject names this repository by the relative URL `../cold-storage`,
so it resolves on whichever host the superproject was cloned from. Azure Repos
is where it lives, and `TheClockwyrks/cold-storage` on GitHub is its mirror.
The pipeline in `.azure-pipelines/mirror.yml` force-pushes `master` there on
every push to `master`, and nothing else writes to the mirror.
