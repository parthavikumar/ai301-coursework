# Unit 2 — Claim and Reproduce

Path: `beat-1-sandbox/unit-2/reproduction.md`

Record of your claim and reproduction on the issue you chose in Unit 1, and of the
evaluation runs that produced `eval-run.txt`. This file is graded at the path above; a copy
kept anywhere else in the repository is not read.

Complete every labelled field below. Each is graded on its own; content placed under the wrong
label is not graded.

---

## Your identity upstream

**GitHub username**

parthavikumar

---

## Posted upstream

**Claim comment**

[Link to the comment where you claimed the issue. Use the comment's own permalink, not the
issue page on its own. **Then paste the text of that comment underneath the link** — the
pasted text is what this field is graded on, so copy across what you actually posted.]

**Reproduction comment**

[Link to the comment where you posted your reproduction. It must record the environment
(OS, relevant versions, code state), steps a stranger could follow, and what you observed.
**Then paste the text of that comment underneath the link** — the pasted text is what this
field is graded on, so copy across what you actually posted.]

## Eval iterations

Answer all four sections. Quote source text directly; paraphrase does not satisfy these
fields.

**Run history**

1. Initial full run: 19/20. The disclosure category was 0/1, so the run did not pass.
2. Targeted retry using `--only pkg-20`: 1/1. The revised rubric rejected pkg-20, matching gold. This partial run did not determine the full bar.
3. Confirming full run: 19/20, PASS. Categories: clear-accept 7/8, disclosure 1/1, no-evidence 4/4, unfollowable-comms 3/3, wrong-target 4/4.


**Package analysis**

I examined pkg-20. Initially, my rubric accepted it while the gold label was reject. Its reproduction evidence supported the reported behavior, but its repo policy stated: "All AI usage in any form must be disclosed, stating the tool used and the extent of the assistance". Neither candidate comment included a disclosure. The initial grader passed Repo conventions because "no evidence of AI assistance exists to require disclosure." I clarified how to handle missing disclosure under an explicit mandatory policy. The targeted retry and final full run both rejected pkg-20, matching gold.


**Check rationale**

My Repo conventions check reads:

"The comments satisfy stated contribution requirements, including mandatory AI-assistance disclosure and required reporting information, and communicate respectfully. Do not invent requirements absent from the available policy."

I included this check because valid technical evidence alone does not establish that a comment meets the repository's contribution rules. After pkg-20 was missed, I added a clarification that silence about AI assistance should not automatically establish compliance with a mandatory disclosure policy. The final sentence limits the check to requirements actually stated by the repository.

**Trade-offs**

The confirming full run caught pkg-20 but falsely rejected pkg-03, which gold accepted. Pkg-03's policy says "comments to maintainers must be written by humans in their own words"; it does not state a mandatory AI-use disclosure requirement. The grader nevertheless marked Repo conventions unclear because the package had "no AI-assistance disclosure and no explicit 'no AI assistance used' statement." This shows a limitation: the grader applied my disclosure clarification too broadly. The final run passed at 19/20, but this false rejection remains unresolved.

---

Related paths: `eval-run.txt` in this directory; your skill's files in
`tools/repro-check/`.
