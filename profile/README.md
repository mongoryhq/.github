# Mongory

**One MongoDB-style query language, native in every runtime.**
Match plain in-memory data (maps, objects, structs, dicts) with `$eq`, `$gte`, `$in`, `$elemMatch`, `$regex` and more — with identical semantics across languages, verified by a shared conformance spec.

👉 **[Try the Playground](https://mongoryhq.github.io/mongory-central/)**

## Packages

| Language | Repo | Install |
|---|---|---|
| Python | [mongory-py](https://github.com/mongoryhq/mongory-py) | `pip install mongory` |
| TypeScript / JS | [mongory-js](https://github.com/mongoryhq/mongory-js) | `npm install mongory-js` |
| Go | [mongory-go](https://github.com/mongoryhq/mongory-go) | `go get github.com/mongoryhq/mongory-go` |
| Ruby | [mongory-rb](https://github.com/mongoryhq/mongory-rb) | `gem install mongory` |
| C99 core | [mongory-core](https://github.com/mongoryhq/mongory-core) | CMake |

## Project

- [mongory-spec](https://github.com/mongoryhq/mongory-spec) — language-agnostic conformance fixtures every implementation must pass
- [mongory-central](https://github.com/mongoryhq/mongory-central) — docs hub & interactive Playground

## Contributing

Issues and PRs are welcome in any repo. Behavior changes start in `mongory-spec`, then flow to each implementation.
