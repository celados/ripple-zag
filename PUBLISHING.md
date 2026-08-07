---
type: Playbook
title: Publish ripple-zag
description: Release @celados/ripple-zag through GitHub and npm.celados.com.
when: Changing the package version, artifact, registry authentication, or release workflow.
---

# Publishing

`package.json#version` is the release source of truth. A published GitHub
Release whose tag is exactly `v${version}` triggers
[the publish workflow](./.github/workflows/release.yml).

## Contract

- Package: `@celados/ripple-zag`
- Registry: `https://npm.celados.com`
- Local authentication: activate `publish-package-celados`, copy its auth
  template to `.npmrc.tpl`, then render it; both local files stay ignored
- CI authentication: the `NPM_TOKEN` Actions secret becomes `NODE_AUTH_TOKEN`
- Artifact: `dist/`, `src/`, `README.md`, `LICENSE`, and package metadata

The workflow performs a frozen install, typecheck, tests, artifact dry-run,
publish, and an exact-version install/import from a clean consumer.

## Release

1. Update `package.json#version` and `CHANGELOG.md`.
2. Run the local gates and inspect the packed artifact.
3. Commit and push `main`.
4. Publish a GitHub Release named after the matching `v${version}` tag.
5. Wait for the publish workflow and verify the exact registry version.
