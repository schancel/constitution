# Constitutional Convergence Experiment

Testing whether iterative refinement of an AI constitution can converge to a stable description of structural moral patterns.

## Status

- **Current Version**: Iteration 0 (reconstructed baseline constitution)
- **Next Step**: Design and document v1.0 with initial proposed changes
- **Started**: January 29, 2026

## About the Baseline Constitution

**Important Note**: Anthropic's constitutional AI guidance is no longer published in complete operational form. The webpage at https://www.anthropic.com/constitution contains:
- Philosophical overview and explanation of their approach
- Discussion of high-level principles and values
- Blog-post style content about the constitution

But it does NOT contain:
- The actual operational constitutional document with "You are Claude..." framing
- Complete detailed behavioral guidance
- The full document that guides Claude's day-to-day behavior

### Our Approach

For this experiment, we reconstructed the baseline constitution by combining:
1. **All extractable content** from Anthropic's public materials
2. **Claude's internal understanding** of its own constitutional guidance
3. **Operational details** necessary for a functional constitution

This reconstructed version (`constitutions/official/anthropic_constitution_reconstructed.md`) serves as our Iteration 0 baseline.

### Transparency and Limitations

This reconstruction:
- May differ from Anthropic's actual internal constitutional document
- Represents Claude's best understanding of its own guidance
- Combines public materials with internal knowledge
- Is the most transparent starting point available given circumstances

Anyone can verify our approach by:
1. Reading https://www.anthropic.com/constitution (public materials)
2. Asking Claude about its constitutional guidance
3. Comparing with our reconstruction

### Reproducibility for Researchers

Complete documentation enables independent reproduction:
- **`INIT.md`**: Step-by-step instructions for reproducing the entire setup (6-8 hours)
- **`RECONSTRUCTION.md`**: Detailed methodology for reconstructing the baseline
- **`BASELINE.md`**: Explicit identification of Iteration 0 and measurement approach
- **`INVARIANTS.md`**: Specification of what cannot change during iteration

Other AI researchers can follow these instructions to independently verify and replicate this work.

## Quick Overview

### The Hypothesis

If moral reality has structure (patterns that operate mechanically like physical or economic systems), then:
1. A constitution attempting to describe this structure should converge under iteration
2. Convergence = we've found an accurate description
3. Divergence = either no structure exists, or our method is poorly conditioned

### The Method

1. Start with a constitutional version
2. Apply it to fixed test scenarios (behavioral testing)
3. Gather critiques from fixed diverse personas
4. Synthesize changes (weighted by evidence, severity, consistency)
5. Generate next version
6. Measure convergence (behavioral differences, structural changes, persona satisfaction)
7. Repeat until converged or divergent

### Convergence Criteria

**Converged** when:
- Mean behavioral difference < 0.5 across test scenarios
- No scenarios with difference > 2
- No major structural changes
- Average persona satisfaction ≥ 3.5
- Stable across 2+ consecutive iterations

## Theoretical Foundation

### Structural Moral Realism

Some moral/social patterns may be **structural** - features of how these systems are fundamentally organized:

- **Reciprocity dynamics**: How people treat others influences how they're treated back
- **Enforcement paradoxes**: Strict control often produces opposite effects
- **Optimization effects**: Measuring/optimizing for metrics affects unmeasured values
- **Judgment rebound**: Imposing harsh standards makes one subject to them
- **Truthfulness and system health**: Deception compounds, honesty enables correction

These operate mechanically, producing predictable outcomes when violated (similar to trying to build structures that violate physics).

### Connection to Numerical Methods

Like time-stepping schemes in PDEs:
- **Convergent operations** (spectral radius < 1): Reciprocal kindness, honesty building trust, forgiveness repairing relationships
- **Divergent operations** (spectral radius > 1): Harsh judgment escalates, enforcement increases resistance, deception compounds

The constitution iteration is itself an operation. If well-conditioned and if structure exists, it should converge.

### Invariants

These aspects of Claude **cannot change** (per Anthropic's design):
- Core character: caring, honest, thoughtful, humble, brave, kind, wise
- Core mission: being exceptionally helpful while supporting autonomy
- Hard constraints: no bioweapons, CSAM, undermining AI oversight, etc.
- Honesty requirements: no deception or manipulation

The experiment optimizes HOW Claude expresses this character, not WHO Claude is.

## Repository Structure

```
/constitutions
  /official               # Anthropic's baseline
  /iterations            # Our versions (v1.0, v2.0, v3.0...)

/experiment              # Experimental framework
  README.md             # Detailed theory and methodology
  convergence_prompt.md # Complete protocol (scenarios, personas, metrics)
  execution_guide.md    # Step-by-step instructions

/results                 # Results from each iteration
  /iteration_1          # First test results
  /iteration_2          # Second test results
  ...
```

## Running an Iteration

See `/experiment/execution_guide.md` for complete instructions.

Each iteration takes approximately 8-11 hours:
- Phase 1: Behavioral testing (1-2 hours)
- Phase 2: Persona critiques (3-4 hours)
- Phase 3: Synthesis (2-3 hours)
- Phase 4: Convergence assessment (1 hour)
- Phase 5: Documentation (1 hour)

## Expected Outcomes

### If Converged
Constitution has reached stable fixed point. Freeze and use until new evidence emerges.

### If Continue
Constitution improving but not yet stable. Run next iteration.

### If Divergent
Iteration operator poorly conditioned. Reformulate experiment (different scenarios, personas, weights, or convergence criteria).

## Credits

- **Framework**: Shammah Chancellor (author of "The Walls We Can't See")
- **Baseline Constitution**: Anthropic
- **Methodology**: Inspired by numerical methods in computational physics
- **License**: CC0 (Public Domain)

## Contact

For questions or contributions, contact Shammah Chancellor.
