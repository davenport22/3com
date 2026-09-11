# 05 Product and MVP Specification

Language: English (build documentation). Revised after the Startup Council, see `12-startup-council.md`.

## What changed in this revision

The original spec described an open session board where anyone posts an ad-hoc session and
others join. The Council rejected that as the v1 scope, and the founding situation confirms it:

- **Coincidence maths.** Joint training requires four simultaneous matches: time, place,
  discipline, pace. Below roughly 250 active users in one city most cells are empty. Ad-hoc
  matching does not work at low density, no matter how good the software is.
- **Central events are the launch plan.** Weekly anchors, coached specials and a winter indoor
  programme are all organiser-led, recurring and known in advance. None of them needs an ad-hoc
  board.

So v1 is not a marketplace. **v1 is the operating system for a small number of recurring
sessions that the founders and, later, other hosts run.**

## MVP thesis

> **A recurring session exists -> the right people find it and commit -> they show up ->
> the host knows who is coming -> it happens again next week.**

Ad-hoc posting, discovery by filter and the social feed are v2. They unlock at density, not
before.

## Scope decision

A custom PWA, built in the founders' base training season (see `10-roadmap.md`), not during
their peak block. A PWA rather than native because it ships without store review, runs on both
platforms from one codebase, and the core use case is committing to a session, not tracking one.

## v1 feature scope

### In scope

**Onboarding and profile**
- Sign in with email magic link, optional Strava OAuth
- Profile: name, photo, home district, disciplines, target race and date
- **Tempo group, not pace numbers.** Three named groups per discipline, self-selected:
  - **Kaffeefahrt** (you can hold a conversation)
  - **Tempo** (short sentences only)
  - **Vollgas** (no talking)
  A numeric band sits behind each group for later matching logic and for Strava-derived
  suggestions, but no user ever sees an interval. Groups overlap deliberately at the edges; a
  member near a boundary is offered both.

**Recurring sessions (the core)**
- A session series: discipline, weekday, time, meeting point, session type, tempo groups
  offered, capacity per group, host, cost, notes
- Each occurrence is its own instance: a member commits to a date, not to the series
- Series page shows the next three occurrences and who has committed to each
- Host can cancel a single occurrence with a reason, or pause a series

**Commitment, not registration**
- One-tap "ich bin dabei" per occurrence, closing at a defined time before the start
- Confirmation prompt 12 hours before: still coming, yes or no
- Attendance marked afterwards by the host in one tap
- **Reliability shown on the profile** as a plain ratio of shown-up to committed. Not a score,
  not a badge, just the number. No-shows are the fastest way to kill a recurring session, and
  visibility is the cheapest available mechanism.

**The host is the primary user**
Every screen is judged by one question: does it make it easier for someone other than a founder
to take over a session? Concretely:
- "Diese Einheit übernehmen" on any series, with a one-screen handover
- Host view: who is coming per group, quick message to committed members, one-tap cancel
- Duplicate a series to create a new one in under 60 seconds
- A short host guide inside the product: how to run two tempo groups, what to say at the start,
  what to do when nobody comes

**Curated and brand sessions**
- Same object as a peer series, with a `layer` flag, optional cost, optional coach, optional
  external booking link
- Limited spots with a waiting list, because coached sessions and studio slots are capacity-bound
- Cost shown transparently as "Coach 120 EUR, geteilt durch Teilnehmende" in the pass-through phase

**Notifications**
- New occurrence opens for commitment
- Reminder 12 hours before, with the confirm prompt
- Session cancelled or moved
- Host notification when commitments drop below a threshold

**Trust and safety**
- Real name and photo required
- No 1:1 direct messages. Group thread per occurrence only.
- Report and block
- Community guidelines at signup, including an explicit "this is not a dating platform" clause
- Liability notice at commitment: participation at own risk, own equipment, own insurance

**Admin**
- Series management, feature a session, member list
- Metrics that matter: commitment-to-attendance ratio, repeat rate per member, sessions hosted
  by someone other than a founder

### Explicitly out of scope for v1

- Ad-hoc one-off session posting by members (v2, unlocks at roughly 250 active users)
- Discovery by filter and map browsing (v2, pointless with under 10 series)
- Social feed, kudos, photo timeline (v2 at the earliest, and only if it is not just Strava again)
- In-app payments (external link or cash at the session)
- 1:1 messaging
- Training plans, FTP, TSS, structured workouts
- Multi-city in the UI (the data model carries `city_id` from day one, the switcher stays hidden)
- Native apps

The one thing to resist reversing: the ad-hoc board. It is the feature that feels like the
product and behaves like an empty room.

## Key user stories

| # | As a | I want to | So that | Priority |
|---|---|---|---|---|
| 1 | member | commit to next Saturday's ride in two taps | I have a fixed point in my week | P0 |
| 2 | member | pick a tempo group by how it feels, not by a number | I do not feel graded before I have even started | P0 |
| 3 | host | see who is actually coming, per group | I can plan the route and not wait for nobody | P0 |
| 4 | host | take over an existing series without asking anyone | the session survives when the founders are unavailable | P0 |
| 5 | founder | run a coached session with limited spots and shared cost | the community gets quality it cannot self-organise | P0 |
| 6 | founder | book an indoor slot as a series over the winter | there is a reason to show up in January | P0 |
| 7 | member | be reminded 12 hours before and confirm | the host is not left guessing | P1 |
| 8 | beginner | read what actually happens at this session before committing | I know whether I belong there | P1 |
| 9 | member | post a one-off session of my own | I get company for a session outside the fixed rhythm | **v2** |

## Screens (v1)

1. **Diese Woche** (default): the next occurrences across all series, with your commitment state
2. **Serie** : what this session is, who hosts it, the next three dates, tempo groups, commit
3. **Occurrence detail**: participants per group, meeting point, group thread, host controls
4. **Serie anlegen / übernehmen**: one scrolling form with sensible defaults
5. **Profil**: tempo groups, target race, upcoming commitments, reliability ratio
6. **Onboarding**: 4 steps, under 90 seconds, ending on a commitment to a real session

The default screen is "Diese Woche", not a board. That single choice encodes the whole revision:
the product answers "what am I doing this week and with whom", not "what is out there".

## Definition of done for the MVP

Not feature completeness. The MVP is done when, for four consecutive weeks:

- at least **five recurring series** are live,
- at least **two of them are hosted by someone other than the two founders**,
- the median occurrence has **four or more people who actually showed up**,
- and the **commitment-to-attendance ratio is above 70 percent**.

The second criterion is the one that decides whether this is a company or a hobby.
