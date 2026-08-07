# ripple-zag

## 0.4.1

### Patch Changes

- Type normalized generic element props as Ripple intrinsic element attributes
  instead of `<head>` attributes, fixing invalid `ref` types on connected APIs.

## 0.4.0

### Breaking Changes

- Remove the `mergeProps` re-export. It had no Ripple-specific behavior and
  forced the adapter to mirror an upstream utility API that consumers can
  import directly from `@zag-js/core` when they actually need it.

## 0.3.0

### Minor Changes

- Publish as `@celados/ripple-zag` through `npm.celados.com`.
- Update Ripple to 0.3.118 and Zag dependencies to 1.43.0.
- Cover Zag's composed `data-ownedby` merge behavior and fix tracked-value typechecking.

## 0.1.4

### Patch Changes

- [`732890e`](https://github.com/anubra266/zag-ripple/commit/732890ead872308cfd6943871443e7c12e219b27) Thanks [@anubra266](https://github.com/anubra266)! - Use core mergeprops

## 0.1.3

### Patch Changes

- [`e6fd1bc`](https://github.com/anubra266/zag-ripple/commit/e6fd1bc5da35fb983bf00469f60be890dd6a14d2) Thanks [@anubra266](https://github.com/anubra266)! - Enhance createBindable function to support synchronous updates with flushSync

## 0.1.2

### Patch Changes

- [`867e85f`](https://github.com/anubra266/zag-ripple/commit/867e85f68cc40d2164d6e2c751b5b82495f209f2) Thanks [@anubra266](https://github.com/anubra266)! - Export proptypes

## 0.1.1

### Patch Changes

- [`267f463`](https://github.com/anubra266/zag-ripple/commit/267f46317a05a21e8f2a65fd5abc68c209f09ce0) Thanks [@anubra266](https://github.com/anubra266)! - Bump

## 0.1.0

### Minor Changes

- [`512be14`](https://github.com/anubra266/zag-ripple/commit/512be1477c4c348d8ca40cdc12ff782f3a3adb2f) Thanks [@anubra266](https://github.com/anubra266)! - Minor bump

### Patch Changes

- [`dfeb166`](https://github.com/anubra266/zag-ripple/commit/dfeb166180b28c6d7f790a205f326057e3e4e7da) Thanks [@anubra266](https://github.com/anubra266)! - bump

## 0.0.18

### Patch Changes

- [`6430e51`](https://github.com/anubra266/zag-ripple/commit/6430e51190274607ad6978e92cc53e634fcf19b3) Thanks [@anubra266](https://github.com/anubra266)! - Port to TS
