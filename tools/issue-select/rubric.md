# Rubric: is this a good first issue?

<!--
THIS IS THE PART YOU WRITE. The skill in SKILL.md executes whatever checks
you define here. It ships empty on purpose: the judgment is your work.

A filled rubric must contain:

1. At least one row in the checks table. Each row needs all four columns:
   - Check: a short name (used in the output JSON).
   - Evidence: exactly what to look at, and where. Name the source
     (repo-facts block, issue body, comment thread, or the locations in
     references/evidence-guide.md). "The repo" is not a source; "the last
     5 default-branch commit dates" is.
   - Pass condition: a condition someone else could apply and get your
     answer. Prefer thresholds with numbers ("a maintainer commented
     within 30 days") over adjectives ("maintainer is responsive").
   - Weight: `required` (a fail here rejects the issue) or `preferred`
     (never changes the verdict; a nice-to-have that helps rank the
     issues you accept).

2. A verdict rule below the table: how the check grades combine into
   accept or reject, including how `unclear` is treated. The verdict
   space is binary. If you write no rule for `unclear`, the skill treats
   it as fail.

Cover what actually kills first contributions. The lecture named four
families: the maintainer is alive, the repo is in use, the scope fits a
newcomer, and nobody else is already on it. A rubric that ignores a family
will fail eval issues designed around that family.
-->

## Checks

| Check | Evidence | Pass condition | Weight |
|---|---|---|---|
| Maintainer alive | Repo facts: last 5 default-branch commits, their authors, and maintainer first-response sample; Comments: author_association and dates | Pass if a human maintainer committed to the default branch within 90 days, a maintainer first responded to a sampled issue within 30 days, or a commenter marked Owner, Member, or Collaborator responded in this issue within 30 days. A bot commit alone does not pass. | required |
| Repo in use | Repo facts: archived flag, latest release, last push to any branch, and stars | Pass if the repo is not archived and either its latest release or last push was within 180 days of the capture date. Stars alone do not pass this check. | required |
| Bounded contribution | Issue body and Comments: requested work, tracking lists, design discussion, and maintainer guidance | Pass if the issue asks for one identifiable change. Fail if it is only a usage question, explicitly tracks multiple separate tasks, has an unresolved design debate, or a maintainer says it requires substantial core-internals work. Missing reproduction steps alone do not fail it. | required |
| Work available | Repo facts: this issue's assignees and linked PR states; Comments: PR mentions, claims, and their dates | Pass if there is no assignee, open PR, or current claim from someone working on it. A closed unmerged PR alone does not count as a current claim. Use the thread to resolve conflicting signals. | required |
| AI contribution allowed | Repo facts: contribution policy, including AI policy and template requirements | Fail only if the policy outright prohibits the AI-assisted contribution workflow. Pass if the policy is silent or permits AI use with conditions such as disclosure, testing, or human review. | required |
| Starting guidance | Issue body and Comments: good-first-issue label, acceptance criteria, file pointers, or maintainer guidance | Pass if at least one of these is present. | preferred |

## Verdict rule

Accept if every required check passes. Reject if any required check fails. Treat an unclear required check as a fail; unclear preferred checks do not affect the verdict. Use preferred checks only to rank accepted issues. Measure dates against the repo-facts capture date in eval mode and against today in live mode.
