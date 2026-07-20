# Risk and Dependency Register

**Project:** La Última Tanda  
**Owner:** Florencia Solange Tapia  
**Review cadence:** Weekly  
**Status:** Active during pre-production

## Scoring Method

Probability and impact are scored from 1 to 3.

- **1:** Low
- **2:** Medium
- **3:** High
- **Risk score:** Probability × Impact

Scores of 6 or 9 require an active mitigation plan and weekly review.

## Risk Register

| ID | Risk | P | I | Score | Response | Owner | Status |
|---|---|---:|---:|---:|---|---|---|
| R-01 | Additional recipes and narrative branches increase the vertical-slice scope | 3 | 3 | 9 | Lock scope after M2 and move new ideas to a future-opportunities list | Producer | Open |
| R-02 | The order-to-delivery loop is functional but not engaging | 2 | 3 | 6 | Test the core loop with placeholder assets before committing to final content | Design | Open |
| R-03 | Engineering work becomes a bottleneck for the small team | 2 | 3 | 6 | Limit work in progress, identify technical spikes early, and protect critical-path tasks | Engineering | Open |
| R-04 | Final art arrives too late for integration and iteration | 2 | 2 | 4 | Approve an asset list by M1 and review integration progress weekly | Art | Monitoring |
| R-05 | Dialogue changes create repeated implementation and audio work | 2 | 2 | 4 | Lock the dialogue structure by M2 and track later changes through change control | Narrative / Audio | Monitoring |
| R-06 | Unstable builds reduce the value of external playtesting | 2 | 3 | 6 | Introduce build verification and resolve blocker defects before test distribution | Engineering / QA | Open |
| R-07 | The absence of a dedicated QA role leaves defects unowned | 3 | 2 | 6 | Assign test ownership, use structured test sessions, and run weekly bug triage | Producer | Open |
| R-08 | Remote communication delays cross-functional decisions | 2 | 2 | 4 | Record decisions, owners, deadlines, and unresolved blockers in one visible location | Producer | Monitoring |

## Risk Triggers

| Risk | Trigger |
|---|---|
| R-01 | A proposed feature changes an approved milestone or adds more than two days of work |
| R-02 | Playtesters cannot explain the core loop after five minutes |
| R-03 | A critical engineering task remains blocked for more than two working days |
| R-04 | More than 20% of required vertical-slice assets remain unintegrated at the end of week 10 |
| R-05 | Dialogue structure changes after audio implementation begins |
| R-06 | Two consecutive builds contain progression-blocking defects |
| R-07 | High-priority defects remain untriaged for more than 48 hours |
| R-08 | A dependency remains unresolved because no decision owner is identified |

## Dependency Register

| ID | Dependency | Required By | Owner | Management Approach |
|---|---|---|---|---|
| D-01 | Validated core loop before final art production | M1 | Design / Engineering | Use greybox assets until the interaction model is approved |
| D-02 | Approved recipe requirements before final UI | M1 | Design | Document quantities, states, and player actions before interface implementation |
| D-03 | Stable dialogue format before audio planning | M2 | Narrative | Approve the structure before estimating audio work |
| D-04 | Stable build before external playtesting | M4 | Engineering | Complete build verification and blocker triage |
| D-05 | Clear acceptance criteria before QA execution | Every milestone | Producer | Add completion criteria to each backlog item |

## Review Rules

- Review high risks every week.
- Assign one accountable owner to every active response.
- Convert realized risks into tracked issues.
- Record material scope or schedule changes in the decision log.
- Close a risk only when the exposure no longer affects the vertical slice.
