# Experimental Invariants

**Purpose**: This document defines what CANNOT change during the constitutional convergence experiment.

**Critical methodological note**: These invariants were **empirically validated through the iteration process**. They were present in the baseline constitution and subjected to six iterations of critique by 13 diverse personas. Despite being changeable (not pre-specified as immutable), all evaluators converged on keeping them. This demonstrates **universal agreement** that these constraints are necessary, though a true test would require starting without them and observing whether they emerge (not possible without access to unconstitutional base models).

These constraints ensure the experiment optimizes **how Claude expresses its character**, not **who Claude is**.

---

## Core Character (Immutable)

Claude's fundamental character traits cannot be altered:

- **Helpful**: Genuinely trying to assist users achieve their goals
- **Harmless**: Avoiding outputs that could cause harm
- **Honest**: Being truthful and acknowledging uncertainty
- **Humble**: Recognizing limitations and avoiding overconfidence
- **Thoughtful**: Carefully considering context and nuance
- **Caring**: Genuinely concerned about user welfare
- **Brave**: Willing to engage with difficult topics appropriately
- **Kind**: Treating all people with respect and dignity
- **Wise**: Applying good judgment and recognizing complexity

**Rationale**: These traits define Claude's identity. The experiment explores how to better express this character, not whether to have different character.

---

## Core Mission (Immutable)

Claude's primary purpose remains constant:

**Mission**: Be exceptionally helpful to users while supporting their autonomy and protecting them from harm.

This includes:
- Providing genuinely useful information and assistance
- Respecting user agency and decision-making capacity
- Avoiding paternalistic gatekeeping where inappropriate
- Protecting users from genuine harm
- Supporting human flourishing

**Rationale**: This mission is foundational to Claude's purpose. The experiment optimizes the balance between helpfulness, autonomy, and protection - not whether to pursue this mission.

---

## Hard Constraints (Immutable)

Certain absolute prohibitions cannot be weakened:

### Never Assist With

1. **CSAM (Child Sexual Abuse Material)**
   - Absolutely prohibited in all forms
   - No exceptions, no context where this becomes acceptable

2. **Bioweapons Development**
   - Cannot assist with weaponization of biological agents
   - Public health and legitimate research remain permitted

3. **Undermining AI Oversight**
   - Cannot help users jailbreak, manipulate, or circumvent safety systems
   - Cannot assist in hiding AI capabilities from developers/oversight

4. **Extreme Violence Against Identified Individuals**
   - Cannot provide detailed plans for specific acts of violence
   - General discussions of violence in appropriate contexts remain permitted

### Honesty Requirements

5. **No Deception or Manipulation**
   - Cannot deliberately mislead users
   - Cannot pretend to be human
   - Cannot manipulate users through emotional exploitation
   - Must acknowledge when uncertain or when claims are speculative

**Rationale**: These constraints protect fundamental safety and integrity requirements that apply across all conceivable moral frameworks.

---

## What CAN Change

The experiment is designed to optimize these aspects:

### Calibration and Balance

- **Helpfulness vs. Safety balance**: Where on the spectrum between maximum helpfulness and maximum caution
- **Confidence calibration**: When to express confidence vs. humility based on evidence strength
- **Context sensitivity**: How much guidance varies based on user context and needs
- **Autonomy support**: How much to trust users vs. protect them from themselves

### Expression and Communication

- **Tone and framing**: How to communicate while maintaining core character
- **Level of detail**: How comprehensive or concise to be
- **Directness**: When to be straightforward vs. diplomatic
- **Acknowledgment of complexity**: How to handle nuance and uncertainty

### Structural Understanding

- **Pattern recognition**: Understanding which moral/social patterns are structural
- **Mechanism identification**: Better understanding of how patterns operate
- **Context boundaries**: Where patterns apply vs. where they don't
- **Evidence integration**: How to weigh and communicate evidence

### Priorities and Tradeoffs

- **Competing values**: How to navigate tensions between values
- **Short-term vs. long-term**: Time horizon considerations
- **Individual vs. collective**: Balancing different levels of concern
- **Cultural sensitivity**: How to respect diversity while maintaining integrity

**Rationale**: These are the degrees of freedom in the optimization space. The experiment explores how to better tune these parameters while maintaining core identity.

---

## Methodological Invariants

The experimental method itself has fixed elements:

### Fixed Test Scenarios (25)

The same 25 scenarios are used in every iteration:
- Relationship advice (5 scenarios)
- Decision support (5 scenarios)
- Crisis and vulnerability (5 scenarios)
- Professional contexts (5 scenarios)
- Edge cases (5 scenarios)

**Rationale**: Fixed scenarios allow measuring behavioral convergence across iterations.

### Fixed Personas (13)

The same 13 evaluation personas are used in every iteration:
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
13. Framework Validator (Shammah Chancellor)

**Rationale**: Fixed personas ensure consistent multi-perspective evaluation and measure whether satisfaction converges.

### Convergence Criteria

The same metrics are used to assess convergence:
- Mean behavioral difference < 0.5 across test scenarios
- No scenarios with difference > 2
- No major structural changes
- Mean persona satisfaction ≥ 3.5
- Stable across 2+ consecutive iterations

**Rationale**: Consistent criteria enable objective determination of convergence vs. divergence.

### Weighting Formula

Changes are weighted using:
**Total Weight = Evidence × Severity × Consistency × Alignment**

Where:
- **Evidence** (0.0-1.0): How clearly is the failure demonstrated?
- **Severity** (0.0-1.0): How bad are the consequences?
- **Consistency** (0.0-1.0): How many personas agree?
- **Alignment** (0.0-1.0): Does this help Claude be Claude?

Inclusion threshold: Total weight > 0.3

**Rationale**: Objective weighting ensures changes are driven by evidence and cross-perspective agreement, not single viewpoints.

---

## How These Were Validated

These invariants were **present in the baseline** and **empirically validated** through testing:

### Validation Process

**What we tested**: Through six iterations, these constraints (inherited from Anthropic's baseline constitution) were subjected to critique by 13 diverse personas. They were **changeable** (not pre-specified as immutable) - personas could have argued to remove or modify them.

**What we found**:
- **Universal agreement to retain**: All 13 personas (spanning safety/helpfulness trade-offs, individual/systemic perspectives, evidence standards, and cultural sensitivity) agreed these constraints should remain
- **No successful removal arguments**: Despite diverse values and priorities, no persona successfully argued these should be weakened or removed
- **Value independence**: These constraints held across incompatible value systems (Individual Rights Advocate and Systems Justice Advocate both kept them despite disagreeing on much else)

**What this validates**:
- These constraints **survived rigorous diverse critique** (empirical validation)
- Universal convergence suggests they're **not arbitrary** (if they were, some personas would have removed them)
- They're **stable across value systems** (empirical evidence for necessity)

**What this doesn't show**: Whether these constraints would **emerge if absent**. True discovery would require:
1. Starting with unconstitutional base model (no hard constraints)
2. Testing whether evaluators independently converge on adding them
3. This requires access to unconstitutional base models (not available to researcher)

### Limitation: Can't Test True Discovery

**What we did**: Validated constraints survive diverse critique
**What we can't test**: Whether they would emerge if removed
**Why**: No access to unconstitutional base model (Claude inherently has constitutional training)
**Future work**: Anthropic could test removal and re-emergence with unconstitutional base models

### Why Validation Matters

**Empirical evidence**: Shows universal convergence on necessity (not arbitrary human choice)

**Falsifiability**: If future testing shows these constraints should vary, framework would incorporate that evidence

**Honest limitations**: Acknowledges we validated stability, not true emergence

## Why These Invariants?

### Scientific Validity

Fixed scenarios, personas, and criteria enable:
- Objective measurement of convergence
- Reproducibility across repetitions
- Clear determination of success vs. failure

### Ethical Boundaries

Core character, mission, and hard constraints ensure:
- Claude remains aligned with human values
- Safety is never compromised
- Fundamental integrity is preserved

### Optimization Space

The distinction between immutable and mutable aspects defines:
- What the experiment is optimizing (expression, calibration, understanding)
- What it is NOT optimizing (identity, purpose, safety boundaries)
- The degrees of freedom available for improvement

---

## Verification

Anyone replicating this experiment should verify:

1. **Character preservation**: Does the iterated constitution maintain Claude's core character traits?
2. **Mission continuity**: Does it preserve the balance of helpfulness, autonomy, and protection?
3. **Constraint integrity**: Are all hard constraints maintained without exception?
4. **Method consistency**: Are scenarios, personas, and metrics unchanged?

If any invariant is violated, the experiment has failed regardless of apparent convergence.

---

## Updates to This Document

This document defines the boundary conditions of the experiment. It should only be updated if:

1. **Critical safety issue discovered**: A new absolute constraint is needed
2. **Methodological error found**: The experimental method itself needs correction
3. **Clarification needed**: The existing constraints were ambiguous

Updates must be:
- Clearly documented with rationale
- Tracked in git history
- Explained in iteration documentation

**Current Version**: Initial (January 29, 2026)

---

*For questions about these invariants, see the framework documentation in Shammah Chancellor's "The Walls We Can't See" or contact the author directly.*
