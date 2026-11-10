# PRAXO-CORE for TypeScript

Dedicated repository for the TypeScript implementation of PRAXO-CORE: an
embeddable, MIT-licensed agent execution kernel with policy controls,
human-in-the-loop approval, checkpoints, events, and tool calling.

- Package: `@axisvela/praxo-core` on npm
- Documentation: https://axisvela.github.io/praxo-core/languages/typescript/
- Consumer starter: https://github.com/axisvela/praxo-core/tree/main/examples/consumer-typescript
- Canonical source: https://github.com/axisvela/praxo-core/tree/main/language/typescript
- Release index: https://axisvela.github.io/praxo-core/languages/registry-status/

This repository is a discovery mirror of the canonical TypeScript source. The
monorepo remains the source of truth and the release workflow source. The
shared conformance vectors are included under `spec/`, so the implementation can
be built and tested here.

## Install

```sh
npm install @axisvela/praxo-core@0.2.2
```

## Verify

From `language/typescript`:

```sh
npm ci
npm test
npm run build
```

## Scope

The TypeScript Core targets the eleven shared vector groups and the agent loop.
It is a native implementation, not a binding over the Go reference. See the
canonical documentation for declared behavior, limitations, and evidence.

PRAXO-CORE is not a hosted model, workflow engine, identity provider, or safety
controller. Do not infer exactly-once execution, complete sandbox isolation,
production security certification, live-provider behavior, or physical safety
from this package.

MIT licensed.
