<p align="center">
  <img src="https://mongoryhq.github.io/mongory-central/mongoryhq-icon.png" alt="Mongory" width="88" />
</p>

# Mongory

**One MongoDB-style query & rule language, native in every runtime — with built-in Explain & Trace debugging.**

Compile JSON/MongoDB-style conditions (`$eq`, `$gte`, `$in`, `$elemMatch`, `$every`, `$present`, `$regex`, ...) once and evaluate plain in-memory data (maps, structs, objects, dicts, arrays) with **identical semantics across 5 languages**, verified by a shared conformance spec.

👉 **[Try the Interactive Playground & Visual Trace Debugger ↗](https://mongoryhq.github.io/mongory-central/)**

## Packages

| Language | Repo | Version | Install | Engine |
|---|---|---|---|---|
| **TypeScript / JS** | [mongory-js](https://github.com/mongoryhq/mongory-js) | `v0.2.0` | `npm install mongory-js` | Pure TS (0 deps, ESM + CJS) |
| **Go** | [mongory-go](https://github.com/mongoryhq/mongory-go) | `v0.4.0` | `go get github.com/mongoryhq/mongory-go` | Pure Go (0 deps, 0 allocs/op hot-path) |
| **Python** | [mongory-py](https://github.com/mongoryhq/mongory-py) | `v0.2.1` | `pip install mongory` | CPython C-API over `mongory-core` |
| **Ruby** | [mongory-rb](https://github.com/mongoryhq/mongory-rb) | `v2.1.1` | `gem install mongory` | Native C99 ext (`mongory-core`, Ruby 2.6–4.0) |
| **C99 Core** | [mongory-core](https://github.com/mongoryhq/mongory-core) | `v0.3.1` | CMake / `pkg-config` | Portable C99 arena pool + opt-in `yyjson` |

## Why Mongory?

| Capability | Mongory | CEL / OPA Rego | JSONLogic | `sift` / `mingo` |
|---|---|---|---|---|
| **Syntax** | Familiar MongoDB JSON query syntax | Custom expression / policy DSL | Custom JSON AST | MongoDB query syntax |
| **Cross-language parity** | 5 languages locked to [`mongory-spec`](https://github.com/mongoryhq/mongory-spec) | Separate runtimes / heavy SDKs | Community ports vary in edge cases | JS/TS only |
| **Visual debugging** | Built-in cost-sorted `explain` & short-circuit `trace` trees | Limited / external | None | None |
| **Performance & footprint** | Zero-alloc Go hot-path, C99 arena core, 0-dep TS | Heavy parser/VM | Interpreted | Slower on large `$in` |

## Project

- [mongory-spec](https://github.com/mongoryhq/mongory-spec) — language-agnostic conformance fixtures every implementation must pass
- [mongory-central](https://github.com/mongoryhq/mongory-central) — docs hub & interactive Playground

## Contributing

Issues and PRs are welcome in any repo. Behavior changes start in `mongory-spec`, then flow to each implementation.
