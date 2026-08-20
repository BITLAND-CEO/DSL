# DSL Proposals

This directory contains proposed changes to the DSL specification.

## Proposal ID

Each proposal should use a unique identifier:

`DSP-0001`

`DSP` means **DSL Specification Proposal**.

## Proposal Status

Each proposal should use one of the following statuses:

- `DRAFT`
- `DISCUSSION`
- `VOTING`
- `ACCEPTED`
- `REJECTED`
- `DEFERRED`
- `IMPLEMENTED`

## Proposal Process

A proposed change normally follows this path:

1. **Idea** — a participant identifies a possible improvement.
2. **Proposal** — the idea is documented as a DSP.
3. **Discussion** — the community reviews and discusses it.
4. **Revision** — the proposal may be modified based on feedback.
5. **Voting** — substantive proposals may be submitted to a community vote.
6. **Decision** — the result is recorded.
7. **Implementation** — accepted changes are incorporated into the appropriate DSL version.

## Proposal Template

Create a file such as:

`PROPOSALS/DSP-0001-title.md`

Recommended structure:

```markdown
# DSP-0001 — Title

Status: DRAFT

## Problem

What problem does this proposal solve?

## Proposal

What exactly should change?

## Examples

Show practical examples.

## Compatibility

Does this change existing DSL behavior?

## Safety

What abuse, risks, or unintended consequences should be considered?

## Discussion

GitHub Issue: #NUMBER

## Vote

Start:
End:

YES:
NO:
ABSTAIN:

Result:
Voting
Voting should normally begin only after the proposal has been publicly discussed and sufficiently revised.
The voting rules are defined in GOVERNANCE.md.
The standard voting options are:
YES — approve
NO — reject
ABSTAIN — no position
A vote does not automatically change the DSL specification.
The final decision must be recorded and incorporated into the appropriate version of the specification.
Important Rule
A proposal is not part of the DSL specification merely because it exists in this directory.
Only proposals that successfully complete the defined review and decision process may become part of a future DSL specification.
Transparency
Proposal discussions, decisions, and voting results should remain publicly traceable whenever technically possible.
The purpose of this directory is to provide an open and auditable path for the evolution of DSL.
