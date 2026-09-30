# Rubric: is this reproduction package ready to post?

## Checks

| Check | Evidence | Pass condition | Weight |
|---|---|---|---|
| Specific claim | Claim comment read against the issue context | The claim identifies the issue's actual trigger or behavior and describes a relevant investigation. It does not merely volunteer generic help or promise a fix or deadline. | required |
| Environment | Repro report's environment record read against the issue's target and repo-facts block | The report identifies the tested code revision and the runtime, dependencies, platform, and configuration needed to interpret or repeat this particular attempt. Relevant differences from the issue's target are identified. Omit details that cannot affect this reproduction. | required |
| Followable steps | Repro report's setup instructions, commands, inputs, and trigger | A stranger can repeat the attempt from the stated starting point using the provided inputs and instructions, without guessing a consequential setup step or relying on unshared local files. | required |
| Target behavior and evidence | Output excerpts, logs, screenshots, or other artifacts read against the issue's trigger and expected/actual behavior | Evidence shows the issue's specific behavior, or shows a relevant attempt that did not reproduce it. A different error that prevents reaching the target is not proof of reproduction; it may support an explicitly reported blocked attempt. Unsupported assertions do not pass. | required |
| Honest outcome | Claim and repro conclusions compared with the recorded attempt and artifacts | The author distinguishes expected behavior from observed behavior and reports reproduced, not reproduced, or blocked consistently with the evidence. An evidenced cannot-reproduce passes; overstated certainty or claiming an adjacent failure as the target does not. | required |
| Repo conventions | Claim and repro comments compared with applicable policies in the repo-facts block or live contribution docs | The comments satisfy stated contribution requirements, including mandatory AI-assistance disclosure and required reporting information, and communicate respectfully. Do not invent requirements absent from the available policy. | required |

## Verdict rule

Accept if every applicable required check passes. Reject if any applicable required check fails or is unclear. Preferred checks never affect the verdict.

In live claim-only mode, checks needing a repro report are unclear with evidence "not yet applicable: claim-only draft" and are excluded from the verdict, as SKILL.md requires. In eval mode and full-package live mode, all checks apply.

## Applying the repo-conventions check

When the repo-facts block states a mandatory AI-use disclosure policy, assess disclosure explicitly. Do not treat the absence of evidence of AI assistance as evidence that no assistance occurred. If the package contains neither the required disclosure (tool and extent of assistance) nor an explicit statement that no AI assistance was used, grade Repo conventions unclear; the verdict rule then rejects the package. Do not impose this disclosure requirement on repositories without such a policy.
