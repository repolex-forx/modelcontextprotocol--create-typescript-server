# Repolex Knowledge Graph of modelcontextprotocol/create-typescript-server

RDF knowledge graph data for [modelcontextprotocol/create-typescript-server](https://github.com/modelcontextprotocol/create-typescript-server), parsed by [repolex](https://repolex.ai).

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
rlex download modelcontextprotocol/create-typescript-server
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 3115f395cebe7c3ca631ba4becd4cbdf46cd6291
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 3115f395cebe7c3ca631ba4becd4cbdf46cd6291
│           └── chunk-001.nq.gz
├── blob
│   ├── 05c32c6053c1edd9a2faaf1b6ebf565c6650fa28.nq.gz
│   ├── 101a553e656799c8b91184b8e79e06c317ef49ce.nq.gz
│   ├── 1a3d6209588d5e03490ac7530827f2ec523ef44c.nq.gz
│   ├── 1eb244a27ea64e43133e52c2b6d1e79290f028ca.nq.gz
│   ├── 20dd44435c1e15e5b0550b621a3e3445679bc095.nq.gz
│   ├── 2de14405c5f5ca1daef341de6f5b00875841f366.nq.gz
│   ├── 33de0de42a1983f2fa629cd8c17bc0bec6b596dd.nq.gz
│   ├── 4ea40c1cc7fa38ef9053793224f403c19fcd066e.nq.gz
│   ├── 6ebc0c8877a25e19ae0e0e733b28fbfa13f6925a.nq.gz
│   ├── 6ecdb00006d82446d41bc0865c6c321240c8d2b4.nq.gz
│   ├── 73cedd5dffc90de309e1b0e32d7f2c355985ce3c.nq.gz
│   ├── 7f106e9fa41f68c4aa7a600940c640019352af97.nq.gz
│   ├── 87336d26d0d60f34f91e09ddb0699a19faec0572.nq.gz
│   ├── 947a41c52bf44557c31cad76dd7821ad04cf9915.nq.gz
│   ├── a14bee07055b3cd300c82b3a53f4192512349392.nq.gz
│   ├── c679ff384d7e7f313aebf670445ab80b0747c3ac.nq.gz
│   └── e63703d83c2b4bd62d4cd7646857fe9fa17dc796.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 3115f395cebe7c3ca631ba4becd4cbdf46cd6291.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 25 files
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

[modelcontextprotocol/create-typescript-server](https://github.com/modelcontextprotocol/create-typescript-server)

---
*Parsed on 2026-10-09 by [repolex](https://repolex.ai)*
