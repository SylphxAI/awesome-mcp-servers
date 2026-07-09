# SOTA Family Roadmap

Status: adoption plan
Owner: SylphxAI awesome-mcp-servers fork
Scope: repo-local future plan and its role in the SylphxAI MCP family
Decision record: `docs/adr/ADR-DRAFT-mcp-family-sota-roadmap.md`

## Family Role

This repository is not an MCP server package. Its family role is ecosystem
intelligence and distribution: a curated market map that helps SylphxAI track
what developers are using, where MCP categories are forming, and where the
Sylphx MCP family should be clearer, faster, safer, or easier to adopt.

It must not become the source of truth for product decisions. Product decisions
live in the owning MCP repositories. This repo can help discovery and learning.

## Family Fit

| Project | Relationship |
| --- | --- |
| Architecture Reader MCP | Uses category intelligence to sharpen architecture-intelligence positioning. |
| CodeRAG | Uses category intelligence to sharpen code retrieval examples and install messaging. |
| Reader MCPs | Use category intelligence to keep evidence-first readers easy to discover and compare by capability class. |
| Filesystem MCP | Uses category intelligence to track safety and local-operation expectations. |
| Consultant MCP | Can use curated category lists as research input when reviewing strategy. |

## SOTA End State

The SylphxAI fork should become a lightweight ecosystem radar for MCP strategy:
clean categories, star and adoption snapshots, capability tags, install-quality
signals, and gaps that inform product roadmaps without duplicating product state
from the owning repos.

## Runtime Direction

This repository does not need a Rust core. If automation is added, it should be
simple and generated: scripts that refresh metadata, validate category format,
and emit read-only reports. Durable product facts remain in the product repos.

## Roadmap

### Phase 0: Boundary And Ownership

- Add a project boundary that says this is a curated ecosystem map, not a
  product SSOT.
- Define the categories that matter to the Sylphx MCP family: evidence readers,
  code intelligence, safe local operations, deliberation, data connectors, and
  deployment/runtime tools.
- Keep upstream sync policy explicit if this remains a fork.

### Phase 1: Metadata Hygiene

- Add machine-readable entries for repo URL, category, language, install path,
  license, local/hosted mode, and update timestamp.
- Add a validation script so the list is not manually inconsistent.
- Add generated star and freshness snapshots as read models only.

### Phase 2: Category Radar

- Add category scorecards for install quality, tool clarity, local-first trust,
  benchmark proof, and evidence quality.
- Emit periodic reports that product repos can cite as research input.
- Avoid product claims that should live in the product repos.

### Phase 3: Family Discovery

- Add a Sylphx MCP family section with concise links to the owning product repos.
- Keep the section generated from a small manifest to avoid drift.
- Use this repo as a top-of-funnel discovery surface, not a replacement for
  product docs.

## Star And Adoption Strategy

This repo should help the family grow by making the category easier to navigate.
Its own star target is secondary to the product repos, but a high-quality public
radar can send developers toward the Sylphx MCP suite.

## Validation Gates

- Category entries validate against a schema before merge.
- Generated snapshots are marked as read models.
- Product claims link to owning repos rather than duplicating their state.
- Upstream sync behavior is documented before large fork-specific changes.
