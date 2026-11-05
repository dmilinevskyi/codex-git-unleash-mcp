# Issue tracker: GitHub

Issues and specs live in GitHub Issues for `dmilinevskyi/codex-git-unleash-mcp`.

## Conventions

Follow `docs/github-issues.md` for issue titles, bodies, labels, and scope.

Prefer GitHub MCP tools for issue operations. Use the `gh` CLI as a fallback
when the required operation is unavailable through MCP. Follow repository
policy for Git and pull request operations.

Before creating an issue, verify the target repository. Never file issues
in the upstream skills repository.

- Publish to the issue tracker: create a GitHub issue.
- Fetch the relevant ticket: read its body, labels, and comments.
- Link child tickets using native GitHub sub-issues where available.
  Otherwise, put `Part of #<parent>` at the top of each child and maintain
  a task list in the parent.
- Record blockers using native GitHub issue dependencies where available.
  Otherwise, put `Blocked by: #<number>` at the top of the blocked issue.
  A ticket is startable only when every blocker is closed.
- When closing an issue with an explanation, post the explanation before
  closing it. If already closed, post the explanation separately.
- Use `docs/agents/triage-labels.md` for canonical triage roles.

## Pull requests as a triage surface

**PRs as a request surface: no.**

## Wayfinding operations

The map is a single issue labelled `wayfinder:map`, holding Notes,
Decisions-so-far, and Fog.

- Child tickets are sub-issues of the map, with a `wayfinder:<type>` label:
  `research`, `prototype`, `grilling`, or `task`.
- Where sub-issues are unavailable, use the parent/child fallback above.
- The frontier is the map's open children without open blockers or an assignee;
  choose the first in map order.
- Claim a ticket by assigning it to the driving developer.
- Resolve it by commenting with the answer, closing it, and adding a summary
  and link to the map's Decisions-so-far.
