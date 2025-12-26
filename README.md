## Description

This is a minimal repro for an issue with `tsx` loading ESM modules without `"type": "module"` in their `package.json`.

https://github.com/privatenumber/tsx/issues/761

## Reproduction Steps

1. Run `pnpm install` to set up the project.
2. Run `pnpm test:good` to test with `tsx` version 4.19.4 (should work).
3. Run `pnpm test:bad` to test with `tsx` version 4.20.0 (should fail).
4. Run `pnpm test:node` to test with Node.js directly (should work with node v22.18.0 or later).
