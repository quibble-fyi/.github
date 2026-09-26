# quibble roadmap

What we're building, what's committed, and what we've deliberately not
started. Generated from the issue tracker, so it cannot quietly go stale.

*Last generated 26 September 2026.*

## Where the work is grouped

Milestones are **outcomes**, not releases. quibble has no tags and no release
artefacts — a version number says what changed, not what it was for.

### Engineering hygiene

`█████░░░░░` **50%** — 13 done, 13 to go

Tooling, CI and auth debt that slows every other milestone down. Nothing here is user-visible; all of it is why the rest can move.

### New trackers & stacks

`█░░░░░░░░░` **14%** — 1 done, 6 to go

Teams on Jira, Linear, Azure DevOps and other trackers, and apps not written in Python or built as SPAs, can adopt quibble.

### Platform coverage

`████████░░` **81%** — 22 done, 5 to go

Every tracker and framework claim is backed by a run against a real instance. 'supported' means tested, not inferred.

### Ready to adopt

`██░░░░░░░░` **25%** — 1 done, 3 to go

What stands between quibble working and someone outside the lab being able to use it: distribution, licence, and a public demo that proves the claims.

### Reporter experience

`████████░░` **82%** — 14 done, 3 to go

The widget and the loop back to the person who filed. Everything a submitter sees, and what happens after they press Save.

### Licence & pricing

`█████░░░░░` **50%** — 3 done, 3 to go

A company can tell in one read whether quibble is free for them or what it costs, pay without friction, and never have quibble phone home or degrade. Epic

### Security & trust

`███░░░░░░░` **33%** — 1 done, 2 to go

What a security reviewer asks before approving quibble has an answer: who filed it, what the token can do, and what runs in our CI.

### Mobile & accessibility

`███████░░░` **67%** — 2 done, 1 to go

The widget works on a phone and for keyboard and screen-reader users: every control on screen, reachable and big enough to tap.


## What's next

### Next

*Committed, and started when what's in flight lands.*

- More trackers and frameworks, each proven against a running instance
- Run quibble as a sidecar container, so apps in any language can use it
- Tell submitters what happened to the note they filed
- Verify a signed identity token, not only a trusted proxy header
- Jira Cloud as a tracker
- An npm package for React, Vue and other single-page apps

### Later

*Agreed and unscheduled. Real, but not a date.*

- Jira Data Center and Jira Server as a tracker
- Decide on Azure DevOps, Redmine, Bitbucket, YouTrack, Shortcut and ClickUp
- Widget appearance options — position, theme and accent colour
- GitHub App authentication, as an alternative to a long-lived token
- Linear as a tracker

## Licence

**Free for individuals and small companies; US$499 a year for everyone else.** quibble is licensed under the PolyForm Small Business License 1.0.0: free for companies with fewer than 100 people and less than US$1M revenue. Larger companies buy a Company licence, US$499 per company per year, with no seat counting. See https://quibble.fyi/pricing/.

## Not started, on purpose

Two things people ask about that are open decisions rather than backlog:

- **Publishing to PyPI.** Installing is from git today, which needs a token we mint. It is friction and we know it.
- **A public comparison page.** Every claim on this page is currently self-asserted. We would rather say that than publish a table we scored ourselves.

## The rule behind the first milestone

**"Supported" means we ran it against a real instance.** Not inferred from
documentation. Of the first nine differences found between two trackers that
both advertise the same API shape, four were absent from the docs and
three returned *silently wrong answers* rather than errors.

That is why every tracker in the README carries a version number, and why one
of them is marked untested instead of claimed.

---

Questions, or want to try it: **hello@quibble.fyi**
