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
      - name: Buck build
        uses: GuilleDF/buckaroo-action@v1.0.1
        with:
          commands: buck build :ext2fs
```
