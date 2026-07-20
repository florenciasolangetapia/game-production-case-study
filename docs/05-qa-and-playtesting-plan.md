# QA and Playtesting Plan

**Project:** La Última Tanda  
**Owner:** Florencia Solange Tapia  
**Target:** Playable vertical slice  
**Status:** Draft — execution not started

## Quality Objectives

The vertical slice should:

- Remain playable from the beginning to the end of one complete shift.
- Communicate the core gameplay loop without external explanation.
- Provide clear feedback for valid and invalid player actions.
- Preserve narrative progression regardless of dialogue choices.
- Support readable text, understandable controls, and adjustable audio.
- Contain no blocker or critical defects in the release candidate.

## Test Stages

| Stage | Milestone | Purpose |
|---|---|---|
| Core-loop verification | M1 | Confirm that receiving, preparing, and delivering one order works |
| Feature verification | M2 | Validate the complete shift and connected gameplay systems |
| Internal playtest | M3 | Assess usability, pacing, clarity, and narrative flow |
| External playtest | M4 | Observe new players without development-team guidance |
| Regression and release verification | M5 | Confirm fixes and protect previously working functionality |

## Test Coverage

### Functional

- Order creation and completion
- Ingredient selection and consumption
- Recipe validation
- Shift timer and closing condition
- Customer dialogue and choices
- End-of-shift outcomes
- Restart and recovery from failed actions

### Usability

- Clarity of the current objective
- Visibility of active orders
- Readability of recipe requirements
- Understanding of interaction feedback
- Time required to learn the core loop
- Points where players request assistance

### Narrative

- Correct dialogue sequence
- Choice tracking
- Customer continuity
- Relationship between choices and outcomes
- Player understanding of narrative consequences

### Accessibility Baseline

- Text remains readable at supported resolutions.
- Essential information is not communicated through color alone.
- Music and sound-effect volume can be adjusted.
- Input prompts remain visible and consistent.
- Timed interactions do not require excessively precise input.

## Defect Severity

| Severity | Definition | Example |
|---|---|---|
| **Blocker** | Testing or progression cannot continue | The shift cannot start or complete |
| **Critical** | A core feature fails with no reasonable workaround | Orders cannot be delivered |
| **Major** | Important functionality is impaired but progression remains possible | Ingredient quantities update incorrectly |
| **Minor** | Limited impact on gameplay or presentation | Incorrect text alignment |
| **Trivial** | Cosmetic issue with no meaningful player impact | Small visual inconsistency |

## Bug Report Template

Every defect should include:

- Clear and searchable title
- Build version
- Test environment
- Preconditions
- Reproduction steps
- Expected result
- Actual result
- Reproduction frequency
- Severity
- Screenshot or video when useful
- Related backlog item

## External Playtest

### Participants

Target: 8–10 players who enjoy cozy, narrative, or light-management games and have not previously seen the project.

### Session Structure

1. Five-minute introduction without gameplay instructions
2. One complete 20–25 minute shift
3. Observation without intervention
4. Ten-minute post-session interview
5. Short written feedback form

### Observation Metrics

- Time required to understand the core loop
- Percentage of players completing the shift
- Number of requests for assistance
- Failed or abandoned orders
- Most common interaction errors
- Dialogue choices and remembered consequences
- Moments of frustration, confusion, or satisfaction

## Target Playtest Criteria

- At least 80% of participants complete the shift.
- Most participants understand the core loop within five minutes.
- No participant encounters a blocker defect.
- At least 70% can describe one consequence of their decisions.
- Repeated usability problems are documented and prioritized.

These are target criteria, not completed test results.

## Feedback Triage

Feedback will be evaluated according to:

1. Frequency across participants
2. Impact on the intended experience
3. Relationship to the vertical-slice goals
4. Implementation effort and production risk

Not every suggestion will become backlog work. Accepted changes must protect the milestone objective and agreed scope.

## Release-Candidate Exit Criteria

- Zero open blocker defects
- Zero open critical defects
- Major defects reviewed and explicitly accepted or scheduled
- Core-loop regression tests passed
- Complete shift verified on the supported environment
- Playtest findings reviewed
- Known issues documented
- Final build approved against M5 criteria
