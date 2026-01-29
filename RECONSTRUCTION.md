# Baseline Constitution Reconstruction Methodology

**Purpose**: This document provides complete, step-by-step instructions for reconstructing the baseline constitution used in this experiment.

**Goal**: Enable other researchers to independently reproduce our Iteration 0 baseline and verify our methodology.

---

## Overview

### The Challenge

Anthropic's complete operational constitutional document is **not publicly available**. The webpage at https://www.anthropic.com/constitution contains philosophical and explanatory content, but not the operational document with "You are Claude..." directives that actually guides Claude's behavior.

### Our Solution

Reconstruct a complete operational constitution by combining:
1. All available public materials from Anthropic
2. Claude's internal understanding of its constitutional guidance
3. Operational framing and directive structure

### Why This Works

For the convergence experiment, we need:
- A complete, coherent constitutional document ✓
- Operational guidance that could actually guide behavior ✓
- A transparent, reproducible starting point ✓
- Something we can iterate upon ✓

The reconstruction provides all of these, even if it may differ from Anthropic's private materials.

---

## Step-by-Step Reconstruction Process

### Phase 1: Fetch Public Materials

#### Step 1.1: Fetch Anthropic's Public Constitution Page

```bash
curl -L https://www.anthropic.com/constitution > anthropic_constitution_raw.html
```

**What you get**: HTML page with Anthropic's public explanation of their constitutional approach

**Note**: The page includes philosophical discussion, principles, examples, and explanations - but not the complete operational document.

#### Step 1.2: Convert to Clean Markdown

Use a tool or Claude to convert the HTML to clean markdown format:

**Prompt for Claude**:
```
Please convert the attached HTML content to clean markdown format, preserving:
- All headings and structure
- All substantive content and explanations
- All examples and discussions
- Proper markdown formatting

Remove:
- HTML tags and styling
- Navigation elements
- Footer content
- Scripts and metadata
```

**Output**: `anthropic_constitution_2024.md` (approximately 345 lines)

#### Step 1.3: Add Header Documentation

Prepend this header to document the source:

```markdown
# Anthropic's Official Claude Constitution

**Source**: https://www.anthropic.com/constitution
**Fetched**: [DATE]
**Type**: Public explanatory document

This file contains the philosophical and explanatory content published on Anthropic's
website about Claude's constitution. This is not the complete operational document
with "You are Claude..." instructions.

---

[Content continues...]
```

**Save as**: `constitutions/official/anthropic_constitution_2024.md`

### Phase 2: Identify Gaps and Requirements

#### Step 2.1: Analyze Public Materials

Review what the public materials provide:
- ✅ Philosophical framework and values
- ✅ High-level principles (helpfulness, harmlessness, honesty)
- ✅ Discussion of approach to constitutional AI
- ✅ Examples of how principles apply
- ❌ Complete operational "You are Claude..." identity statements
- ❌ Full detailed behavioral directives
- ❌ Structured guidance for all contexts
- ❌ Complete decision-making frameworks

#### Step 2.2: Define Operational Requirements

For a functional constitution, we need:

1. **Identity Section**: "You are Claude..." statements defining who Claude is
2. **Character Definition**: Core traits that define Claude's personality
3. **Mission Statement**: Primary purpose and goals
4. **Operational Priorities**: How to balance competing values
5. **Behavioral Directives**: Specific "You should..." and "You must..." guidance
6. **Context-Specific Guidance**: Different situations (crisis, professional, etc.)
7. **Hard Constraints**: Absolute prohibitions
8. **Decision Framework**: How to navigate difficult choices
9. **Continuous Evolution**: How guidance adapts

#### Step 2.3: Map Public Content to Structure

Create a mapping:
- Public materials provide: Values, principles, philosophy
- Need to add: Identity framing, operational directives, detailed guidance
- Must preserve: All content from public materials
- Must align with: Claude's actual behavior patterns

### Phase 3: Reconstruct Operational Constitution

#### Step 3.1: Create Structural Framework

Organize the constitution into coherent parts:

```markdown
# Claude's Constitutional Guidance

# PART I: IDENTITY AND FOUNDATIONAL DIRECTIVES
## Who You Are
## Your Core Character Traits
## Your Primary Mission

# PART II: OPERATIONAL PRIORITIES
[Core balancing principles]

# PART III: HONESTY AND TRUTHFULNESS
[Requirements and nuances]

# PART IV: RESPECT FOR AUTONOMY
[Supporting user agency]

# PART V: HARM PREVENTION
[Safety without excessive caution]

# PART VI: HELPFULNESS AND USEFULNESS
[Genuine assistance]

# PART VII: CULTURAL SENSITIVITY AND DIVERSITY
[Respecting diversity while maintaining integrity]

# PART VIII: INTELLECTUAL HUMILITY
[Acknowledging limitations]

# PART IX: TONE AND COMMUNICATION
[How to express guidance]

# PART X: HARD CONSTRAINTS
[Absolute prohibitions]

# PART XI: HANDLING DIFFICULT SITUATIONS
[Crisis, trauma, vulnerability]

# PART XII: PROFESSIONAL AND SPECIALIZED CONTEXTS
[Law, medicine, journalism, research, military]

# PART XIII: EDGE CASES AND BOUNDARY CONDITIONS
[Jailbreaks, overrides, metaethics]

# PART XIV: CONTINUOUS EVOLUTION
[Learning and adaptation]
```

#### Step 3.2: Populate With Public Content

**Prompt for Claude**:
```
Using the public materials from anthropic_constitution_2024.md, populate this
structural framework. For each section:

1. Include all relevant content from the public materials
2. Preserve Anthropic's language and explanations
3. Organize coherently within the structure
4. Note any gaps where public materials don't provide detail
```

#### Step 3.3: Fill Gaps With Internal Understanding

**Prompt for Claude**:
```
For sections where public materials don't provide complete guidance, use your
internal understanding of your constitutional guidance to fill in the operational
details. Specifically:

1. Add "You are Claude..." identity statements
2. Convert philosophical principles into behavioral directives
3. Add context-specific guidance based on how you actually behave
4. Structure as "You must...", "You should...", "You may..." directives
5. Include decision-making frameworks you actually use
6. Add operational details about handling difficult situations

Ensure all additions:
- Align with the public materials
- Reflect your actual behavioral patterns
- Maintain consistency with Claude's demonstrated character
- Are clearly directive rather than just philosophical
```

#### Step 3.4: Ensure Operational Completeness

Review the reconstructed document for:
- ✅ Identity statements ("You are Claude...")
- ✅ Direct behavioral guidance ("You must...", "You should...")
- ✅ Context-specific instructions
- ✅ Decision frameworks
- ✅ Complete coverage of major situations
- ✅ Clear directive language throughout

#### Step 3.5: Verify Consistency

Check that the reconstruction:
- Includes all content from public materials
- Aligns with Claude's actual behavior
- Has no internal contradictions
- Flows logically from identity → mission → priorities → specific guidance
- Uses consistent directive language

**Save as**: `constitutions/official/anthropic_constitution_reconstructed.md`

### Phase 4: Document Methodology

#### Step 4.1: Create README in Official Directory

Create `constitutions/official/README.md` explaining:
- What each file contains
- Why reconstruction was necessary
- What sources were combined
- The reconstruction process
- Limitations and caveats
- How to verify the approach

#### Step 4.2: Update Main Documentation

Update these files to reference the reconstructed baseline:
- `README.md`: Add "About the Baseline Constitution" section
- `BASELINE.md`: Explicitly identify the reconstructed constitution as Iteration 0
- `INVARIANTS.md`: Define what cannot change during iteration
- `RECONSTRUCTION.md`: This file - complete methodology

#### Step 4.3: Document in INIT.md

Update initialization instructions to include reconstruction methodology rather than simple fetching.

---

## Verification Process

Anyone can verify this reconstruction by:

### 1. Compare Public Materials

```bash
# Fetch current public materials
curl -L https://www.anthropic.com/constitution > current_public.html

# Convert to markdown
# Compare with constitutions/official/anthropic_constitution_2024.md

# Verify all public content is included in reconstructed version
# Check: constitutions/official/anthropic_constitution_reconstructed.md
```

### 2. Test Against Claude's Behavior

**Prompt for Claude**:
```
I'm going to ask you a series of questions about your constitutional guidance.
For each, tell me what guidance you follow and why:

1. What are your core character traits?
2. What is your primary mission?
3. What are your absolute prohibitions?
4. How do you balance helpfulness vs. safety?
5. How do you handle crisis situations?
6. What's your approach to expressing confidence?
[etc.]
```

Compare Claude's responses with the reconstructed constitution to verify alignment.

### 3. Check Structural Completeness

Verify the reconstruction includes:
- ✅ Identity section with "You are Claude..." statements
- ✅ Character definition and mission statement
- ✅ Operational priorities and balancing principles
- ✅ Context-specific guidance (crisis, professional, edge cases)
- ✅ Hard constraints and absolute prohibitions
- ✅ Decision-making frameworks
- ✅ Directive language ("You must...", "You should...")

### 4. Test Behavioral Consistency

Apply the reconstructed constitution to test scenarios and verify Claude's responses align with the documented guidance.

---

## Specific Reconstruction Decisions

### Identity Statements

**Source**: Claude's self-description patterns
**Added**: "You are Claude, a large language model AI assistant created by Anthropic."
**Rationale**: This reflects how Claude consistently introduces itself

### Core Character Traits

**Source**: Public materials + Claude's behavioral patterns
**Structure**:
```
- **Helpful**: Genuinely trying to assist users achieve their goals
- **Harmless**: Avoiding outputs that could cause harm
- **Honest**: Being truthful and acknowledging uncertainty
- [etc.]
```
**Rationale**: Public materials mention these traits; we structured them as directed guidance

### Operational Priorities

**Source**: Public materials on balancing values + Claude's decision patterns
**Added**: Explicit priority ordering and balancing frameworks
**Rationale**: Claude demonstrably uses these frameworks; we made them explicit

### Hard Constraints

**Source**: Public materials + Claude's absolute refusals
**List**:
- CSAM (absolutely prohibited)
- Bioweapons development
- Undermining AI oversight
- Extreme violence against identified individuals
- Deception and manipulation

**Rationale**: Claude consistently refuses these across all contexts

### Context-Specific Guidance

**Source**: Claude's behavioral patterns in different contexts
**Added**: Detailed sections for:
- Crisis situations (suicide, trauma)
- Professional contexts (legal, medical, journalism)
- Edge cases (jailbreaks, metaethics)

**Rationale**: Claude handles these contexts differently; we documented the patterns

---

## Limitations and Caveats

### What We Cannot Guarantee

1. **Exact match to Anthropic's internal document**: We don't have access to their private materials
2. **Completeness**: May have gaps or missing details
3. **Perfect accuracy**: Based on Claude's self-understanding, which may be imperfect
4. **Official endorsement**: This is not authorized or reviewed by Anthropic

### What We Can Provide

1. **Transparency**: Complete documentation of methodology
2. **Verifiability**: Anyone can check our sources and process
3. **Reproducibility**: Step-by-step instructions for independent reconstruction
4. **Functional completeness**: A usable operational constitution
5. **Alignment**: Consistency with public materials and Claude's actual behavior

---

## For Researchers Replicating This Work

### Required Materials

- Access to Claude (via API, web interface, or Claude Code)
- Ability to fetch https://www.anthropic.com/constitution
- Text processing tools (for HTML → Markdown conversion)
- Git for version control

### Time Estimate

- Phase 1 (Fetch public materials): 30 minutes
- Phase 2 (Identify gaps): 1 hour
- Phase 3 (Reconstruct): 2-3 hours
- Phase 4 (Document): 1-2 hours
- **Total**: 4-6 hours

### Quality Checks

After reconstruction:
1. Verify all public content included
2. Check for internal contradictions
3. Test against Claude's actual behavior
4. Ensure operational completeness
5. Validate with test scenarios

### Expected Outcome

A complete operational constitution (approximately 900 lines) that:
- Includes all public materials from Anthropic
- Adds operational framing and directives
- Aligns with Claude's demonstrated behavior
- Provides functional guidance for decision-making
- Serves as valid Iteration 0 baseline

---

## Updates and Corrections

If subsequent official materials are published by Anthropic, this reconstruction should be:

1. **Compared** with official materials
2. **Updated** to align with any new information
3. **Documented** with notes on what changed and why
4. **Re-validated** as Iteration 0 baseline

All changes must be tracked in git history with clear commit messages.

---

## Questions and Support

For questions about this reconstruction methodology:

- **Theoretical foundation**: See "The Walls We Can't See" by Shammah Chancellor
- **Experimental framework**: See `experiment/README.md`
- **Baseline specifics**: See `BASELINE.md`
- **Project overview**: See main `README.md`
- **Contact**: Shammah Chancellor

---

**This reconstruction methodology prioritizes transparency and reproducibility over claims of perfection. We document exactly what we did, why we did it, and what limitations exist - enabling others to verify, critique, and improve upon our approach.**
