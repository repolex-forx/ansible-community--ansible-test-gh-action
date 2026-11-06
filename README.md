# Repolex Knowledge Graph of ansible-community/ansible-test-gh-action

RDF knowledge graph data for [ansible-community/ansible-test-gh-action](https://github.com/ansible-community/ansible-test-gh-action), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download ansible-community/ansible-test-gh-action
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── dc5c5bfa02fa4b6633e6175e65e9f8f53088180a
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── dc5c5bfa02fa4b6633e6175e65e9f8f53088180a
│           └── chunk-001.nq.gz
├── blob
│   ├── 0291fa4fa37df22e4a4c5cea87e2236f0de33819.nq.gz
│   ├── 10148d418add81e94ba11b911193d711a8bad437.nq.gz
│   ├── 162afceb142598d6603176e82f1d8ecbbfc06b36.nq.gz
│   ├── 16805ba93821b975b710abd88e78c3d793a478b5.nq.gz
│   ├── 16be8f2193eadbfc2e56f06968aca064a36735a2.nq.gz
│   ├── 20f0efddd89eda21b5c87ee33f2e74595d0cd69f.nq.gz
│   ├── 3b3699f214fb31e98d063314a45e760d7f39cfcd.nq.gz
│   ├── 3cbef9e9f2a4a0e120764dd9767cf87110315fbe.nq.gz
│   ├── 68bf02c49f131e9434b18175116f2a39e2d25059.nq.gz
│   ├── a6dafcf8cd8b039530128f336ff3a42ce1fd5fec.nq.gz
│   ├── ac8aa7fd536668a5aa2122944079959d306e2504.nq.gz
│   ├── b69e158533b28f7447f414b13b42d9d177c45dfd.nq.gz
│   ├── b6e47617de110dea7ca47e087ff1347cc2646eda.nq.gz
│   ├── c9b431a97bdabf010ad05f5194aaadad516416aa.nq.gz
│   ├── f288702d2fa16d3cdf0035b15a9fcbc552cd88e7.nq.gz
│   └── fa3842119ca9884d0e369f19a96c3b35739db533.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── dc5c5bfa02fa4b6633e6175e65e9f8f53088180a.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 24 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[ansible-community/ansible-test-gh-action](https://github.com/ansible-community/ansible-test-gh-action)

---
*Parsed on 2026-11-06 by [repolex](https://repolex.ai)*
