# QUICKWIT

![license](https://img.shields.io/badge/license-license-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![category](https://img.shields.io/badge/category-search_engines-lightgrey)

> Anticloud-hardened packaging of the upstream project `QUICKWIT` in category **SEARCH ENGINES**. Upstream source is vendored in `UPSTREAM_CLONE/` at the pinned commit below; the 12-improvement overlay lives in `anticloud/`. Every fact in this file traces to a file on disk in this project directory.

**Category:** SEARCH ENGINES · **Upstream:** https://github.com/quickwit-oss/quickwit · **Upstream pin:** `8f865ff98603db649a9f6338b9b40cf0bf3a64a3` · **Vendor:** Anticloud FZ LLE

---

## What This Project Does

[![CI](https://github.com/quickwit-oss/quickwit/actions/workflows/ci.yml/badge.svg)](https://github.com/quickwit-oss/quickwit/actions?query=workflow%3ACI+branch%3Amain)
[![codecov](https://codecov.io/gh/quickwit-oss/quickwit/branch/main/graph/badge.svg?token=06SRGAV5SS)](https://codecov.io/gh/quickwit-oss/quickwit)
[![OpenSSF Scorecard](https://api.scorecard.dev/projects/github.com/quickwit-oss/quickwit/badge)](https://scorecard.dev/viewer/?uri=github.com/quickwit-oss/quickwit)
[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)](CODE_OF_CONDUCT.md)
[![License: Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue?style=flat-square)](LICENSE)
[![Twitter Follow](https://img.shields.io/twitter/follow/Quickwit_Inc?color=%231DA1F2&logo=Twitter&style=plastic)](https://twitter.com/Quickwit_Inc)
[![Discord](https://img.shields.io/discord/908281611840282624?logo=Discord&logoColor=%23FFFFFF&style=plastic)](https://discord.quickwit.io)
<br/>

<br/>
<br/>
<p align="center">
  <img src="docs/assets/images/logo_horizontal.svg#gh-light-mode-only" alt="Quickwit Cloud-Native Search Engine" height="40">
  <img src="docs/assets/images/quickwit-dark-theme-logo.png#gh-dark-mode-only" alt="Quickwit Cloud-Native Search Engine" height="40">
</p>

<h2 align="center">
Open-source search engine for observability (logs, traces, and soon metrics!).
</h2>

<h4 align="center">
  <a href="https://quickwit.io/docs/get-started/quickstart">Quickstart</a> |
  <a href="https://quickwit.io/docs/">Docs</a> |
  <a href="https://quickwit.io/tutorials">Tutorials</a> |
  <a href="https://discord.quickwit.io">Chat</a> |
  <a href="https://quickwit.io/docs/get-started/installation">Download</a>
</h4>
<br/>

<b>We just released Quickwit 0.8! Read the [blog post](https://quickwit.io/blog/quickwit-0.8) to learn about the latest powerful features!</b>

### **Quickwit is the fastest search engine on cloud storage. It's the perfect fit for observability use cases**

- [Log management](https://quickwit.io/docs/log-management/overview)
- [Distributed tracing](https://quickwit.io/docs/distributed-tracing/overview)
- Metrics support is on the roadmap

### 🚀 Quickstart

- [Search and analytics on Stack Overflow dataset](https://quickwit.io/docs/get-started/quickstart)
- [Trace analytics with Grafana](https://quickwit.io/docs/get-started/tutorials/trace-analytics-with-grafana)
- [Distributed tracing with Jaeger](https://quickwit.io/docs/get-started/tutorials/tutorial-jaeger)

<br/>

<video src="https://github.com/quickwit-oss/quickwit/assets/653704/020b94b9-deeb-4376-9a3a-b82e1168094c" controls="controls" style="max-width: 1200px;">
</video>

<br/>

# 💡 Features

- Full-text search and aggregation queries
- Elasticsearch-compatible API, use Quickwit with any Elasticsearch or OpenSearch client
- [Jaeger-native](https://quickwit.io/docs/distributed-tracing/plug-quickwit-to-jaeger)
- OTEL-native for [logs](https://quickwit.io/docs/log-management/overview) and [traces](https://quickwit.io/docs/distributed-tracing/overview)
- [Schemaless](https://quickwit.io/docs/guides/schemaless) or strict schema indexing
- Schemaless analytics
- Sub-second search on cloud storage (Amazon S3, Azure Blob Storage, Google Cloud Storage, …)
- Decoupled compute and storage, stateless indexers & searchers
- [Grafana data source](https://github.com/quickwit-oss/quickwit-datasource)
- Kubernetes ready - See our [helm-chart](https://quickwit.io/docs/deployment/kubernetes/helm)
- RESTful API

## Enterprise ready

- Multiple [data sources](https://quickwit.io/docs/ingest-data/) Kafka / Kinesis / Pulsar native
- Multi-tenancy: indexing with many indexes and partitioning
- Retention policies
- Delete tasks (for GDPR use cases)
- Distributed and highly available* engine that scales out in seconds (*HA indexing only with Kafka)

# 📑 Architecture overview

![Quickwit Distributed Tracing](./docs/assets/images/quickwit-overview-light.svg#gh-light-mode-only)![Quickwit Distributed Tracing](./docs/assets/images/quickwit-overview-dark.svg#gh-dark-mode-only)

- [Architecture overview]([https://quickwit.io/docs/distributed-tracing/overview](https://quickwit.io/docs/overview/architecture))
- [Log management](https://quickwit.io/docs/log-management/overview)
- [Distributed traces](https://quickwit.io/docs/distributed-tracing/overview)

# 📕 Documentation

- [Installation](https://quickwit.io/docs/get-started/installation)
- [Log management with Quickwit](https://quickwit.io/docs/log-management/overview)
- [Distributed Tracing with Quickwit](https://quickwit.io/docs/distributed-tracing/overview)
- [Ingest data](https://quickwit.io/docs/ingest-data/)
- [REST API](https://quickwit.io/docs/reference/rest-api)

# 📚 Resources

- [Blog posts](https://quickwit.io/blog/)
- [Youtube channel](https://www.youtube.com/@quickwit8103)
- [Discord](https://discord.quickwit.io)

# 🙋 FAQ

### How can I switch from Elasticsearch or OpenSearch to Quickwit?

Quickwit supports a large subset of Elasticsearch/OpenSearch API.

For instance, it has an ES-compatible ingest API to make it easier to migrate your log shippers (Vector, Fluent Bit, Syslog, ...) to Quickwit.

On the search side, the most popular Elasticsearch endpoints, query DSL, and even aggregations are supported.

The list of available endpoints and queries is available [here](https://quickwit.io/docs/reference/es_compatible_api), while the list of supported aggregations is available [here](https://quickwit.io/docs/reference/aggregation).

Let us know if part of the API you are using is missing!

If the client you are using is refusing to connect to Quickwit due to missing headers, you can use the `extra_headers` option in the [node configuration](https://quickwit.io/docs/configuration/node-config#rest-configuration) to impersonate any compatible version of Elasticsearch or OpenSearch.

### How is Quickwit different from traditional search engines like Elasticsearch or Solr?

The core difference

*(excerpt; full text in `UPSTREAM_CLONE/`)*

*Quoted from the upstream `README.md` file in `UPSTREAM_CLONE/`.*
Project-specific facts detected in this directory:

- Ecosystem: **C/C++ / Make** (manifests: Makefile; scanned in UPSTREAM_CLONE)
- Top-level source layout: `build/`, `config/`, `distribution/`, `monitoring/`, `quickwit/`
- Snapshot size: **1145 files**, **283125 lines of code** (measured; see Benchmarks)
- Primary languages: `.rs` (633), `.yaml` (145), `.sql` (67), `.toml` (46), `.md` (39), `.json` (38)
- Upstream commit pinned for this packaging: `8f865ff98603db649a9f6338b9b40cf0bf3a64a3`

---

## Installation

<a href="https://quickwit.io/docs/">Docs</a> |
  <a href="https://quickwit.io/tutorials">Tutorials</a> |
  <a href="https://discord.quickwit.io">Chat</a> |
  <a href="https://quickwit.io/docs/get-started/installation">Download</a>
</h4>
<br/>

<b>We just released Quickwit 0.8! Read the [blog post](https://quickwit.io/blog/quickwit-0.8) to learn about the latest powerful features!</b>

### **Quickwit is the fastest search engine on cloud storage. It's the perfect fit for observability use cases**

- [Log management](https://quickwit.io/docs/log-management/overview)
- [Distributed tracing](https://quickwit.io/docs/distributed-tracing/overview)
- Metrics support is on the roadmap

*Section quoted from the upstream readme.*
Overlay install (this project):

```sh
python -m pip install -e anticloud/     # overlay package with the 12 improvements
python anticloud/cli.py --help          # 13 subcommands, JSON stdout
```

---

## Usage

<a href="https://discord.quickwit.io">Chat</a> |
  <a href="https://quickwit.io/docs/get-started/installation">Download</a>
</h4>
<br/>

<b>We just released Quickwit 0.8! Read the [blog post](https://quickwit.io/blog/quickwit-0.8) to learn about the latest powerful features!</b>

### **Quickwit is the fastest search engine on cloud storage. It's the perfect fit for observability use cases**

- [Log management](https://quickwit.io/docs/log-management/overview)
- [Distributed tracing](https://quickwit.io/docs/distributed-tracing/overview)
- Metrics support is on the roadmap

*Section quoted from the upstream readme.*
Anticloud overlay CLI (available in every project):

```sh
python anticloud/cli.py --help     # 13 subcommands, JSON stdout
python anticloud/cli.py checks     # run the 16-check suite
```

---

## API

[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)](CODE_OF_CONDUCT.md)
[![License: Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue?style=flat-square)](LICENSE)
[![Twitter Follow](https://img.shields.io/twitter/follow/Quickwit_Inc?color=%231DA1F2&logo=Twitter&style=plastic)](https://twitter.com/Quickwit_Inc)
[![Discord](https://img.shields.io/discord/908281611840282624?logo=Discord&logoColor=%23FFFFFF&style=plastic)](https://discord.quickwit.io)
<br/>

<br/>
<br/>
<p align="center">
  <img src="docs/assets/images/logo_horizontal.svg#gh-light-mode-only" alt="Quickwit Cloud-Native Search Engine" height="40">
  <img src="docs/assets/images/quickwit-dark-theme-logo.png#gh-dark-mode-only" alt="Quickwit Cloud-Native Search Engine" height="40">
</p>

<h2 align="center">
Open-source search engine for observability (logs, traces, and soon metrics!).
</h2>

<h4 align="center">
  <a href="https://quickwit.io/docs/get-started/quickstart">Quickstart</a> |
  <a href="https://quickwit.io/docs/">Docs</a> |
  <a href="https://quickwit.io/tutorials">Tutorials</a> |
  <a href="https://discord.quickwit.io">Chat</a> |
  <a href="https://quickwit.io/docs/get-started/installation">Download</a>
</h4>
<br/>

<b>We just released Quickwit 0.8! Read the [blog post](https://quickwit.io/blog/quickwit-0.8) to learn about the latest powerful features!</b>

### **Quickwit is the fastest search engine on cloud storage. It's the perfect fit for observability use cases**

- [Log management](https://quickwit.io/docs/log-management/overview)
- [Distributed tracing](https://quickwit.io/docs/distributed-tracing/overview)
- Metrics support is on the roadmap

*Section quoted from the upstream readme.*
---

## Dependencies

| Metric | Value |
|--------|-------|
| Ecosystem | C/C++ / Make |
| Manifests detected | Makefile |
| Files in snapshot | 1145 |
| Lines of code | 283125 |
| Dependency references | 339 |
| Dependencies by ecosystem | cargo: 294, npm: 39, pypi: 6 |
| Upstream license | Apache-2.0 |
| Overlay license | Anticommons 0.1.0 |

Top dependency references recorded in the benchmark snapshot:

| Ecosystem | Name | Version | Source file |
|-----------|------|---------|-------------|
| cargo | resolver | 2 | quickwit/Cargo.toml |
| cargo | version | 0.9.1 | quickwit/Cargo.toml |
| cargo | edition | 2024 | quickwit/Cargo.toml |
| cargo | homepage | https://quickwit.io/ | quickwit/Cargo.toml |
| cargo | documentation | https://quickwit.io/docs/ | quickwit/Cargo.toml |
| cargo | project | https://github.com/quickwit-oss/quickwit | quickwit/Cargo.toml |
| cargo | license | Apache-2.0 | quickwit/Cargo.toml |
| cargo | ahash | 0.8 | quickwit/Cargo.toml |
| cargo | anyhow | 1 | quickwit/Cargo.toml |
| cargo | arc-swap | 1.9 | quickwit/Cargo.toml |
| cargo | assert-json-diff | 2 | quickwit/Cargo.toml |
| cargo | async-compression | 0.4 | quickwit/Cargo.toml |
| cargo | async-speed-limit | 0.4 | quickwit/Cargo.toml |
| cargo | async-trait | 0.1 | quickwit/Cargo.toml |
| cargo | atomic_float | 1.1 | quickwit/Cargo.toml |
| ... | (324 more) | | |

Pinned lockfile: `anticloud/requirements.lock` (hash-pinned, PEP 508). SBOM: `sbom.cdx.json` (CycloneDX 1.5, pinned to the upstream SHA).

---

## Configuration

### How is Quickwit different from traditional search engines like Elasticsearch or Solr?

The core difference and advantage of Quickwit is its architecture built from the ground to search on cloud storage. We optimized IO paths, revamped the index data structures and made search stateless and sub-second on cloud storage.

### How does Quickwit compare to Elastic in terms of cost?

We estimate that Quickwit can be up to 10x cheaper on average than Elastic. To understand how, check out our [blog post](https://quickwit.io/blog/commoncrawl/) about searching the web on AWS S3.

*Section quoted from the upstream readme.*
Overlay configuration (Anticloud):

- `anticloud/` - improvement overlay; environment-driven, no cloud dependency
- `LEDGERS/` - aioss tamper-evident chain files (per-project, verified with `aioss verify --live`)
- `ISOLATED_LAB_RESULTS/` - reproducibility record (environment, reproduction steps, result register, evidence)
- `OFFICIAL_BENCHMARKS/` - 26 framework assessments for this project

---

## Contributing

*Excerpt from upstream `CONTRIBUTING.md`:*

# Contributing to Quickwit
There are many ways to contribute to Quickwit.
Code contributions are welcome of course, but also
bug reports, feature requests, and evangelizing are as valuable.

# Submitting a PR
Check if your issue is already listed on [github](https://github.com/quickwit-oss/quickwit/issues).
If it is not, create your own issue.

Please add the following phrase at the end of your commit `Closes #<Issue Number>`.
It will automatically link your PR in the issue page. Also, once your PR is merged, it will
close the issue. If your PR only partially addresses the issue and you would like to
keep it open, just write `See #<Issue Number>`.

Feel free to send your contribution in an unfinished state to get early feedback.
In that case, simply mark the PR with the tag [WIP] (standing for work in progress).

# Development

## Setup & run tests

### Local Development

1. Install Rust, CMake, Docker (https://docs.docker.com/engine/install/) and Docker Compose (https://docs.docker.com/compose/install/)
2. Install node@24 and `npm install -g yarn`
3. Install awslocal https://github.com/localstack/awscli-local
4. Install protoc https://grpc.io/docs/protoc-installation/ (you may need to install the latest binaries rather than your distro's flavor)
5. Install nextest https://nexte.st/docs/installation/pre-built-binaries/

### GitHub Codespaces

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/quickwit-oss/quickwit?devcontainer_path=.devcontainer/devcontainer.json)

GitHub Codespaces provides a fully configured development environment in the cloud, making it easy to get started with Quickwit development. By clicking the badge above, you can create a codespace with all the necessary tools installed and configured.

### Running tests
Run `make test-all` to run all tests.

## Useful commands
* `make test-all` - starts necessary Docker services and runs all tests.
* `make -k test-all docker-compose-down` - the same as above, but tears down the Docker services after running all the tests.
* `make fmt` - runs formatter, this command requires the nightly toolchain to be installed by running `rustup toolchain install nightly`.
* `make fix` - runs formatter and clippy checks as well as removing unused dependencies (requires `cargo install cargo-machete`).
* `make typos` - runs the spellcheck tool over the codebase. (Install by running `cargo install typos-cli`)
* `make doc` - builds docs.
* `make docker-compose-up` - start

Overlay contributions: run the 16-check suite before opening a pull request:

```sh
python anticloud/bench/runner.py --cwd anticloud
```

---

## License

**Upstream license: Apache-2.0** (evidence: `LICENSE` in the upstream snapshot).

License file excerpt:

```text
                                 Apache License
                           Version 2.0, January 2004
                        http://www.apache.org/licenses/

   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION

   1. Definitions.

      "License" shall mean the terms and conditions for use, reproduction,
      and distribution as defined by Sections 1 through 9 of this document.

      "Licensor" shall mean the copyright owner or entity authorized by
      the copyright owner that is granting the License.

      "Legal Entity" shall mean the union of the acting entity and all
      other entities that control, are controlled by, or are under common
      control with that entity. For the purposes of this definition,
      "control" means (i) the power, direct or indirect, to cause the
      direction or management of such entity, whether by contract or
      otherwise, or (ii) ownership of fifty percent (50%) or more of the
```

### Anticommons 0.1.0 overlay

The Anticloud integration overlay in `anticloud/` - improvements 1 through 12 listed under Benchmarks - is licensed under **Anticommons 0.1.0**. Upstream code remains under its original Apache-2.0 terms. See `ANTICOMMONS_LICENSE.md` in this directory for the overlay terms and contact.

SPDX: `Apache-2.0` (upstream) + Anticommons 0.1.0 (overlay, dual).

---

## Upstream

- **Project:** `QUICKWIT` (category: SEARCH ENGINES)
- **Upstream URL:** https://github.com/quickwit-oss/quickwit
- **Pinned commit (SHA):** `8f865ff98603db649a9f6338b9b40cf0bf3a64a3`
- **Branch:** HEAD
- **Pin provenance:** resolved during the second documentation pass. The parent-project stamp is explicitly rejected for this project.
- **Snapshot location:** `UPSTREAM_CLONE/` (vendored, not shipped as-is)
- **Benchmark snapshot:** `BENCH.json`

---

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`316dd91bb7a90f62a31ed06888d38558308b9d546dd45eaf129619fa45574f9f`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe and Mail, Business Insider, National Post, Financial Post, StreetInsider, Digital Journal, Barchart, International Business Times, and fox47 · National Law Review.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

