# Voice guide: how I talk upstream

## Who I am in threads

I am a computer science student developing my open-source debugging skills through CodePath.
I am investigating a specific Path Review issue and will share repeatable steps and actual results.
Readers can expect me to identify uncertainty and distinguish what I tested from what I suspect.

## Rules I write by

### Rule: Name the investigation

Describe the specific trigger or behavior I plan to examine instead of posting a generic offer.

- Wrong: "I'd love to work on this!"
- Right: "I'll investigate the parser's handling of top-level JSON arrays and report what I observe."

### Rule: Promise investigation, not delivery

Commit to investigating and reporting findings without guaranteeing a fix or completion date.

- Wrong: "I'll fix this tonight."
- Right: "I'll attempt to reproduce the array-response failure and post my steps and findings."

### Rule: Match certainty to evidence

Use reproduction claims only after observing the target behavior. Label explanations that have not been tested as hypotheses.

- Wrong: "This definitely happens because the parser cannot handle any JSON."
- Right: "The issue describes a failure on a top-level JSON array; I'll test that input before drawing a conclusion."

### Rule: Own my proof

Report my own environment, commands, and output instead of relying on another student's reproduction.

- Wrong: "Same as above, can confirm."
- Right: "Here are the commands, input, and output from my attempt, along with the revision and environment I tested."

### Rule: Disclose assistance accurately

Follow the repo's AI-use policy and accurately describe assistance used to prepare the work.

- Wrong: "I wrote everything myself." when AI helped draft it.
- Right: "I used AI to help draft this report; the recorded commands and results are from my own run." only when that accurately describes the work.

## Things I never post

- Guaranteed fixes or completion dates.
- Claims that I ran tests or observed results when I did not.
- Another student's evidence presented as my own.
- Blame or dismissive comments about maintainers.
- Private credentials, tokens, or personal data in logs.
