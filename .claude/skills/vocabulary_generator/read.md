# Vocabulary Generator - Implementation Guide

## Skill Invocation

```
/vocabulary_generator [CEFR_LEVEL]
```

**Parameters:**
- `CEFR_LEVEL`: One of A1, A2, B1, B2, or C1

## Operational Workflow

### Phase 1: Input Validation

- Verify CEFR level specification (A1, A2, B1, B2, or C1)
- Confirm user comprehension of task parameters
- Clarify context or domain preferences if applicable

### Phase 2: Vocabulary Selection

**A1 (Beginner) Level Criteria:**
- Basic, high-frequency words
- Simple, everyday objects and activities
- Present tense focused vocabulary
- Words requiring no contextual knowledge
- Examples: apple, house, happy, run, sleep

**A2 (Elementary) Level Criteria:**
- Expanded everyday vocabulary
- Simple descriptive terms
- Basic past/future temporal vocabulary
- Common daily activities
- Examples: morning, friend, important, travel, remember

**B1 (Intermediate) Level Criteria:**
- More varied vocabulary
- Abstract concept vocabulary
- Moderately complex descriptions
- Diverse semantic fields
- Examples: opportunity, develop, strategy, community, experience

**B2 (Upper-Intermediate) Level Criteria:**
- Sophisticated vocabulary
- Nuanced expressions
- Idiomatic usage
- Professional and academic vocabulary
- Examples: sophisticated, elaborate, significant, advocate, consequently

**C1 (Advanced) Level Criteria:**
- Advanced vocabulary
- Precise, sophisticated terminology
- Rare but useful words
- Semantic nuance and distinction
- Examples: meticulous, eloquent, fortuitous, ubiquitous, pragmatic

### Phase 3: Definition Formulation

**Simplification Requirements:**

For each word, create definition following standards:

- **A1 Definitions**: Single, basic sentence; use only high-frequency words
- **A2 Definitions**: Simple sentence; use A1+ vocabulary
- **B1 Definitions**: Complete but straightforward; basic subordination acceptable
- **B2 Definitions**: Clear and specific; some sophistication permitted
- **C1 Definitions**: Precise and nuanced; professional terminology acceptable

**Definition Examples:**

```
A1: "happy" - When you feel good and smile a lot.
A2: "important" - Something that matters very much; it's very necessary.
B1: "opportunity" - A good chance to do something you want.
B2: "meticulous" - Very careful and paying attention to small details.
C1: "pragmatic" - Based on practical considerations; dealing with things in a realistic way.
```

### Phase 4: Example Sentence Creation

**Natural Usage Requirements:**

- Sentences must reflect authentic daily conversation
- Context must be immediately comprehensible
- Vocabulary usage must appear organic, not forced
- Permit learner visualization of practical application

**Example Sentence Standards:**

```
A1: "I like to drink coffee in the morning." (Simple subject-verb-object)
A2: "She travels to her office by bus every day." (Basic routine expression)
B1: "This job offers a good opportunity to develop new skills." (Contextual placement)
B2: "The architect's meticulous attention to detail ensured a flawless design." (Professional context)
C1: "The pragmatic approach to resolving the dispute proved far more effective than litigation." (Sophisticated context)
```

### Phase 5: List Organization

Structure output in consistent format:

- Sequential ordering (1-25)
- Parallel formatting for each entry
- Clear visual separation between words
- Consistent definition and example structure

## Output Format (STRICT ADHERENCE REQUIRED)

```
Vocabulary List for [LEVEL] - [CEFR]

1. Word: [Word]
   Meaning: [Simple definition]
   Example: [Natural usage sentence]

2. Word: [Word]
   Meaning: [Simple definition]
   Example: [Natural usage sentence]

...

25. Word: [Word]
    Meaning: [Simple definition]
    Example: [Natural usage sentence]
```

## Critical Implementation Rules

### Absolute Constraints

1. **Exactly 25 Words**: No more, no fewer
2. **Simple Definitions**: Understandable at specified proficiency level
3. **Daily Life Context**: All examples from practical, relatable scenarios
4. **No Grammatical Explanation**: Focus on meaning only
5. **No Testing**: Assessment function prohibited
6. **No Teaching**: Instructional guidance prohibited

### Vocabulary Quality Standards

- All words suitable for daily conversation
- No obscure, highly technical, or archaic vocabulary
- Diverse semantic categories represented
- Level-appropriate complexity throughout
- Useful for practical language application

### Definition Quality Standards

- Definitions must be comprehensible
- Avoid circular definitions
- Permit word understanding without context
- One sentence maximum per definition
- Use accessible vocabulary in definitions

### Example Quality Standards

- Sentences must be natural and conversational
- Context must be immediately clear
- Vocabulary integration must appear organic
- Examples must permit practical visualization
- Variety in sentence structure and contexts

## Vocabulary Distribution Guidelines

For balanced list compilation:

- **Common Verbs**: 6-8 words
- **Essential Nouns**: 6-8 words
- **Descriptive Adjectives**: 4-5 words
- **Adverbs and Expressions**: 3-4 words
- **Practical Phrases/Concepts**: 2-3 words

## Integration with Other Skills

Upon vocabulary generation completion:

- **Vocabulary Test**: Uses generated vocabulary for assessment
- **English Level Analyzer**: Results inform vocabulary level selection
- **Sentence Correction**: May reference vocabulary from generated lists

## Performance Considerations

- Word selection must prioritize practical utility
- Definition clarity enables independent learning
- Examples facilitate memorable association
- Format supports easy review and reference
- Lists optimized for learner retention and application
