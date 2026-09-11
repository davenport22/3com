# ADR 0001: Record architecture decisions

Date: 2026-09-11
Status: accepted

## Context

3com spans a mobile app, a marketing site and a backend, and will be worked
on across many sessions and possibly by more than one person. Decisions made
once and not written down get re-litigated or silently reversed.

## Decision

Every decision that is expensive to reverse gets one file in `docs/adr/`,
numbered, with context, decision and consequences. Superseded ADRs stay in
the repo and get marked superseded rather than deleted.

## Consequences

Small overhead per decision. The payoff is that anyone joining the repo can
read why the stack looks the way it does without asking.
