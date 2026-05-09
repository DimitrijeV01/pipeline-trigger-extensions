# pipeline-trigger-extensions

A focused fork of two upstream repositories by **Benjamin Huser-Berta**, both MIT-licensed:

- [huserben/TfsExtensions](https://github.com/huserben/TfsExtensions) — build tasks for triggering, waiting on, and cancelling Azure DevOps pipelines. Preserved under [`tfsextensions/`](./tfsextensions). The dashboard widgets from upstream are not maintained in this fork and have been removed.
- [huserben/tfsrestservice](https://github.com/huserben/tfsrestservice) — REST API wrapper consumed by the build tasks. Preserved under [`tfsrestservice/`](./tfsrestservice).

Each subdirectory keeps its own `README` and `LICENSE` from the original repository. Full git history of both upstreams is preserved.

## Why merged

Combining the two repositories removes the publish-and-republish dependency between them: changes to the wrapper and the consuming build tasks can be developed and shipped together without an intermediate `npm publish` step. The wrapper is consumed by tasks via a `file:` dependency, and the resulting `.vsix` task package bundles it inline at packaging time.
