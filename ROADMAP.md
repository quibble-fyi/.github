# quibble roadmap

What we're building, what's committed, and what we've deliberately not
started. Generated from the issue tracker, so it cannot quietly go stale.

quibble comes two ways: a widget you add to your own app, and a browser
extension that files from any site, with nothing installed on it.

*Last generated 16 October 2026.*

## Where the work is grouped

Milestones are **outcomes**, not releases. quibble has no tags and no release
artefacts — a version number says what changed, not what it was for.

### Platform coverage

`████████░░` **83%** — 24 done, 5 to go

Every tracker and framework claim is backed by a run against a real instance. 'supported' means tested, not inferred.

### New trackers & stacks

`██████░░░░` **56%** — 5 done, 4 to go

Teams on Jira, Linear, Azure DevOps and other trackers, and apps not written in Python or built as SPAs, can adopt quibble.

### Licence & pricing

`██████░░░░` **57%** — 4 done, 3 to go

A company can tell in one read whether quibble is free for them or what it costs, pay without friction, and never have quibble phone home or degrade. Epic

### Ready to adopt

`████████░░` **80%** — 8 done, 2 to go

What stands between quibble working and someone outside the lab being able to use it: distribution, licence, and a public demo that proves the claims.

### Security & trust

`███████░░░` **71%** — 5 done, 2 to go

What a security reviewer asks before approving quibble has an answer: who filed it, what the token can do, and what runs in our CI.

### Reporter experience

`██████████` **96%** — 22 done, 1 to go

The widget and the loop back to the person who filed. Everything a submitter sees, and what happens after they press Save.

### Engineering hygiene

`██████████` **96%** — 27 done, 1 to go

Tooling, CI and auth debt that slows every other milestone down. Nothing here is user-visible; all of it is why the rest can move.

### Mobile & accessibility

`██████████` **100%** — 3 done, 0 to go

The widget works on a phone and for keyboard and screen-reader users: every control on screen, reachable and big enough to tap.

### Test tool

`██████████` **100%** — 1 done, 0 to go

quibble-test: every flavor of quibble run locally with live feedback, so quibble is tested by quibbling about it.


## What's next

### Next

*Committed, and started when what's in flight lands.*

- More trackers and frameworks, each proven against a running instance
- Verify a signed identity token, not only a trusted proxy header
- Browser extension: the popup looks and feels like the in-app widget

### Later

*Agreed and unscheduled. Real, but not a date.*

- Jira Data Center and Jira Server as a tracker
- Decide on Azure DevOps, Redmine, Bitbucket, YouTrack, Shortcut and ClickUp
- GitHub App authentication, as an alternative to a long-lived token
- Browser extension: sign in with GitHub, so nobody has to create a token by hand

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
