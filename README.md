# actions-update-changelog

This is a composite GitHub Actions for my projects

```yaml
on:
  push:
    branches:
      - main
jobs:
  changelog:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: yykamei/actions-update-changelog@main
        with:
          token: ${{ secrets.GITHUB_TOKEN }}
```
