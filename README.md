## Description

This is a minimal repro for an issue with `tsx` loading re-exported ESM modules.

It happens starting from `tsx` version 4.20.0.

## Reproduction Steps

1. Run `pnpm install` to set up the project.
2. Run `pnpm test:good` to test with `tsx` version 4.19.4 (should work).
3. Run `pnpm test:bad` to test with `tsx` version 4.20.0 (should fail).
