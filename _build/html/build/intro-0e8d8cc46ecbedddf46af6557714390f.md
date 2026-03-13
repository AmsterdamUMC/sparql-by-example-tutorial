---
title: "Learning SPARQL By Example"
subtitle: "SWAT4HCLS 2026 Tutorial"
date: 2026-03-23
doi: "10.5281/zenodo.XXXXXXX"

license:
  name: "Creative Commons Attribution 4.0 International"
  short: "CC-BY-4.0"
  url: "https://creativecommons.org/licenses/by/4.0/"

authors:
  - name: "Vincent Emonet"
    affiliations:
      - name: "SIB Swiss Institute of Bioinformatics"
        ror: "https://ror.org/002n09z45"
  - name: "Pauline Lubet"
    affiliations:
      - name: "Amsterdam UMC"
        ror: "https://ror.org/05grdyy37"
  - name: "Tarcisio Mendes"
    affiliations:
      - name: "SIB Swiss Institute of Bioinformatics"
        ror: "https://ror.org/002n09z45"
  - name: "Ana-Claudia Sima"
    affiliations:
      - name: "SIB Swiss Institute of Bioinformatics"
        ror: "https://ror.org/002n09z45"
  - name: "Jerven Bolleman"
    affiliations:
      - name: "SIB Swiss Institute of Bioinformatics"
        ror: "https://ror.org/002n09z45"
  - name: "Andra Waagmeester"
    orcid: "https://orcid.org/0000-0001-9773-4008"
    affiliations:
      - name: "Amsterdam UMC"
        ror: "https://ror.org/05grdyy37"

keywords:
  - SPARQL
  - RDF
  - Linked Data
  - Knowledge Graph
  - Semantic Web
  - Wikidata
  - UniProt
  - FAIR data
  - Life Sciences

abstract: |
  This tutorial teaches SPARQL — the query language for RDF knowledge graphs —
  through practical examples drawn from life sciences datasets. Starting from
  basic triple patterns, you will progress through filtering, aggregation,
  optional patterns, federated queries, and SPARQL Update. All examples use
  publicly accessible SPARQL endpoints including Wikidata, UniProt, and others.
---

# Learning SPARQL By Example

**SPARQL** (SPARQL Protocol and RDF Query Language) is the standard query
language for RDF knowledge graphs. It is to semantic data what SQL is to
relational databases.

This tutorial teaches SPARQL through hands-on examples drawn from publicly
available life sciences endpoints. No local installation is required — all
queries can be run directly in your browser.

## Tutorial structure

The tutorial is organised in three parts:

### Part I — SPARQL Basics

1. **RDF Basics** — A brief refresher on triples, IRIs, literals, and the
   graph data model. Understanding RDF is a prerequisite for writing SPARQL.
2. **Your First Queries** — Write `SELECT` queries using basic triple patterns.
   Learn the `PREFIX`, `SELECT`, `WHERE`, and `LIMIT` keywords.

### Part II — Core SPARQL Features

3. **Filtering** — Use `FILTER`, `REGEX`, `LANG`, and comparison operators
   to narrow down results.
4. **Aggregation** — Group results and compute counts, sums and averages with
   `GROUP BY`, `COUNT`, `SUM`, `AVG`, `MIN`, and `MAX`.
5. **OPTIONAL and UNION** — Handle missing values with `OPTIONAL` and combine
   alternative patterns with `UNION`.

### Part III — Advanced SPARQL

6. **Named Graphs** — Query across multiple named graphs in a dataset using
   `FROM NAMED` and `GRAPH`.
7. **SPARQL Update** — Insert and delete triples with `INSERT DATA`,
   `DELETE DATA`, and `DELETE/INSERT`.
8. **Federated Queries** — Query multiple remote SPARQL endpoints in a single
   query using the `SERVICE` keyword.

## Endpoints used in this tutorial

| Endpoint        | URL                                          | Contents                 |
|-----------------|----------------------------------------------|--------------------------|
| Wikidata        | `https://query.wikidata.org/sparql`          | General knowledge graph  |
| UniProt         | `https://sparql.uniprot.org/sparql`          | Protein sequences & function |
| Bgee            | `https://www.bgee.org/sparql`                | Gene expression data     |
| Idsm            | `https://idsm.elixir-czech.cz/sparql`        | Chemical structures      |

## How to follow along

All SPARQL queries in this tutorial are self-contained and can be pasted
directly into any SPARQL endpoint's query editor. For Wikidata queries, use
the [Wikidata Query Service](https://query.wikidata.org/).

```{tableofcontents}
```
