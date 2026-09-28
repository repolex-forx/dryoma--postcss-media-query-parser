# Repolex Knowledge Graph of dryoma/postcss-media-query-parser

RDF knowledge graph data for [dryoma/postcss-media-query-parser](https://github.com/dryoma/postcss-media-query-parser), parsed by [repolex](https://repolex.ai).

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
rlex download dryoma/postcss-media-query-parser
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── b7a9bf029ea986a5826cf561a5c2295156ed4632
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── b7a9bf029ea986a5826cf561a5c2295156ed4632.nq.gz
│   └── repolex
│       └── b7a9bf029ea986a5826cf561a5c2295156ed4632
│           └── chunk-001.nq.gz
├── blob
│   ├── 0632306a06bc927cbf2f68173e721dfddf9ae49b.nq.gz
│   ├── 323f416ebaec5f208f47518c93cd708f206043b4.nq.gz
│   ├── 36506e954e25a2eea121c20861c7547a8feb425b.nq.gz
│   ├── 3f6dbc847b97f99dcf55c7cd1ea8e3e7fdb7d2e4.nq.gz
│   ├── 4afe455cdf8024def5792bd100dc1fa9ecb4b78d.nq.gz
│   ├── 66e618c05d5919f1510b30b70543c9aab5f7ecf8.nq.gz
│   ├── 763cd11d05768b944effcdb4277c25311d5f6be3.nq.gz
│   ├── b2ae4c34711674c12a05c3e3bdf64f46278e587a.nq.gz
│   ├── c53479aaf5dc8a4f6963052067c1f09508b6d1af.nq.gz
│   ├── d4d7e3f6142fc46cf3168c34008336bfa1607df2.nq.gz
│   └── da4a92c28e1f77f192e33cba00262a2a3468dd90.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── b7a9bf029ea986a5826cf561a5c2295156ed4632.nq.gz
├── filetree
│   └── b7a9bf029ea986a5826cf561a5c2295156ed4632.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

15 directories, 21 files
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

[dryoma/postcss-media-query-parser](https://github.com/dryoma/postcss-media-query-parser)

---
*Parsed on 2026-09-28 by [repolex](https://repolex.ai)*
