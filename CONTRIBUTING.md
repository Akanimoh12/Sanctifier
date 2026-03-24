# Contributing to Sanctifier

Thanks for helping improve Sanctifier.

## Required repository secrets

### `CRATES_IO_TOKEN`

The release workflow publishes both `sanctifier-core` and `sanctifier-cli`
when a version tag such as `v0.1.0` is pushed.

To configure the token:

1. Open the Sanctifier repository on GitHub.
2. Go to `Settings` -> `Secrets and variables` -> `Actions`.
3. Create a new repository secret named `CRATES_IO_TOKEN`.
4. Generate the token from your [crates.io account settings](https://crates.io/settings/tokens).

The workflow publishes `sanctifier-core` first and then `sanctifier-cli`,
because the CLI depends on the core crate.
