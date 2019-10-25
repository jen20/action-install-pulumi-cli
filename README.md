# Install `pulumi` CLI Action

This repository contains an action for use with GitHub Actions, which installs a specified version of  the `pulumi` CLI.

`pulumi` is installed into `/home/runner/.pulumi` (or equivalent on Windows) and the `bin` subdirectory is added to the PATH.

## Usage

Install the latest version of the Pulumi CLI:

```yaml
- name: Install Pulumi CLI
  uses: jen20/action-install-pulumi-cli@releases/v1
```

Install a specific version of the Pulumi CLI:

```yaml
- name: Install pulumi
  uses: jen20/action-install-pulumi-cli@releases/v1
  with:
    pulumi-version: 1.4.0
```
