# Pipeline sizing

Choose jobs from measured build time, repository layout, deployment topology, release frequency,
and failure impact. These are starting points, not fixed project-size tiers.

- **Single service or small app:** one PR validation path, one reproducible build, staging smoke
  test, protected production promotion of the same digest, and a rollback job. Keep jobs serial
  when parallelism would add more setup than it saves.
- **Multi-service or monorepo:** split independent tests by service, reuse common job definitions,
  cache immutable dependencies, and build only affected artifacts. Keep integration and release
  checks across services when a shared contract changes.
- **High-impact or frequent releases:** add provenance and policy checks, environment locks,
  progressive rollout, bake windows, automatic abort signals, and independent rollback drills.
  Add regions or deployment waves only when availability and recovery requirements justify them.

Measure pipeline duration and failure causes after rollout, then simplify or parallelize accordingly.
