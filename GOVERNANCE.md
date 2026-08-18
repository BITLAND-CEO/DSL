# DSL Governance v1.0

## Purpose

This document defines how the DSL project can evolve through open proposals, discussion, and community voting.

## 1. Proposal First

Any participant may submit a proposal.

A proposal should explain:

- the problem
- the proposed change
- why it is needed
- examples
- compatibility impact
- safety considerations

Proposals belong in `PROPOSALS/` and should normally have a corresponding GitHub Issue.

## 2. Discussion Period

A proposal should remain open for public discussion for at least **14 days** before a final decision.

Urgent security or safety corrections may use a shorter period when necessary.

## 3. Voting

For proposals that change DSL meaning, syntax, governance, or compatibility, a community vote should be opened after discussion.

Preferred voting mechanism:

1. GitHub Discussions Poll, if enabled.
2. Otherwise a clearly identified GitHub Issue vote.

The proposal must state:

- voting start date
- voting end date
- options
- eligibility rule
- result

The default voting period is **7 days**.

## 4. Vote Options

Standard options:

- YES — approve
- NO — reject
- ABSTAIN — no position

Abstentions are recorded but do not count as approval or rejection.

## 5. Approval Threshold

A substantive proposal is considered community-approved when:

- at least **2/3 of non-abstaining votes** are YES; and
- at least **5 eligible participants** vote.

If fewer than five participants vote, the result is recorded as **insufficient participation** and may be reopened.

For the early project, votes are advisory against the final repository decision. This prevents a small number of accounts from automatically changing the standard.

## 6. Final Decision

After the vote, maintainers publish the result and merge, reject, or request revision.

A rejected proposal may be resubmitted after substantial changes.

## 7. Editorial Changes

Typographical, formatting, documentation, and non-semantic corrections may be merged without a community vote.

## 8. Conflicts of Interest

Participants should disclose material conflicts of interest when relevant to a proposal.

## 9. Version Releases

A release should include:

- version number
- change summary
- accepted proposals
- rejected/deferred proposals where relevant
- compatibility notes

## 10. Governance Changes

Changes to this governance document follow the same proposal process.

## 11. Principle

No individual owns the meaning of DSL.

The repository is intended to preserve an auditable public record of how the specification evolves.
