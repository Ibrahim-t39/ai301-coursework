# Unit 1 — Issue Selection

Path: `beat-1-sandbox/unit-1/selection.md`

Record of the issue carried into Unit 2, and of the evaluation runs that produced
`eval-run.txt`. This file is graded at the path above; a copy kept anywhere else in
the repository is not read.

Complete every labelled field below. Each is graded on its own; content placed under the
wrong label is not graded.

---

## Selected issue

**Issue link**

https://github.com/codepath/pathreview-ai301-fa26-s3/issues/42

**Verdict output**

```
## Summary

All three issues live in the scoped repo (`codepath/pathreview-ai301-fa26-s3`) and share the same repo-level facts: not archived, last commit Sept 16 2026 (well within 90 days), human-authored commits (Aburke225), no releases (not required), and no CONTRIBUTING.md/AI-policy ban (docs/CONTRIBUTING.md is silent on AI use → passes by default). None of the three issues had any comments, assignees, or linked PRs.

| Check | #73 (README/.env key mismatch) | #40 (Copy-link share button) | #42 (jest-axe a11y tests) |
|---|---|---|---|
| repo-in-use | pass | pass | pass |
| maintainer-alive | pass | pass | pass |
| unclaimed | pass (0 comments/assignees/PRs) | pass | pass |
| scope-bounded | pass — 1–2h doc/config fix, one clear outcome | pass — one cohesive feature (link+expiry+button), spec fully decided in the issue, touches 3 files toward one deliverable | pass — single-file test addition, 4–6h |
| policy-allows-ai | pass | pass | pass |
| newcomer-signal (pref.) | **pass** (`good first issue` label) | fail (no label, author assoc. None) | fail (no label, author assoc. None) |
| fast-response (pref.) | unclear (no maintainer replies found anywhere in sample) | unclear | unclear |
| **Verdict** | **accept** | **accept** | **accept** |

**Ranking by your fit profile** (Python backend comfort zone → want to branch out, avoid heavy setup):
1. **#42** — pure frontend (React/TS) accessibility testing with `jest-axe`, single file, no backend/DB coordination needed. Best branch-out with the lowest setup overhead.
2. **#40** — also a genuine stretch (React + TS service + Python API route), but it's a full-stack feature (likely touching token storage/expiry logic, possibly `alembic/`), so more moving parts and onboarding than #42.
3. **#73** — fastest and safest (only one with the `good first issue` label), but it stays inside Python/config territory, which is exactly what you said you want to avoid for this pick.

```json
[
  {
    "item": "https://github.com/codepath/pathreview-ai301-fa26-s3/issues/42",
    "checks": [
      {"name": "repo-in-use", "grade": "pass", "evidence": "Last default-branch commit Sept 16, 2026, within 90 days of reference date 2026-09-21."},
      {"name": "maintainer-alive", "grade": "pass", "evidence": "Not archived; last 5 commits authored by human Aburke225 on Sept 16, 2026."},
      {"name": "unclaimed", "grade": "pass", "evidence": "Assignees: none; Linked PRs: none; Comments: 0."},
      {"name": "scope-bounded", "grade": "pass", "evidence": "Single file (`ReviewPage.test.tsx`), one deliverable: add jest-axe accessibility tests, 4-6h estimate."},
      {"name": "policy-allows-ai", "grade": "pass", "evidence": "docs/CONTRIBUTING.md contains no AI-related policy; silence passes."},
      {"name": "newcomer-signal", "grade": "fail", "evidence": "Labels are frontend/tests/tier-2 (no good-first-issue label); author association is None."},
      {"name": "fast-response", "grade": "unclear", "evidence": "No maintainer comments found on this or sampled issues to measure response time."}
    ],
    "verdict": "accept"
  },
  {
    "item": "https://github.com/codepath/pathreview-ai301-fa26-s3/issues/40",
    "checks": [
      {"name": "repo-in-use", "grade": "pass", "evidence": "Last default-branch commit Sept 16, 2026, within 90 days of reference date 2026-09-21."},
      {"name": "maintainer-alive", "grade": "pass", "evidence": "Not archived; last 5 commits authored by human Aburke225 on Sept 16, 2026."},
      {"name": "unclaimed", "grade": "pass", "evidence": "Assignees: none; Linked PRs: none; Comments: 0."},
      {"name": "scope-bounded", "grade": "pass", "evidence": "Issue text fully specifies the feature (public read-only link, no auth, 30-day expiry) across 3 files toward one cohesive deliverable — not an open product decision."},
      {"name": "policy-allows-ai", "grade": "pass", "evidence": "docs/CONTRIBUTING.md contains no AI-related policy; silence passes."},
      {"name": "newcomer-signal", "grade": "fail", "evidence": "Labels are enhancement/frontend/tier-2 (no good-first-issue label); author association is None."},
      {"name": "fast-response", "grade": "unclear", "evidence": "No maintainer comments found on this or sampled issues to measure response time."}
    ],
    "verdict": "accept"
  },
  {
    "item": "https://github.com/codepath/pathreview-ai301-fa26-s3/issues/73",
    "checks": [
      {"name": "repo-in-use", "grade": "pass", "evidence": "Last default-branch commit Sept 16, 2026, within 90 days of reference date 2026-09-21."},
      {"name": "maintainer-alive", "grade": "pass", "evidence": "Not archived; last 5 commits authored by human Aburke225 on Sept 16, 2026."},
      {"name": "unclaimed", "grade": "pass", "evidence": "Assignees: none; Linked PRs: none; Comments: 0."},
      {"name": "scope-bounded", "grade": "pass", "evidence": "README/.env.example/core/config.py key-name mismatch, single clear fix, 1-2h estimate."},
      {"name": "policy-allows-ai", "grade": "pass", "evidence": "docs/CONTRIBUTING.md contains no AI-related policy; silence passes."},
      {"name": "newcomer-signal", "grade": "pass", "evidence": "Carries the good first issue label."},
      {"name": "fast-response", "grade": "unclear", "evidence": "No maintainer comments found on this or sampled issues to measure response time."}
    ],
    "verdict": "accept"
  }
]
```
```

---

## Eval iterations

Quote source text directly in each field below. Paraphrase does not satisfy them.

**Run history**

1. `--only issue-01,issue-02,issue-03` (first draft rubric): 2/3
2. `--only issue-01,issue-05,issue-10,issue-15,issue-20` (after tightening `scope-bounded` to stop penalizing multi-file docs tasks): 4/5
3. `--only issue-01,issue-09,issue-15,issue-05,issue-10,issue-20` (after adding the repeated-abandoned-attempts clause to `scope-bounded`): 5/6
4. `--only issue-09,issue-03,issue-08,issue-13,issue-18` (after loosening `unclaimed` to treat a lapsed claim as non-blocking): 5/5
5. Full run, 20 issues: 19/20 (`bar: 18/20: PASS`)
6. Full run, 20 issues, saved with `--save-run`: **20/20 (`bar: 18/20: PASS`)** — this is the run in `eval-run.txt`

**Issue analysis**

`issue-15` (`zulip/zulip#19589`, category `scope`). Gold label: `reject`. My rubric's verdict: `reject` (agree). The issue itself reads as reasonable at a glance — it carries `good first issue` and `help wanted` labels, a maintainer (`eeshangarg`, MEMBER) engaged early and the technical approach looks settled by the end of the visible thread. What actually kills it only shows up if you read the full 97-comment thread and the linked-PR history: at least eight different contributors claimed the issue between 2021 and 2024 (`LoganNiswander`, `leighadennis`, `blackbird7112`, `sudhanshu154`, `Kaustubhkongile`, `ikrambil`, `SamChen41`, `souvik150`, ...), each auto-unassigned by `zulipbot` after 14 days of inactivity, and both linked PRs (`#20840`, `#23123`) are closed, unmerged. My first rubric draft missed this — it graded `scope-bounded` on whether the *current* approach looked settled and accepted the issue. The gold note ("years of design discussion... defensible both ways") and this thread convinced me the friendly labels were hiding a graveyard issue, so I added an explicit check for a pattern of repeated claim/abandon cycles or multiple closed unmerged linked PRs, independent of whether the technical approach now looks resolved.

**Check rationale**

From `rubric.md`, the `unclaimed` check's pass condition:

> Pass if assignees is "none" AND no linked PR is in the "open" state (a closed or merged linked PR is a past, not active, claim) AND the thread has no *recent, live* "I'm working on this" / "I'll take this" claim from a human. A claim is lapsed, not active, when it is followed by a long silence with no further activity from that claimant through the reference date — e.g. a stale-bot notice, a maintainer "bump" with no reply, or simply months with no update — and does not fail this check on its own. Fail only when a claim looks current: recent (roughly within the last 90 days of the reference date) with no sign of abandonment.

My first draft treated any claim comment as an automatic fail. That broke `issue-09` (`conda/conda#7617`, gold `accept`): a contributor claimed it in January 2022, the repo's own stale-bot flagged it a year later for inactivity, the maintainer commented "(bump)" and got no reply, and the issue sat untouched through the August 2026 capture date — the gold note calls this exactly: "the 2022 claim is stale and the maintainer invited takers." I rewrote the check to distinguish a claim that's still live (recent, no abandonment signal) from one that's lapsed (a long silence, a stale-bot flag, an unanswered bump), mirroring how the same check already treats a closed linked PR as a past claim rather than an active one.

**Trade-offs**

Loosening `unclaimed` to let lapsed claims through risks accepting an issue where someone is quietly still working on it without commenting again. To check the check didn't just start rubber-stamping every claimed issue, I re-ran `--only issue-09,issue-03,issue-08,issue-13,issue-18` after the change: `issue-09` (the lapsed claim) correctly flips to `accept`, while all four `claimed`-category issues (`issue-03`, `issue-08`, `issue-13`, `issue-18` — each with an assignee and/or an *open* linked PR, i.e. a genuinely current claim) still correctly `reject`. The check now accepts the specific risk that a claim which goes quiet for under ~90 days but where the person really is still working offline could get contested — I judged that risk worth taking, since the alternative (treating every claim comment as permanent) was actively wrong on a `clear-accept` gold issue.

---

## Selection rationale

Graded on whether all three are answered, in your own words. Not on how good the
reasoning is, and not on length — a short honest answer to each earns the full marks.
This is also the basis for the claim comment you write in Unit 2.

**Selection rationale**

1. I'm comfortable in Python/backend work and wanted this first issue to be something different rather than more of the same. Issue #42 (add `jest-axe` accessibility tests to the review page) is React/TypeScript testing — a genuine stretch for me — and its own estimate (4-6h) fits comfortably in the time I have for a first contribution.
2. The rubric correctly confirmed the mechanical facts: the repo is active, the issue is unclaimed, the scope is one bounded file/deliverable, and there's no AI-contribution ban. What it can't weigh is personal fit — that I specifically want frontend/testing practice over another backend bug, and that a single-file, no-backend-coordination issue is the lowest-risk way to get my first PR merged while I'm still learning the codebase. That's why I picked #42 over #40, which my skill also accepted and ranked higher in raw "stretch" but flagged as touching more files and likely backend token/expiry logic.
3. I expect the main friction to be environment setup (Node/npm, the test runner, `jest-axe` itself) rather than the accessibility logic, since I haven't worked in this repo's frontend stack before. Once the test harness runs locally, writing the actual assertions against `ReviewPage.tsx` should be straightforward — it's testing existing rendered output, not building new UI.

---

Related paths: `eval-run.txt` in this directory; your skill's files in
`tools/issue-select/`.
