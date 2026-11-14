# Vote Action officials data

Static roster files for the Vote Action app, published with GitHub Pages at
`https://ezgstudio.github.io/voteaction-data/v1/`.

- `v1/manifest.json`: build version, and each file's size and SHA-256.
- `v1/<state>.json`: one file per state. `ma.json` holds Massachusetts (legislature, Congress,
  statewide officials, towns and local councils); other states hold a Census-only roster.

The files are generated from reviewed sources (state legislatures, Open States, the
unitedstates/congress-legislators project, official city and town rosters). The app checks
each file against the manifest hash before using it. Don't edit by hand: they are rebuilt
and published from the app project with `scripts/publish_hosted_data.sh`.
