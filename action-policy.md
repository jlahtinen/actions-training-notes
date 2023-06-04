Use https://github.com/EficodeDemoOrg/demo-environments-secrets/edit/main/.github/workflows/demo-secrets-env.yml
to demo that you can restrict the actions you run.

if not already there, create a workflow with the following:

```yaml
name: Mixed actions
on: [workflow_dispatch]
jobs:
  github-action:
    runs-on: ubuntu-latest
    steps:
      - name: checkout
        uses: actions/checkout@v3 # from https://github.com/marketplace/actions/checkout
  verified-action:
    runs-on: ubuntu-latest
    steps:
      - name: install dapr
        uses: dapr/setup-dapr@v1 # from https://github.com/marketplace/actions/dapr-tool-installer
        with:
          version: 1.2.0 # default is 1.2.0
          id: install
  non-verified-action:
    runs-on: ubuntu-latest
    steps:
    - name: Close issues
      uses: mxie/close-outdated-issues-action@main    # from https://github.com/mxie/close-outdated-issues-action/blob/main/README.md
      with:
        token: ${{ secrets.GITHUB_TOKEN }}
        days-before: 30

```

https://github.com/organizations/EficodeDemoOrg/settings/actions
