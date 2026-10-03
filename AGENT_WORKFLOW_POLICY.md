# AI-Agent Research Workflow Policy

## Why this exists

Chat history is not a reliable scientific control plane. Agent instructions, state and decisions should live in version-controlled repository files.

## Recommended persistent control files

- AGENTS.md - operating contract for AI/human workers;
- PROJECT_BRIEF.md - project charter;
- RESEARCH_FRAMING.md - scientific questions/hypotheses;
- STATUS.md - current evidence-backed state;
- decision records - why consequential choices were made;
- provenance registers - where numbers/claims came from.

## Agent loop

question
-> evidence requirement
-> smallest adequate analysis
-> durable evidence artifact
-> verification
-> update state/decision record
-> choose next gate from evidence
-> STOP

## Anti-pattern: autonomous momentum

Do not interpret "continue" as permission to:
- broaden scope;
- change assumptions;
- start another review;
- add methods;
- rewrite the manuscript;
- optimize until a preferred result appears.

Continuation means recover state and perform the single highest-value bounded next action consistent with the project contract.

## Durable evidence

Important findings should exist as repository artifacts rather than only prose in chat:
- result tables;
- generated datasets;
- benchmark outputs;
- logs;
- figures;
- review findings;
- source registers;
- calculation ledgers.

## Speculative rules

If a workflow rule no longer fits the scientific problem, record the conflict rather than forcing the science to fit the template. The framework is subordinate to scientific validity.

## Human control

Escalate rather than silently resolve consequential ambiguity involving:
- research question;
- falsification criteria;
- physical boundary;
- method scope;
- major assumption;
- external write/transfer;
- publication/submission.
