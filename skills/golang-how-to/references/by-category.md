# Golang skills — full catalog by category

30 skills. Skills marked ⭐️ are recommended for all Go projects. Skills marked ⚙️ can be superseded by a company-specific skill.

---

## Table of Contents

- [Code Quality](#code-quality)
  - [`samber/cc-skills-golang@golang-code-style` ⭐️ ⚙️](#sambercc-skills-golanggolang-code-style-%EF%B8%8F-%EF%B8%8F)
  - [`samber/cc-skills-golang@golang-documentation` ⭐️ ⚙️](#sambercc-skills-golanggolang-documentation-%EF%B8%8F-%EF%B8%8F)
  - [`samber/cc-skills-golang@golang-error-handling` ⭐️ ⚙️](#sambercc-skills-golanggolang-error-handling-%EF%B8%8F-%EF%B8%8F)
  - [`samber/cc-skills-golang@golang-lint`](#sambercc-skills-golanggolang-lint)
  - [`samber/cc-skills-golang@golang-naming` ⭐️ ⚙️](#sambercc-skills-golanggolang-naming-%EF%B8%8F-%EF%B8%8F)
  - [`samber/cc-skills-golang@golang-safety` ⭐️](#sambercc-skills-golanggolang-safety-%EF%B8%8F)
  - [`samber/cc-skills-golang@golang-security` ⭐️ 🧠](#sambercc-skills-golanggolang-security-%EF%B8%8F-)
  - [`samber/cc-skills-golang@golang-structs-interfaces` ⚙️](#sambercc-skills-golanggolang-structs-interfaces-%EF%B8%8F)
- [Architecture & Design](#architecture--design)
  - [`samber/cc-skills-golang@golang-concurrency` ⚙️](#sambercc-skills-golanggolang-concurrency-%EF%B8%8F)
  - [`samber/cc-skills-golang@golang-context` ⚙️](#sambercc-skills-golanggolang-context-%EF%B8%8F)
  - [`samber/cc-skills-golang@golang-data-structures` ⭐️](#sambercc-skills-golanggolang-data-structures-%EF%B8%8F)
  - [`samber/cc-skills-golang@golang-database` ⭐️ ⚙️](#sambercc-skills-golanggolang-database-%EF%B8%8F-%EF%B8%8F)
  - [`samber/cc-skills-golang@golang-dependency-injection` ⚙️](#sambercc-skills-golanggolang-dependency-injection-%EF%B8%8F)
  - [`samber/cc-skills-golang@golang-design-patterns` ⭐️ ⚙️](#sambercc-skills-golanggolang-design-patterns-%EF%B8%8F-%EF%B8%8F)
  - [`samber/cc-skills-golang@golang-modernize` ⭐️](#sambercc-skills-golanggolang-modernize-%EF%B8%8F)
  - [`samber/cc-skills-golang@golang-refactoring` ⭐️ 🧠 ⚙️](#sambercc-skills-golanggolang-refactoring-%EF%B8%8F--%EF%B8%8F)
- [QA & Performance](#qa--performance)
  - [`samber/cc-skills-golang@golang-benchmark` 🧠](#sambercc-skills-golanggolang-benchmark-)
  - [`samber/cc-skills-golang@golang-observability` ⚙️](#sambercc-skills-golanggolang-observability-%EF%B8%8F)
  - [`samber/cc-skills-golang@golang-performance` 🧠](#sambercc-skills-golanggolang-performance-)
  - [`samber/cc-skills-golang@golang-testing` ⭐️ 🧠 ⚙️](#sambercc-skills-golanggolang-testing-%EF%B8%8F--%EF%B8%8F)
  - [`samber/cc-skills-golang@golang-troubleshooting` ⭐️ 🧠](#sambercc-skills-golanggolang-troubleshooting-%EF%B8%8F-)
- [Project Setup](#project-setup)
  - [`samber/cc-skills-golang@golang-cli`](#sambercc-skills-golanggolang-cli)
  - [`samber/cc-skills-golang@golang-continuous-integration`](#sambercc-skills-golanggolang-continuous-integration)
  - [`samber/cc-skills-golang@golang-dependency-management`](#sambercc-skills-golanggolang-dependency-management)
  - [`samber/cc-skills-golang@golang-gopls`](#sambercc-skills-golanggolang-gopls)
  - [`samber/cc-skills-golang@golang-how-to` ⭐️](#sambercc-skills-golanggolang-how-to-%EF%B8%8F)
  - [`samber/cc-skills-golang@golang-pkg-go-dev`](#sambercc-skills-golanggolang-pkg-go-dev)
  - [`samber/cc-skills-golang@golang-popular-libraries`](#sambercc-skills-golanggolang-popular-libraries)
  - [`samber/cc-skills-golang@golang-project-layout`](#sambercc-skills-golanggolang-project-layout)
  - [`samber/cc-skills-golang@golang-stay-updated`](#sambercc-skills-golanggolang-stay-updated)

## Code Quality

### `samber/cc-skills-golang@golang-code-style` ⭐️ ⚙️

Golang code formatting, conventions, and project-level style consistency — gofmt, goimports, line length, var declarations, blank lines, comment heuristics.

Use when: the user asks about formatting rules, style review, or project coding standards. Not for naming conventions (→ `golang-naming`), linter configuration (→ `golang-lint`), or doc comments (→ `golang-documentation`).

---

### `samber/cc-skills-golang@golang-documentation` ⭐️ ⚙️

Golang documentation standards — package docs, godoc conventions, example functions, README structure, CHANGELOG, llms.txt, API reference generation.

Use when: writing or reviewing Go doc comments, README files, or API reference. Not for code comments that explain logic (→ `golang-code-style`).

---

### `samber/cc-skills-golang@golang-error-handling` ⭐️ ⚙️

Golang error handling best practices — error creation, wrapping with fmt.Errorf and errors.Is/As, sentinel errors, custom error types, panic recovery, and structured error context with `github.com/samber/oops`.

Use when: writing or reviewing error propagation, wrapping, logging, structured error context, or recovery patterns. For preventing panics → `golang-safety`; for production logging pipelines → `golang-observability`.

---

### `samber/cc-skills-golang@golang-lint`

Golang linting — golangci-lint configuration, presets, custom rules, CI integration, nolint suppressions, linter selection and output interpretation.

Use when: setting up or tuning golangci-lint, interpreting lint failures, or deciding which linters to enable. For style conventions not enforced by linters → `golang-code-style`.

---

### `samber/cc-skills-golang@golang-naming` ⭐️ ⚙️

Golang naming conventions across all identifier types — packages, constructors, structs, interfaces, constants, errors, receivers, acronyms, test functions. Covers MixedCaps rules, Get-prefix, and utils/helpers anti-patterns.

Use when: naming a new type, function, package, or constant. Not for broader formatting (→ `golang-code-style`).

---

### `samber/cc-skills-golang@golang-safety` ⭐️

Defensive Golang coding — prevents panics, silent data corruption, and runtime bugs. Nil safety, append aliasing, map concurrent access, float comparison, zero-value design, numeric overflow.

Use when: writing or reviewing code that could silently produce wrong results or panic. Not for external threats (→ `golang-security`) or error handling idioms (→ `golang-error-handling`).

---

### `samber/cc-skills-golang@golang-security` ⭐️ 🧠

Golang security best practices — injection prevention (SQL, command, XSS), cryptography, filesystem/network safety, secrets management, cookie security, tool configuration. Audit and review modes.

Use when: auditing a codebase for vulnerabilities, writing security-sensitive code, or reviewing auth/crypto/secrets handling. Not for runtime correctness bugs (→ `golang-safety`).

---

### `samber/cc-skills-golang@golang-structs-interfaces` ⚙️

Golang struct and interface design — composition, embedding, type assertions, interface segregation, struct tags (JSON/YAML/DB), pointer vs value receivers.

Use when: designing types, choosing between value vs pointer receivers, writing struct tags, or working with interface hierarchies. For architectural patterns that use interfaces → `golang-design-patterns`.

---

## Architecture & Design

### `samber/cc-skills-golang@golang-concurrency` ⚙️

Golang concurrency patterns — goroutines, channels, sync primitives, context cancellation, worker pools, fan-out/fan-in, pipelines, errgroup.

Use when: writing concurrent code, coordinating goroutines, or reviewing for race conditions. For context propagation specifically → `golang-context`. When cancelling goroutines via context — load both.

---

### `samber/cc-skills-golang@golang-context` ⚙️

Idiomatic context.Context usage — creation, cancellation, timeouts, values, propagation patterns, WithoutCancel, common anti-patterns.

Use when: propagating deadlines and cancellation signals, or passing request-scoped values. Not for code that merely accepts ctx as first parameter.

---

### `samber/cc-skills-golang@golang-data-structures` ⭐️

Golang data structures internals and usage — slices (capacity growth, append aliasing), maps, channels, sync primitives, container/\*, generic collections, and when to use each.

Use when: choosing a data structure, understanding slice/map performance characteristics, or using container/list, container/heap, or ring.

---

### `samber/cc-skills-golang@golang-database` ⭐️ ⚙️

Golang database access patterns — parameter binding, connection pooling, transactions, migrations, sqlboiler/sqlc code generation, query builders.

Use when: writing SQL queries, designing repository patterns, or configuring database connections. For security aspects of queries (injection) → also consult `golang-security`.

---

### `samber/cc-skills-golang@golang-dependency-injection` ⚙️

Dependency injection patterns in Golang — constructor injection, interface-based DI, `uber-go/dig`, `uber-go/fx`, and `samber/do` comparison, and when DI is worth the complexity.

Use when: deciding whether to use DI, designing constructor signatures, comparing or wiring `go.uber.org/dig`, `go.uber.org/fx`, or `github.com/samber/do`, or refactoring away from globals. For package API lookup → `golang-pkg-go-dev`.

---

### `samber/cc-skills-golang@golang-design-patterns` ⭐️ ⚙️

Idiomatic Golang design patterns — functional options, constructors, builder pattern, middleware chains, circuit breaker, and architecture guides.

Use when: choosing architectural patterns, designing APIs, or implementing resilience patterns. For type-level design (embedding, receivers) → `golang-structs-interfaces`.

---

### `samber/cc-skills-golang@golang-modernize` ⭐️

Modernize Golang code using recent language features — range-over-int, min/max builtins, iterators, slices/maps/cmp/slog stdlib packages, testing patterns (t.Context, b.Loop, synctest), and tooling upgrades.

Use when: upgrading a codebase to a newer Go version or replacing pre-generics patterns. Not for lint rule enforcement (→ `golang-lint`).

---

### `samber/cc-skills-golang@golang-refactoring` ⭐️ 🧠 ⚙️

Safe, staged, at-scale refactoring process for existing Golang code — blast-radius mapping, coverage-adaptive safety nets, tool-driven transforms (`gopls`, `gofmt -r`), breaking import cycles, type-alias gradual repair, and staged PR workflows.

Use when: restructuring existing packages, renaming or moving symbols across many callers, or breaking up large packages safely. Load alongside whichever target-state skill owns the destination shape (`golang-naming`, `golang-code-style`, `golang-project-layout`, `golang-design-patterns`, `golang-modernize`).

---

## QA & Performance

### `samber/cc-skills-golang@golang-benchmark` 🧠

Golang benchmarking, profiling, and performance measurement — pprof, trace, CPU/memory/block profiles, flame graphs, benchstat, CI regression detection, continuous profiling.

Use when: measuring performance, capturing profiles, comparing benchmark runs, or setting up CI regression detection. For applying optimization patterns → `golang-performance`. For debugging a crash → `golang-troubleshooting`.

---

### `samber/cc-skills-golang@golang-observability` ⚙️

Golang production observability — structured logging (slog), Prometheus metrics, OpenTelemetry tracing, pprof profiling endpoints, alerting, Grafana dashboards.

Use when: instrumenting a service for production monitoring. Not for temporary deep-dive investigation (→ `golang-benchmark`, `golang-performance`).

---

### `samber/cc-skills-golang@golang-performance` 🧠

Golang performance optimization — allocation reduction, CPU efficiency, memory layout, GC tuning, pooling, caching, hot-path optimization.

Use when: applying optimization patterns after profiling. Not for measurement methodology (→ `golang-benchmark`) or debugging workflow (→ `golang-troubleshooting`).

---

### `samber/cc-skills-golang@golang-testing` ⭐️ 🧠 ⚙️

Production-ready Golang tests — table-driven tests, fuzzing, fixtures, goroutine leak detection (goleak), snapshot testing, code coverage, integration tests, parallel tests.

Use when: writing or reviewing unit, integration, or fuzz tests (including suites using `github.com/stretchr/testify`). For measurement methodology → `golang-benchmark`.

---

### `samber/cc-skills-golang@golang-troubleshooting` ⭐️ 🧠

Systematic Golang debugging — common pitfalls, test-driven debugging, pprof capture, Delve debugger, race detection, GODEBUG tracing, production debugging.

Use when: debugging a panic, unexpected output, or hard-to-reproduce bug. Not for interpreting profiles (→ `golang-benchmark`) or applying optimization patterns (→ `golang-performance`).

---

## Project Setup

### `samber/cc-skills-golang@golang-cli`

Golang CLI application development — project layout, exit codes, signal handling, I/O patterns, argument parsing, terminal UX, Cobra command trees, and Viper configuration layering.

Use when: building, extending, or reviewing a CLI tool (including codebases using `github.com/spf13/cobra` or `github.com/spf13/viper`). For package API lookup → `golang-pkg-go-dev`.

---

### `samber/cc-skills-golang@golang-continuous-integration`

CI/CD pipeline configuration for Golang projects using GitHub Actions — build, test, lint, and release workflows.

Use when: setting up or improving a CI pipeline for a Go project.

---

### `samber/cc-skills-golang@golang-dependency-management`

Golang module dependency strategies — go.mod conventions, versioning, replace directives, tool dependencies, and multi-module workspaces.

Use when: managing go.mod, dealing with replace directives, or structuring a multi-module repo.

---

### `samber/cc-skills-golang@golang-gopls`

Semantic code intelligence for the local Golang build via `gopls` — go-to-definition, find references, call/implementation hierarchy, workspace symbol search, compiler diagnostics, safe rename, and structural refactors.

Use when: navigating definitions and call sites in local or `go.sum`-pinned code, checking compiler diagnostics after edits, or running safe workspace-wide renames. For packages not in the local build → `golang-pkg-go-dev`.

---

### `samber/cc-skills-golang@golang-how-to` ⭐️

Golang skills orchestrator — routes tasks to primary and secondary skills, disambiguates overlapping skill clusters, and configures project agent-config files (`/golang-how-to configure`).

Use when: starting any Go task to select the right combination of skills, resolving boundary questions between overlapping skills, or configuring always-loaded Go skills in a repository.

---

### `samber/cc-skills-golang@golang-pkg-go-dev`

Golang package and module exploration via `godig`, a pkg.go.dev API client (CLI + MCP server) — docs, symbols, versions, importers, licenses, and known vulnerabilities.

Use when: looking up a module's available versions, CVEs, docs/symbols, or who imports it, or searching pkg.go.dev. For upgrading deps → `golang-dependency-management`; for choosing a library → `golang-popular-libraries`.

---

### `samber/cc-skills-golang@golang-popular-libraries`

Curated recommendations for production-ready Golang libraries — when the stdlib is enough vs when to reach for a package.

Use when: choosing a library for a new concern (HTTP, logging, testing, CLI, DI, etc.). Once a library is chosen, inspect its current API and examples via `golang-pkg-go-dev`.

---

### `samber/cc-skills-golang@golang-project-layout`

Golang project structure and workspace setup — cmd/internal/pkg conventions, monorepo layout, CLI project structure, and when to keep things flat.

Use when: starting a new project or restructuring an existing one. For architectural patterns within the project → `golang-design-patterns`.

---

### `samber/cc-skills-golang@golang-stay-updated`

Resources to stay current with Golang — official channels, community hubs, key people to follow, learning resources.

Use when: looking for ways to track Go releases, proposals, and community news.
