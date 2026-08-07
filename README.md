<div align="center">

  <h1>
    <br />
    ripple-zag
    <br />
    <br />
  </h1>
  <sup>
    Ripple/TSRX adapter for Zag JS state machines
  </sup>
  <br />
  <br />
  <pre>bun add @celados/ripple-zag</pre>
  <br />
</div>

## Install

```bash
bun add @celados/ripple-zag
```

The package is published to `https://npm.celados.com` under the `@celados` scope.
Configure registry authentication before installing it.
This package is not published to npm.

## Usage

```ts
import { useMachine, normalizeProps } from "@celados/ripple-zag"
```

`useMachine` binds a `@zag-js/*` machine to Ripple's reactivity;
`normalizeProps` maps Zag's prop objects onto Ripple/TSRX attributes.

## Peer dependencies

- `ripple ^0.3.118`

## Demo

Component demos live in the [`ripple-explore`](https://github.com/ethan-huo/ripple-explore)
showcase.

## Provenance

Hard fork of [`anubra266/zag-ripple`](https://github.com/anubra266/zag-ripple)
(MIT, © Abraham Aremu). Renamed to `ripple-zag` and maintained independently for
our own Ripple/TSRX projects; it no longer tracks upstream.

## Releasing

See [PUBLISHING.md](./PUBLISHING.md). Bump `package.json#version`, push to
`main`, and CI tags `v${version}`.
