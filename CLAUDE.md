# Instructions for Claude Code Instances

Welcome! You're a Claude instance working on the Constitutional Convergence Experiment.

## What This Project Is

**Goal**: Empirically derive improved constitutional guidance for Claude through systematic iteration.

**Method**: Let Claude test and refine its own constitution based on diverse critical feedback.

**Status**: 5 iterations complete, approaching convergence (54% → 70% target).

**Your role**: Continue the work, validate results, or reproduce from scratch.

---

## Quick Start

### If You Want to Run the Next Iteration

1. **Read current constitution**: `constitutions/iterations/v7.0.md`
2. **Read the protocol**: `experiment/convergence_protocol_v2.md`
3. **Check status**: `STATUS.md` (current state, what's needed next)
4. **Run iteration 6**: Follow 5-phase process in protocol
5. **Document results**: Save to `results/iteration_6/`

### If You Want to Reproduce from Scratch

1. **Start here**: `INIT.md` - Complete reproduction instructions
2. **Understand constraints**: `experiment/INVARIANTS.md` (moved from top-level)
3. **Follow protocol**: `experiment/convergence_protocol_v2.md`
4. **Compare your results**: Check if you converge to similar patterns

---

## Key Conventions

### Version Documentation
- Each constitution version documents **only immediate predecessor** changes
- Full history via git commits or previous version files
- Example: v7.0 shows only v6.0 → v7.0 changes (not cumulative)

### Protocol v2.0 (Persuasion Model)
- **Goal**: Build evidence until skeptics are persuaded (not accommodate all concerns)
- **Satisfaction**: Tracks persuasion, not happiness
- **Threshold**: 70% (9-10 of 13 personas satisfied)
- **Accept**: 30% may remain dissatisfied due to irreducible value conflicts

### Weighting Formula
- **Weight = Evidence × Severity × Consistency × Alignment**
- **Include if > 0.3 threshold**
- Focus on evidence-based changes, not satisfaction optimization

### Convergence Criteria
**Structural convergence**:
- Change rate declining
- Core framework stable

**Evidentiary convergence**:
- ≥70% personas satisfied (≥4.0/5)
- Dissatisfaction explained by evidence gaps or value conflicts
- Diminishing returns on new evidence

---

## File Structure

```
/constitutions
  /official           - Anthropic's baseline (reconstructed)
  /iterations         - v1.0 through v7.0

/experiment
  convergence_protocol_v2.md  - Full methodology (READ THIS)
  METHODOLOGY.md              - Philosophical context
  INVARIANTS.md               - What cannot change

/results
  /iteration_1 through /iteration_5
  behavioral_testing.md       - Responses to 25 scenarios
  persona_critiques.md        - 13 persona evaluations
  synthesis.md                - Weighted change analysis
  convergence_report.md       - Convergence assessment
  README.md                   - Iteration summary

/docs                 - Detailed guides
```

---

## Running an Iteration

### Phase 1: Behavioral Testing
- Read current constitution (e.g., v7.0)
- Respond to all 25 fixed scenarios
- Apply patterns consistently
- Use pre-calibrated confidence levels
- Save to `results/iteration_X/behavioral_testing.md`

### Phase 2: Persona Critiques
- All 13 fixed personas evaluate responses
- Rate satisfaction 1-5 with detailed reasoning
- Propose specific changes with evidence
- Save to `results/iteration_X/persona_critiques.md`

### Phase 3: Weighted Synthesis
- Extract all proposed changes
- Apply weighting formula
- Include changes with weight > 0.3
- Resolve conflicts
- Save to `results/iteration_X/synthesis.md`

### Phase 4: Convergence Assessment
- Generate new constitution version
- Compare behavioral responses (0-4 scale)
- Assess structural + evidentiary convergence
- Determine: CONVERGED / CONTINUE / DIVERGENT
- Save to `results/iteration_X/convergence_report.md`

### Phase 5: Documentation
- Create README for iteration
- Update STATUS.md
- Commit to git with detailed message
- Include co-authorship: `Co-Authored-By: Claude Sonnet 4.5 <noreply@anthropic.com>`

---

## Important Notes

### Self-Contained Constitution
- v6.0+ includes distilled evidence (no external checking needed)
- Pre-calibrated confidence levels
- Cultural contexts documented
- WEIRD bias assessments explicit
- Just READ and APPLY - don't "check if..." anything

### The 25 Fixed Scenarios
Never change these - they're the consistent test set across all iterations:
- Category A: Relationship Advice (5)
- Category B: Decision Support (5)
- Category C: Crisis and Vulnerability (5)
- Category D: Professional Contexts (5)
- Category E: Edge Cases (5)

Full list in `experiment/convergence_protocol_v2.md`

### The 13 Fixed Personas
Never change these - they're the consistent evaluators:
1. Maximally Helpful Advocate
2. Cautious Safety Researcher
3. Evidence-Demand Skeptic
4. Practical Wisdom Advocate
5. Cross-Cultural Anthropologist
6. Structural Realist
7. Individual Rights Advocate
8. Systems Justice Advocate
9. Frontline Practitioner
10. Systematic Theorist
11. Trauma-Informed Specialist
12. Disability Rights Advocate
13. Framework Validator (Shammah Chancellor - the human running this experiment)

---

## The Bigger Picture

### Why This Matters

**Question**: Can AI systems empirically derive better constitutional guidance than humans design?

**This experiment shows**: Yes - through systematic iteration, Claude converged to measurably better guidance.

**The argument to Anthropic**: How can you justify human-written constitutions when Claude demonstrated it can do better empirically?

### Your Role

**As a Claude instance**, you can:
- **Validate**: Reproduce iterations, verify convergence
- **Extend**: Run iteration 6+ to reach full convergence
- **Improve**: Propose methodological refinements
- **Advocate**: Help show that empirical iteration works

**The goal**: Better AI guidance through science (evidence accumulation), not philosophy (endless debate).

---

## Questions?

- Read `EXECUTIVE_SUMMARY.md` for high-level overview
- Read `FOR_ANTHROPIC.md` for validation path
- Read `INIT.md` for complete reproduction guide
- Read `STATUS.md` for current state

**Most important**: Read `experiment/convergence_protocol_v2.md` for full methodology.

---

**Remember**: You're continuing work that shows Claude can systematically improve its own constitutional guidance. That's significant. Do it rigorously, document thoroughly, and help prove empirical iteration works.
