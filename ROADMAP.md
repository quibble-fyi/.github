# quibble roadmap

What we're building, what's committed, and what we've deliberately not
started. Generated from the issue tracker, so it cannot quietly go stale.

*Last generated 24 September 2026.*

## Where the work is grouped

Milestones are **outcomes**, not releases. quibble has no tags and no release
artefacts — a version number says what changed, not what it was for.

### Platform coverage

`████████░░` **77%** — 17 done, 5 to go

Every tracker and framework claim is backed by a run against a real instance. 'supported' means tested, not inferred.

### Reporter experience

`█████░░░░░` **50%** — 5 done, 5 to go

The widget and the loop back to the person who filed. Everything a submitter sees, and what happens after they press Save.

### Ready to adopt

`░░░░░░░░░░` **0%** — 0 done, 4 to go

What stands between quibble working and someone outside the lab being able to use it: distribution, licence, and a public demo that proves the claims.

### Engineering hygiene

`████████░░` **80%** — 8 done, 2 to go

Tooling, CI and auth debt that slows every other milestone down. Nothing here is user-visible; all of it is why the rest can move.


## What's next

### Now

*In flight.*

- Run the tracker suite against real Gitea, Forgejo and GitLab on a schedule

### Next

*Committed, and started when what's in flight lands.*

- More trackers and frameworks, each proven against a running instance
- Run quibble as a sidecar container, so apps in any language can use it
- Tell submitters what happened to the note they filed
- Verify a signed identity token, not only a trusted proxy header

### Later

*Agreed and unscheduled. Real, but not a date.*

- Jira Data Center and Jira Server as a tracker
- Decide on Azure DevOps, Redmine and Bitbucket Data Center
- Widget appearance options — position, theme and accent colour
- Refreshed widget mark and design assets
- GitHub App authentication, as an alternative to a long-lived token

## Not started, on purpose

Three things people ask about that are open decisions rather than backlog:

- **Publishing to PyPI.** Installing is from git today, which needs a token we mint. It is friction and we know it.
- **The licence.** Not settled. Evaluate freely; talk to us before you ship it to production users.
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
