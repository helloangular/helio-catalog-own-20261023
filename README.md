# helio-catalog-own-20261023

Synthetic test fixture for Helio's Environment Catalog acceptance cases (BlueMatrix, 23 Oct 2026).
Nothing here deploys anything: every job prints a line and sleeps. The repository holds no secrets.

- `.github/workflows/catalog-own-release.yml`: pure catalog caller of the central template
  `helloangular/helio-client-capacity-20260916/.github/workflows/catalog-own-deploy.yml@catalog-own-20261023`.
- `.github/workflows/catalog-own-mixed.yml`: the same template after a team `cown-team-qa` job.
- `VERSION`: changed to make a new commit; every commit is tagged `helio/workflow/<sha>` in the same step.
- `.helio-cown/catalog-fail/<environment>` / `.helio-cown/catalog-slow/<environment>`: per-commit switches.
