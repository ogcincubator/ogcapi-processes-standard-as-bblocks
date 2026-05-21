# OGC API - Processes - Part 1 (Standard as Building Blocks)

OGC API — Processes Part 1: Core, authored as Building Blocks. This is a proof-of-concept
demonstrating the "OGC Standards as BBs" methodology, where the standards document is generated
from a set of Building Blocks rather than from AsciiDoc source.


This repository contains the Building Blocks for OGC API — Processes Part 1: Core (OGC 18-062r3).
It demonstrates the [OGC Standards as BBs](https://github.com/opengeospatial/ogcapi-processes/blob/master/docs/ogc-standards-as-bblocks.md)
proposal, where normative requirements, conformance tests, schemas, and prose are all co-located
in a Building Block, and the standards document is generated from the BB set.

New BB types introduced: `requirements-class`, `clause`, `terms`, `references`.
New `bblock.json` fields: `clause-index`, `normative`, `standardization-target`.


## Building Blocks

### `ogc.api.processes.part1.clauses.conventions` — Conventions

**Type:** clause

Conventions used throughout OGC API — Processes Part 1: Core.

### `ogc.api.processes.part1.clauses.references` — Normative References

**Type:** references

Normative references for OGC API — Processes Part 1: Core.

### `ogc.api.processes.part1.clauses.scope` — Scope

**Type:** clause

Scope clause for OGC API — Processes Part 1: Core.

### `ogc.api.processes.part1.clauses.terms` — Terms and Definitions

**Type:** terms

Terms, definitions and abbreviated terms for OGC API — Processes Part 1: Core.

### `ogc.api.processes.part1.requirements.core` — Core

**Type:** requirements-class

Core requirements class for OGC API — Processes Part 1. Specifies the fundamental operations a server must support: landing page, conformance declaration, process list, process description, process execution, job status, and job results.

### `ogc.api.processes.part1.requirements.json` — JSON

**Type:** requirements-class

Requirements class for JSON encoding. Requires that all supported API endpoints respond with application/json when requested.

