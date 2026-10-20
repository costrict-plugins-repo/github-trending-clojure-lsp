# clojure-lsp plugin for Claude Code

Clojure/ClojureScript language server plugin for [Claude Code](https://claude.com/claude-code), providing code intelligence, navigation, and refactoring via [clojure-lsp](https://clojure-lsp.io/).

## Supported file types

| Extension | Language |
|-----------|----------|
| `.clj` | Clojure |
| `.cljs` | ClojureScript |
| `.cljc` | Clojure (common) |
| `.edn` | EDN |

## Prerequisites

Install the `clojure-lsp` binary before using this plugin.

**macOS (Homebrew):**
```bash
brew install clojure-lsp/brew/clojure-lsp-native
```

**Nix:**
```bash
nix-env -i clojure-lsp
```

**Other platforms:** download from the [clojure-lsp releases](https://github.com/clojure-lsp/clojure-lsp/releases).

## Installation

```bash
claude plugin install clojure-lsp
```

## LSP capabilities

Once installed, Claude Code gains access to these operations on Clojure files:

- `goToDefinition` — jump to where a symbol is defined
- `findReferences` — find all usages of a symbol
- `hover` — get documentation and type info
- `documentSymbol` — list all symbols in a file
- `workspaceSymbol` — search for symbols across the project
- `goToImplementation` — find implementations of a protocol/multimethod

## License

Apache 2.0
