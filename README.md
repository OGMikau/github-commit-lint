# github-commit-lint
Checks to see if commit messages meet standards

## Example

```yaml
name: Generate
jobs:
  generate:
    steps:
      - uses: actions/checkout@v3
      - name: 'Commit Lint'
        uses: "OGMikau/github-commit-lint@main"
        with:
          message: "${{github.event.head_commit.message}}"
