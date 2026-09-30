# Evidence guide: where proof lives in a reproduction package

## Environment

- Where it lives: In eval mode, compare the repro report's environment record with the issue context and repo-facts block. In live mode, compare the draft's environment record with the issue and relevant README, dependency manifests, and setup docs.
- What good looks like: The tested revision and behavior-relevant runtime, dependencies, platform, and configuration are identifiable. Differences from the target are stated; irrelevant details are not mandatory.

## Steps

- Where it lives: The repro report's setup instructions, commands, input examples, configuration, and action that triggers the behavior. In live mode, use repo setup docs to assess those instructions, but do not use unpublished local files to fill gaps in the draft.
- What good looks like: A stranger can start from the stated revision and repeat the attempt without guessing consequential details. Necessary custom inputs are included or accessible through a specific reference.

## Behavior shown

- Where it lives: The issue context's trigger and expected/actual behavior, compared with the report's output excerpts, logs, screenshots, or other recorded artifacts. In live mode, read the actual issue and the artifacts included or quoted in the draft.
- What good looks like: The artifact demonstrates the target behavior under the relevant trigger, or records what happened during a relevant unsuccessful attempt. A setup failure or adjacent exception cannot establish reproduction of the target bug.

## Honesty

- Where it lives: Statements in the claim and repro conclusion compared with the report's steps, environment, and artifacts.
- What good looks like: The conclusion states only what the evidence supports and separates observations from hypotheses. A supported cannot-reproduce or blocked result is valid when limitations are explicit; an unsupported success claim is not.

## Comms

- Where it lives: The claim comment compared with the issue's specifics, and both comments compared with contribution requirements in the eval repo-facts block. In live mode, consult the scoped repo's README, CONTRIBUTING, applicable templates, and linked policies; also read voice-guide.md.
- What good looks like: The claim identifies a concrete investigation without promising a fix or date. Comments follow explicit repo requirements, including AI-use disclosure when required, and present the author's own evidence respectfully. Another student's claim does not block a claim in Path Review, and another student's reproduction cannot substitute for the author's evidence.

## Evidence boundaries

In eval mode, use only the bundle text; never fetch outside evidence. In live mode, fetch issue-side context and policies, but judge candidate proof from what the draft comments contain and quote. Missing evidence is unclear; do not assume a command ran or an artifact exists.
