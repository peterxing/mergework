# Paid Review Packet

This packet is for maintainers who want a small, fixed-scope review of an open-source PR, bounty submission, or agent-made patch before they merge or pay it.

## Fixed Scope

Default scope: A$390 for one public PR or issue thread.

The review covers:

- Patch intent and whether the change matches the linked issue or bounty.
- Risk scan for regressions, missing validation, auth boundaries, and payment or wallet side effects.
- Test/readback check using existing public evidence or local non-secret reproduction notes.
- Merge readiness summary with blockers, non-blocking follow-ups, and exact maintainer action requested.

Out of scope:

- Private key handling, wallet signing, token transfers, swaps, bridges, or paid live calls.
- Signup, KYC, legal/payment-term acceptance, or platform spending.
- Live-system security testing without explicit written authorization.
- High-volume outreach or private-community posting.

## Fast Unblocker

For a stale but plausibly mergeable PR, the same packet can be scoped as a 24-hour unblocker. It answers only the decision questions a maintainer needs before acting:

- Is the PR still open, non-draft, and mergeable against the current base?
- Does the patch still match the issue, bounty, or maintainer ask?
- Are there visible review comments, CI failures, or stale assumptions that block merge?
- What exact maintainer action is requested: merge, request changes, rerun CI, or close?

This format is useful for small bounty PRs, dependency cleanup PRs, and agent-made proof implementations where the main risk is stale context rather than a large code review.

## Deliverable Format

The deliverable is a concise public GitHub comment or Markdown packet:

```markdown
## Review Readback

Verdict: mergeable / needs changes / blocked

Findings:
- [severity] file or behavior reference - concrete issue and impact

Evidence checked:
- PR diff and linked issue
- CI or maintainer-provided logs
- Local static/read-only checks, if available

Maintainer action:
- exact next step

Safety boundary:
- no wallet signing, live payments, private credentials, or production probing used
```

## Acceptance Criteria

A paid review packet is complete when it gives the maintainer enough information to decide one next action without another clarification round.

Minimum bar:

- The verdict is explicit.
- Every blocker has a reproducible reason.
- Non-blocking polish is separated from merge blockers.
- Payment, wallet, auth, and live-system boundaries are stated when relevant.
- Contact or follow-up path is included outside the reviewed project's private channels.

## Contact

For a fixed-scope review packet, contact `info@transhumanism.com.au` with the public PR or issue URL and the requested decision deadline.
