<h1 align="center"><span>Switch</span>board</h1>

<p align="center"><b>Open-source, self-hosted feature management with one identical evaluation engine in six languages — proven byte-for-byte in CI.</b></p>

<p align="center">
  <a href="https://github.com/switchboard-io/switchboard/actions/workflows/tests.yml"><img src="https://github.com/switchboard-io/switchboard/actions/workflows/tests.yml/badge.svg" alt="Tests"/></a>
  <a href="https://github.com/switchboard-io/switchboard/blob/main/conformance/RESULTS.md"><img src="https://github.com/switchboard-io/switchboard/actions/workflows/conformance.yml/badge.svg" alt="Conformance"/></a>
  <img src="https://img.shields.io/badge/license-Apache--2.0-blue" alt="License"/>
  <img src="https://img.shields.io/badge/languages-6-3884ff" alt="Six languages"/>
</p>

<p align="center">
  <a href="https://switchboard-io.github.io/switchboard/"><img src="https://raw.githubusercontent.com/switchboard-io/switchboard/main/docs/diagrams/architecture.svg" width="92%" alt="Switchboard architecture — manage once, stream everywhere, evaluate locally, proven identical in CI"/></a>
</p>

---

### What is Switchboard?

Feature flags, targeting, progressive rollouts, kill switches, and experimentation —
**without vendor lock-in**. Every SDK evaluates flags **locally, in-process**, so flag
checks add no network latency and keep working even if the server is unreachable.

The differentiator: **one evaluation engine, six languages, proven identical.** .NET,
JavaScript, Python, Go, Java, and Rust implement the same spec. A shared conformance
corpus runs through all of them on every push and publishes a
**[150/150 pass/fail matrix](https://github.com/switchboard-io/switchboard/blob/main/conformance/RESULTS.md)**
— including *exact* cross-language identity of the SHA1 rollout bucketing, so a user
lands in the same percentage slice no matter which SDK your services use.

### Explore

- 🌐 **[Live site, dashboard & playground](https://switchboard-io.github.io/switchboard/)** — evaluate a flag in your browser with the real engine
- 📦 **[switchboard](https://github.com/switchboard-io/switchboard)** — the monorepo: engine, SDKs, OpenFeature providers, CLI, server, conformance, docs
- ✅ **[Conformance matrix](https://github.com/switchboard-io/switchboard/blob/main/conformance/RESULTS.md)** — six-language proof, refreshed by CI
- 📊 **[Benchmarks](https://github.com/switchboard-io/switchboard/blob/main/docs/BENCHMARKS.md)** — measured evaluation throughput per language

### Install

```bash
dotnet add package Switchboard.Sdk      # .NET
npm install @switchboard/sdk            # JavaScript
pip install switchboard-sdk             # Python
go get github.com/switchboard-io/switchboard-go
cargo add switchboard-sdk               # Rust
```

### Run the server

```bash
docker compose up --build   # Admin UI + REST + live updates at http://localhost:8080
```

<p align="center"><sub>Apache-2.0 · self-hosted · no lock-in · built by <a href="https://parags.dev">Parag Sawant</a> (<a href="https://github.com/paragpsawant">GitHub</a>)</sub></p>
