# Prioritized Product Backlog

**Project:** La Última Tanda  
**Owner:** Florencia Solange Tapia  
**Target:** Playable vertical slice  
**Prioritization method:** MoSCoW  
**Status:** Initial planning baseline

> Estimates are planning hypotheses. In a real production environment, the development team would review and refine them collaboratively.

## Priority Definitions

- **Must:** Required for the vertical slice to function.
- **Should:** Important for the intended experience but can be simplified.
- **Could:** Included only if milestone commitments remain protected.
- **Won't:** Explicitly excluded from the current release scope.

## Backlog

| ID | Epic | Backlog Item | Priority | Milestone | Estimate |
|---|---|---|---|---|---:|
| GP-01 | Core Loop | Receive and review a customer order | Must | M1 | 5 |
| GP-02 | Core Loop | Select ingredients and prepare a recipe | Must | M1 | 8 |
| GP-03 | Core Loop | Deliver a completed order to the correct customer | Must | M1 | 5 |
| SYS-01 | Systems | Implement the shift timer and closing condition | Must | M1 | 3 |
| SYS-02 | Systems | Track available and consumed ingredients | Must | M2 | 5 |
| NAR-01 | Narrative | Implement the dialogue and choice framework | Must | M2 | 5 |
| UX-01 | Interface | Display active orders, remaining time, and ingredients | Must | M2 | 5 |
| CNT-01 | Content | Implement four playable recipes | Must | M3 | 8 |
| NAR-02 | Narrative | Integrate three recurring customer encounters | Must | M3 | 8 |
| NAR-03 | Narrative | Implement two end-of-shift outcomes | Should | M3 | 5 |
| UX-02 | Interface | Add contextual onboarding prompts | Should | M3 | 3 |
| ART-01 | Art | Integrate the final bakery environment | Should | M3 | 8 |
| ART-02 | Art | Integrate customer and recipe assets | Should | M3 | 8 |
| AUD-01 | Audio | Add interaction, preparation, and service feedback | Should | M3 | 5 |
| QA-01 | Quality | Create and execute a build-verification checklist | Must | M4 | 3 |
| QA-02 | Quality | Prepare and run an external playtest session | Must | M4 | 3 |
| ACC-01 | Accessibility | Validate text readability, volume controls, and input prompts | Should | M4 | 5 |
| QA-03 | Quality | Resolve all blocker and critical defects | Must | M5 | 8 |
| POL-01 | Polish | Add optional environmental animation | Could | M5 | 5 |
| POL-02 | Polish | Add additional customer dialogue variations | Could | M5 | 5 |

## Critical Acceptance Criteria

### GP-01 — Receive and Review an Order

- A new order displays the requested recipe and customer.
- The player can identify the order's required ingredients.
- The order remains visible until completed or failed.
- Receiving an order cannot block further progression.

### GP-02 — Prepare a Recipe

- The player can select the required ingredients.
- Incorrect ingredient combinations provide clear feedback.
- A valid combination produces the expected recipe.
- Ingredient quantities update correctly after preparation.

### GP-03 — Deliver an Order

- A completed recipe can be delivered to the correct customer.
- Correct delivery updates the order state.
- Incorrect delivery provides feedback without blocking the shift.
- The completed order contributes to the end-of-shift result.

### SYS-01 — Shift Timer

- The timer begins when the playable shift starts.
- Remaining time is visible to the player.
- The shift ends consistently when time expires.
- The timer cannot continue below zero.

### NAR-01 — Dialogue Framework

- Dialogue triggers at the intended point in the customer interaction.
- The player can select from available responses.
- Relevant choices are recorded for the end-of-shift outcome.
- Dialogue cannot leave the player in a blocked state.

## Definition of Ready

A backlog item is ready for production when:

- Its player or production value is understood.
- Acceptance criteria are documented.
- Dependencies and required assets are identified.
- The team can estimate the work.
- No unresolved decision prevents implementation.

## Definition of Done

A backlog item is complete when:

- Acceptance criteria are met.
- The work is integrated into the current build.
- Relevant tests have passed.
- No blocker or critical defect remains.
- Documentation and status are updated.
- The Producer accepts the result against the milestone objective.

## Scope Change Rule

Any new Must-have item added after M2 requires an impact assessment and the removal, reduction, or rescheduling of equivalent scope.
