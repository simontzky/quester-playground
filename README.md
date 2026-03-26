# quester-playground

Playground repository for Quester agent e2e smoke tests.

Agents dispatched here can safely create branches, commits, and PRs without affecting production codebases.

## Usage

This repo is used by `quester smoke` to verify the full agent pipeline:
1. Webhook received
2. Agent dispatched to workstation
3. Agent executes (creates branch, commits, PR)
4. Completion reported back to orchestrator

## Structure

```
src/
  hello.js    -- minimal file agents can modify
CLAUDE.md     -- agent instructions for this repo
```
