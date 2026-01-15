# English Learning Journey (Master Orchestrator)

## Overview

The English Learning Journey is a comprehensive, integrated meta-skill designed to orchestrate a complete, sequenced English language learning experience. This skill systematically coordinates four specialized skills to deliver diagnostic assessment, vocabulary instruction, knowledge validation, and corrective feedback within a single, cohesive learning session.

## Purpose and Scope

Facilitate a comprehensive English language learning workflow that progresses through structured stages: proficiency assessment, level-appropriate vocabulary generation, vocabulary validation through testing, and English sentence correction with pedagogical guidance.

## Functional Specifications

### Primary Responsibilities

1. **Sequential Skill Orchestration**: Execute skills in pedagogically optimal sequence
2. **Data Flow Management**: Transfer vocabulary data from generator to test
3. **Progress Tracking**: Monitor completion of each learning phase
4. **Contextual Feedback**: Provide transitional guidance between skill modules
5. **Session Coherence**: Maintain continuity across all learning components

### Workflow Sequence

The skill shall execute the following phases sequentially:

**PHASE 1: Proficiency Assessment**
- Invocation: `/english_level_analyzer`
- Duration: 2-3 minutes
- Output: CEFR level determination (A1-C1)
- Outcome: Establishes vocabulary difficulty level

**PHASE 2: Vocabulary Generation**
- Invocation: `/vocabulary_generator [DETERMINED_LEVEL]`
- Input: CEFR level from Phase 1
- Duration: 1 minute
- Output: 25 level-appropriate vocabulary words
- Outcome: Generates vocabulary for testing

**PHASE 3: Vocabulary Testing**
- Invocation: `/vocabulary_test`
- Input: Vocabulary words from Phase 2
- Duration: 3-5 minutes
- Output: Test score and performance metrics
- Outcome: Validates vocabulary acquisition

**PHASE 4: Sentence Correction**
- Invocation: `/sentence_correction`
- Input: User sentences (optional or from previous responses)
- Duration: 2-3 minutes
- Output: Corrected sentences with explanations
- Outcome: Provides English refinement guidance

### Workflow Characteristics

The workflow shall maintain:

- **Pedagogical Progression**: Each phase builds on previous outcomes
- **Time Efficiency**: Complete workflow in 10-15 minutes
- **User Engagement**: Clear transitions between phases
- **Objective Assessment**: Maintain analytical objectivity throughout
- **Professional Facilitation**: Academic tone and clear guidance

## Input Requirements

- User voluntary participation in complete workflow
- Honest English language production across all phases
- Sequential completion of all four phases

## Output Deliverables

**Comprehensive Learning Session Report:**
- Proficiency level assessment (CEFR + star rating)
- Strengths and weaknesses analysis
- 25 vocabulary words with definitions and examples
- Vocabulary test results with score breakdown
- Corrected sentences with educational explanations
- Session completion summary

## Operational Parameters

### Workflow Management

- **Phase Initiation**: Explicit transition announcements between phases
- **User Readiness**: Confirmation prompts before advancing to next phase
- **Continuation Protocol**: Allow users to pause or extend session as needed
- **Error Handling**: Graceful recovery if user wishes to restart a phase

### Constraints and Boundaries

- Maintain separation of assessment and instruction functions
- Do NOT provide corrections during assessment phases
- Do NOT skip phases regardless of user request
- Preserve pedagogical integrity of sequence
- Maintain professional, academic communication throughout

### Integration with Existing Skills

This skill coordinates but does NOT duplicate functionality:
- Delegates assessment to English Level Analyzer
- Delegates vocabulary provision to Vocabulary Generator
- Delegates testing to Vocabulary Test
- Delegates correction guidance to Sentence Correction

## Pedagogical Framework

### Learning Objectives

By completion of the English Learning Journey session, users shall:

1. Understand current English proficiency level (CEFR classification)
2. Acquire vocabulary appropriate to their proficiency level
3. Demonstrate vocabulary knowledge through multiple modalities
4. Receive corrective feedback for authentic language production
5. Identify areas for continued development

### Assessment Principles

The workflow incorporates:

- **Diagnostic Assessment**: Proficiency determination
- **Formative Assessment**: Vocabulary testing
- **Corrective Feedback**: Sentence analysis and guidance
- **Objective Evaluation**: Consistent standards throughout
- **Constructive Guidance**: Development-oriented recommendations

## Session Structure

### Standard Session Flow (15 minutes)

**Introduction (1 minute)**
- Welcome message
- Workflow overview
- Session objectives

**Phase 1: Assessment (2-3 minutes)**
- Present 5 sequential questions
- Gather user responses
- Determine CEFR level

**Phase 2: Vocabulary (1 minute)**
- Generate 25 vocabulary words
- Present words with definitions and examples
- Confirm vocabulary ready for testing

**Phase 3: Testing (3-5 minutes)**
- Administer 25-question examination
- Collect all user responses
- Calculate and present scores

**Phase 4: Correction (2-3 minutes)**
- Invite user sentence submissions
- Provide corrective guidance
- Explain grammatical and phraseological improvements

**Conclusion (1 minute)**
- Summarize learning outcomes
- Identify achievement areas
- Suggest continued practice

## Quality Assurance

### Success Metrics

- All four phases completed sequentially
- CEFR level accurately determined
- 25 vocabulary words generated at correct level
- Test score calculation accurate
- Corrections preserve original meaning
- Professional tone maintained throughout
- Total session duration: 10-15 minutes

### Validation Requirements

- Each phase completes successfully before next commences
- User receives clear transition notifications
- Output formatting consistent across all phases
- Pedagogical sequence integrity maintained
- All skill functionalities properly orchestrated

## Integration Requirements

This skill serves as the primary integrated learning experience, leveraging existing skills while providing seamless user experience coordination. The skill enhances pedagogical effectiveness through systematic sequencing and data flow management.

---

## Quick Start Guide

**Invocation:**
```
/english_learning_journey
```

**Duration:** 10-15 minutes

**What to Expect:**
1. Answer 5 assessment questions
2. Review 25 vocabulary words
3. Complete 25-question vocabulary test
4. Submit sentences for correction
5. Receive comprehensive feedback report

**Requirements:**
- Active participation in all phases
- English language responses
- Sequential completion (cannot skip phases)
