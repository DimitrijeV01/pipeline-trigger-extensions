# pipeline-trigger-extensions

A focused fork of two upstream repositories by [@huserben](https://github.com/huserben) (Benjamin Huser-Berta), both MIT-licensed:

- [huserben/TfsExtensions](https://github.com/huserben/TfsExtensions) — build tasks for triggering, waiting on, and cancelling Azure DevOps pipelines. Preserved under [`tfsextensions/`](./tfsextensions). The dashboard widgets from upstream are not maintained in this fork and have been removed.
- [huserben/tfsrestservice](https://github.com/huserben/tfsrestservice) — REST API library consumed by the build tasks. Preserved under [`tfsrestservice/`](./tfsrestservice).

Each subdirectory keeps its own `README` and `LICENSE` from the original repository. Full git history of both upstreams is preserved.

## Motivation

To publish a new version of the TriggerBuild task with additional capabilities on top of the upstream design. Background discussion: [huserben/TfsRestService#20](https://github.com/huserben/TfsRestService/issues/20).
