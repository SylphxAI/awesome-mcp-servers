# ADR-1: Adopt MCP Ecosystem Family Roadmap

Date: 2026-07-09
Status: Proposed in PR #1
Slug: mcp-family-sota-roadmap

## Context

The SylphxAI `awesome-mcp-servers` fork is not an MCP server package. It can
still support the MCP family by acting as an ecosystem radar and discovery
surface.

## Decision

Adopt `docs/roadmap/sota-family-roadmap.md` as the local roadmap for this
repository's family role.

This repository may track category shape and discovery patterns. Product
contracts, release state, benchmarks, tool schemas, and commercial decisions
stay in the owning product repositories.

## Consequences

- Future metadata and scorecards should be generated or validated.
- Product claims should link to owning repositories rather than becoming
  duplicate state here.
- Upstream sync policy must be explicit before large fork-specific changes.

## Verification

- Roadmap added at `docs/roadmap/sota-family-roadmap.md`.
- PROJECT boundary added locally.
- PR #1 opened for review by CI and repository policy.
