# Anchor Test action

Github action for running Anchor tests for programs on the Solana blockchain

### Example action

```yaml
name: Anchor Test

on:
  push:
    branches: main

jobs:
  anchor-test:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - name: Anchor Test
        uses: mrgnlabs/anchor-test-action@v0.3
        with:
          args: "" # add anchor test args, e.g. "--skip-lint"
```
