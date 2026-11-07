# Positive Edge Action

Keeps your [Positive Edge](https://positiveedge.dev) allowlist contract in sync with your code. On every push it re-derives `edge-contract.json` from your source, validates it with Positive Edge, and opens a pull request when your attack surface changes. No secrets needed: it authenticates with GitHub OIDC.

```yaml
name: Positive Edge
on:
  push:
    branches: [main]
permissions:
  contents: write
  pull-requests: write
  id-token: write
jobs:
  contract:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: edwardwc/positive-edge-action@v1
        with:
          dashboard-url: https://positiveedge.dev
          create-pr: true
```

This repository contains a compiled distribution only. Copyright (c) Positive Edge. All rights reserved; use is permitted only together with the Positive Edge service.
