# Splox documentation

The source of [docs.splox.io](https://docs.splox.io). Mintlify, one `.mdx` per
page, arranged by `docs.json`.

## Running it

```bash
npx mint dev          # preview on http://localhost:3000
npx mint broken-links # every internal link and image
```

Mintlify's CLI needs an LTS Node; it refuses Node 25.

## What is where

| Directory | Pages |
| --- | --- |
| `concepts/` | machine, harness, program, agent, run, model — the vocabulary the rest depends on |
| `app/` | the product as a person uses it, screen by screen |
| `build/` | changing what an agent is: programs, agents, hooks, tools, sub-agents, skills, evals, versions |
| `tools/` | what an agent can reach: the shipped packages, MCP servers, and writing your own |
| `api/`, `sdk/` | the v2 API and the three SDKs |
| `account/` | plans, usage windows, billing, API keys |
| `tutorials/` | six end-to-end walkthroughs |
| `images/` | screenshots, grouped by the section that uses them |

`docs.json` also carries the redirects from the previous documentation, which
described a product built out of workflows, nodes and edges. Every one of its 85
paths lands somewhere in this tree; `/what-changed` is the page that maps the old
vocabulary onto the new one.

## Writing

Verified or absent: a page says what somebody ran, read in the source, or saw on
screen, and nothing else. No adjectives standing in for facts, no feature
described from memory. If a claim cannot be checked, it does not ship.
