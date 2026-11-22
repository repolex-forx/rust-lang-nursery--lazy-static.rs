# Repolex Knowledge Graph of rust-lang-nursery/lazy-static.rs

RDF knowledge graph data for [rust-lang-nursery/lazy-static.rs](https://github.com/rust-lang-nursery/lazy-static.rs), parsed by [repolex](https://repolex.ai).

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
rlex download rust-lang-nursery/lazy-static.rs
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── be7c1c43f264699f956b70ce8e29941bd1e61bde
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── be7c1c43f264699f956b70ce8e29941bd1e61bde.nq.gz
│   └── repolex
│       └── be7c1c43f264699f956b70ce8e29941bd1e61bde
│           └── chunk-001.nq.gz
├── blob
│   ├── 045ce14b8fa0191495f81fa36fa34dff1523ca9b.nq.gz
│   ├── 16fe87b06e802f094b3fbb0894b137bca2b16ef1.nq.gz
│   ├── 23b8f5eb554eb79063824cd5208a2e464fcdbe83.nq.gz
│   ├── 25597d5838fa4cd7ff5c3c2bb1d1b4c3731eda7f.nq.gz
│   ├── 36d52d347b8d468e896c4ad48e36cfae1c259821.nq.gz
│   ├── 38007d475e4d92e70e14f20ca193638111310d5b.nq.gz
│   ├── 3de0e4b952dd021a4ca32d811c75326ae92373e1.nq.gz
│   ├── 4486f013d3ecdf20962117dc15b6aee53c2580a8.nq.gz
│   ├── 49407ab6a67deffc460041fed631c589ac1ec495.nq.gz
│   ├── 5003fa2c9957d81d484f80b0c3adb68973608f78.nq.gz
│   ├── 5d44f02dcb25626c3e104aa143f9f7b55d30be70.nq.gz
│   ├── 69a9a062288a43be1d60021cf8f777637d4807bb.nq.gz
│   ├── 92b07ab9d431f8a6dcfe849fb076a537ef9e1ae7.nq.gz
│   ├── 93edbe8a6b6f9babc4c7d3a40eac6267945c7529.nq.gz
│   ├── af007cd274b38cb02871a8aa6185a80695c17b87.nq.gz
│   ├── e2f16bcde8509f0020c3ec1dcaf92e9470737f47.nq.gz
│   ├── e3324949a181a8c621c8e0092d69247161688185.nq.gz
│   ├── e5ccb61c17d292b622b30719d145e67c301b589d.nq.gz
│   └── eb659d426d5548288cb1d57c6159934f6004eed7.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── be7c1c43f264699f956b70ce8e29941bd1e61bde.nq.gz
├── filetree
│   └── be7c1c43f264699f956b70ce8e29941bd1e61bde.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

15 directories, 29 files
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

[rust-lang-nursery/lazy-static.rs](https://github.com/rust-lang-nursery/lazy-static.rs)

---
*Parsed on 2026-11-22 by [repolex](https://repolex.ai)*
