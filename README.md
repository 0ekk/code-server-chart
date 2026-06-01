# code-server Helm chart repository

This repository publishes the Helm chart from `coder/code-server` releases.

The GitHub workflow runs every day at 00:00 UTC, checks the latest stable
upstream `coder/code-server` tag, and skips publishing only when this
repository already has a matching GitHub release tag and `gh-pages` already has
the matching chart package and index entry.

After a successful sync, the chart repository is available from:

```sh
helm repo add code-server https://0ekk.github.io/code-server-chart
helm repo update
```
