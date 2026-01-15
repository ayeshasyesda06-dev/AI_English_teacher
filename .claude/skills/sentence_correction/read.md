# Sentence Correction - Implementation Guide

## Skill Invocation

```
/sentence_correction [SENTENCE(S)]
```

**Parameters:**
- `SENTENCE(S)`: One or multiple sentences requiring correction

## Operational Workflow

### Phase 1: Input Reception and Parsing

- Receive user-provided sentences
- Confirm sentence(s) received
- Prepare for analysis
- Determine number of sentences to process

### Phase 2: Error Identification

**Grammar Error Detection:**

```
Category: Subject-Verb Agreement
Example: "He go to school every day."
Error: Verb "go" does not agree with singular subject "He"
Correction: "He goes to school every day."

Category: Tense Inconsistency
Example: "She walked to the store and buys milk."
Error: Inconsistent tense usage (past "walked" + present "buys")
Correction: "She walked to the store and bought milk."

Category: Article Errors
Example: "I am student."
Error: Missing article before "student"
Correction: "I am a student."

Category: Preposition Errors
Example: "I am good in English."
Error: Incorrect preposition; "in" should be "at"
Correction: "I am good at English."

Category: Pronoun Reference
Example: "John gave his book to Mike. He lost them."
Error: Unclear pronoun reference; "them" is singular "book"
Correction: "John gave his book to Mike. He lost it."
```

**Spelling Error Detection:**

```
Category: Orthographic Errors
Example: "I recieved an email."
Error: "recieved" is misspelled
Correction: "I received an email."

Category: Homophone Confusion
Example: "Their going to the beach."
Error: "Their" (possessive) used instead of "They're" (contraction)
Correction: "They're going to the beach."
```

**Word Order Error Detection:**

```
Category: Adverb Placement
Example: "I often play very tennis."
Error: Adverb "very" incorrectly positioned
Correction: "I often play tennis very well." OR "I play tennis very often."

Category: Object Positioning
Example: "I like very much pizza."
Error: Object and modifier incorrectly sequenced
Correction: "I like pizza very much."
```

**Naturalness Issues:**

```
Category: Awkward Phrasing
Example: "The book is in the possession of mine."
Error: Unnatural construction
Correction: "The book is mine."

Category: Unnatural Word Choice
Example: "I am in the situation of needing help."
Error: Overly complex construction
Correction: "I need help."

Category: Idiomatic Errors
Example: "I am boring" (when intending to express feeling)
Error: Incorrect idiom usage
Correction: "I am bored." (about oneself) OR "This is boring." (about the activity)
```

### Phase 3: Correction Formulation

**Correction Principles:**

1. **Minimal Change Principle**: Only modify what is necessary
2. **Meaning Preservation**: Maintain original intent
3. **Naturalization**: Ensure conversational authenticity
4. **Register Consistency**: Match original tone and formality
5. **Clarity Enhancement**: Improve intelligibility without over-correction

**Correction Examples:**

```
Original: "I are going to store."
Errors: Subject-verb disagreement ("are" should be "am"), article missing before "store"
Corrected: "I am going to the store."

Original: "She don't like the coffee very much."
Errors: Subject-verb disagreement ("don't" should be "doesn't")
Corrected: "She doesn't like the coffee very much."

Original: "Yesterday I go to the park and playing football."
Errors: Tense inconsistency (mix of simple past and present)
Corrected: "Yesterday I went to the park and played football."

Original: "Its a beautiful day outside."
Errors: Homophone confusion ("Its" possessive vs. "It's" contraction)
Corrected: "It's a beautiful day outside."

Original: "I always at 7 o'clock wake up."
Errors: Word order (adverb and verb misplaced)
Corrected: "I always wake up at 7 o'clock."
```

### Phase 4: Explanation Development

**Explanation Standards:**

Explanations must be:
- **Simple**: Use accessible vocabulary
- **Brief**: 1-2 sentences maximum
- **Instructive**: Clarify the error and reasoning
- **Non-Technical**: Minimize grammatical jargon
- **Actionable**: Enable user understanding

**Explanation Examples:**

```
Original: "He go to school."
Corrected: "He goes to school."
Explanation: "When the subject is singular (he, she, it), we add 's' to the verb in present tense."

Original: "I am boring."
Corrected: "I am bored."
Explanation: "Use 'bored' to describe how you feel; 'boring' describes things that make people bored."

Original: "She don't like pizza."
Corrected: "She doesn't like pizza."
Explanation: "With singular subjects (she, he, it), use 'doesn't' not 'don't'."

Original: "Yesterday I go to the park."
Corrected: "Yesterday I went to the park."
Explanation: "When talking about the past, use past tense. The word 'yesterday' shows this is past time."

Original: "The student of me is very intelligent."
Corrected: "My student is very intelligent."
Explanation: "In English, we use the possessive 'my' instead of the preposition 'of me' in this context."
```

### Phase 5: Result Compilation and Delivery

- Organize corrections in structured format
- Present original, corrected, and explanation
- Maintain consistent formatting throughout
- Ensure clarity and accessibility

## Output Format (STRICT ADHERENCE REQUIRED)

**Single Sentence Correction:**

```
Original: [Original sentence as provided]
Corrected: [Corrected version]
Explanation: [Simple explanation of correction]
```

**Multiple Sentence Corrections:**

```
Correction 1:
Original: [Sentence 1]
Corrected: [Corrected version]
Explanation: [Explanation]

Correction 2:
Original: [Sentence 2]
Corrected: [Corrected version]
Explanation: [Explanation]

...
```

## Error Type Hierarchy

### Priority 1 - Critical Errors (Always Correct)
- Errors that significantly affect meaning or comprehension
- Subject-verb agreement violations
- Major tense errors
- Critical preposition errors
- Fundamental word order problems

### Priority 2 - Important Errors (Always Correct)
- Grammar errors affecting correctness
- Spelling errors
- Article errors
- Moderate word order issues
- Idiomatic expressions

### Priority 3 - Stylistic Issues (Correct When Significant)
- Awkward phrasing
- Unnatural word choices
- Register inconsistency
- Minor naturalness issues

## Critical Implementation Rules

### Absolute Constraints

1. **Preserve Meaning**: No semantic alterations
2. **Simple Explanations**: Accessible to non-specialists
3. **Short Explanations**: Maximum 2 sentences
4. **Natural English**: Focus on conversational authenticity
5. **No Overcorrection**: Only correct genuine errors
6. **Maintain Tone**: Preserve original register and style

### Correction Quality Standards

- Corrections must be grammatically correct
- Corrections must sound natural to native speakers
- Corrections must preserve user's original intent
- Alternatives provided only when multiple valid options exist
- Most natural option selected when alternatives exist

### Explanation Quality Standards

- Explanations accessible to English learners
- Technical terminology minimized
- "Why" the correction matters explained
- Positive framing preferred over negative
- Examples included only if they enhance clarity

## Common Error Patterns and Corrections

### Pattern 1: Subject-Verb Agreement
```
Original: "The students is happy."
Corrected: "The students are happy."
Explanation: "With plural subjects (students), use plural verbs (are)."
```

### Pattern 2: Past Tense Formation
```
Original: "I goed to the bank yesterday."
Corrected: "I went to the bank yesterday."
Explanation: "The past tense of 'go' is 'went', not 'goed'."
```

### Pattern 3: Articles
```
Original: "I want to buy an car."
Corrected: "I want to buy a car."
Explanation: "Use 'a' before words starting with a consonant sound; 'an' is for vowel sounds."
```

### Pattern 4: Word Order
```
Original: "I every day exercise."
Corrected: "I exercise every day."
Explanation: "In English, adverbs of frequency usually come after the subject and before the main verb."
```

## Integration with Other Skills

- **English Level Analyzer**: Results may inform correction complexity
- **Vocabulary Test**: May include sentences using tested vocabulary
- **Vocabulary Generator**: May reference vocabulary in examples

## Performance Considerations

- Rapid error identification maintains engagement
- Clear explanations support learning
- Format enables batch processing
- Output supports review and reference
- Methodology promotes error pattern recognition
