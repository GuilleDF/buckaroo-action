# buckaroo-action

Use buck and buckaroo in your github CI

```yaml
name: CI

on: [push]

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - uses: actions/checkout@v1
      - uses: GuilleDF/buckaroo-action@v1.0.0
      - name: Build
        run: buck build :ext2fs

```
