# GrandTour content

The published GrandTour tracks, as any GrandTour server serves them: a
[`grandtour.json`](grandtour.json) index naming one bundle per track under
[`tours/`](tours). Point the app at this repository (Tracks → Server →
`github.com/gtfyi/content`) or at [grandtour.fyi](https://grandtour.fyi),
which serves the same files. Recordings live at
`https://data.grandtour.fyi/audio/<sha256>.<ext>`, named inside each bundle.

The files follow the schemas in
[`@grandtour/shared`](https://github.com/gtfyi/grandtour/tree/main/packages/shared)
(`Index`, `IndexTrack`, `TrackExport`); see the monorepo's
[docs/distribution.md](https://github.com/gtfyi/grandtour/blob/main/docs/distribution.md).
Published from the private repository of record by `content:publish`.

## Licence

GrandTour's own text and recordings are released under the MIT licence
([LICENSE](LICENSE)). Third-party content keeps its own terms, stated per
piece in `provenance.origin` inside each bundle: the National Park Service
tours are United States government work in the public domain
(17 U.S.C. §105), with the attribution lines their descriptions carry. A
piece's `origin.license` is the term that applies to it; `clearance`
records that someone checked.
