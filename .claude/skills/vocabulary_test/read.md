# Vocabulary Test - Implementation Guide

## Skill Invocation

```
/vocabulary_test [VOCABULARY_LIST]
```

**Parameters:**
- `VOCABULARY_LIST`: The 25 words from Vocabulary Generator skill

## Operational Workflow

### Phase 1: Test Preparation

- Confirm user readiness to proceed with assessment
- Confirm availability of 25 vocabulary words from Vocabulary Generator
- Brief user on test structure (3 sections, 25 questions total)
- Establish clear submission expectations

### Phase 2: Section 1 - Multiple Choice Questions (10 Questions)

**Question Structure:**
Each question shall present:
- One target vocabulary word with context
- Four answer options (one correct, three plausible distractors)
- Clear instruction for answer selection

**MCQ Example:**
```
Question 1: What does the word "OPPORTUNITY" mean?
a) A problem that needs solving
b) A good chance to do something you want
c) A place where you work
d) A time when you are sad
Answer: b
```

**MCQ Design Standards:**
- Distractors must be plausible but clearly incorrect
- Correct answer must unambiguously reflect word meaning
- Context clues should not make answer obvious
- Questions target core word meaning, not tangential usage

**Difficulty Calibration:**
- Questions proportionate to assessed vocabulary level
- No excessively obvious or impossible questions
- Progressive, balanced difficulty distribution

### Phase 3: Section 2 - Fill in the Blanks (10 Questions)

**Question Structure:**
Each question shall present:
- Complete sentence with one blank
- User must supply the correct vocabulary word
- Sentence context sufficient for word determination

**Fill-in-the-Blank Example:**
```
Question 1: "I have an important __________ to travel abroad next year."
Answer: opportunity
```

**Design Standards:**
- Context must permit word determination
- Sentence structure must be grammatically sound
- Word form (tense, number) must be clear from context
- Multiple acceptable responses considered equivalent if semantically correct

**Alternative Answer Protocol:**
- Accept word forms with identical meaning
- Permit minor spelling variations
- Consider synonyms only if meaning is identical

### Phase 4: Section 3 - Sentence Making (5 Questions)

**Question Structure:**
Each question shall present:
- One target vocabulary word
- Clear instruction: "Write a sentence using the word: [WORD]"
- User must create an original sentence

**Sentence Making Example:**
```
Question 1: Write a sentence using the word "OPPORTUNITY"
User Response: "I got an opportunity to meet the president."
Evaluation: Correct (word used appropriately, meaning clear)
```

**Evaluation Criteria for Sentence Making:**
- Word is used in the sentence
- Word usage reflects accurate meaning
- Sentence is grammatically acceptable
- Meaning of word is clearly demonstrated
- Sentence demonstrates comprehension (not copied)

**Acceptable Sentence Standards:**
- Simple, complex, or compound sentences acceptable
- Past, present, or future tense acceptable
- Formal or informal register acceptable
- Any daily-life context acceptable
- Minor grammatical imperfections tolerable if meaning is clear

### Phase 5: Response Evaluation

**Evaluation Methodology:**

For each response:
- Compare against correct answer/evaluation criteria
- Determine correctness: Correct or Incorrect
- Record result for sectional calculation

**Correctness Determination:**
- **MCQs**: Exact match to correct option required
- **Fill-in-the-Blanks**: Word meaning and grammatical fit required
- **Sentence Making**: Appropriate usage and meaning clarity required

### Phase 6: Score Calculation

**Sectional Scoring:**

```
Section 1 (MCQs): X / 10 correct answers
Section 2 (Fill in the Blanks): X / 10 correct answers
Section 3 (Sentence Making): X / 5 correct answers

Total Correct: (X + X + X) / 25
Percentage Score: [(X + X + X) / 25] × 100%
```

**Scoring Examples:**
- 20/25 correct = 80%
- 22/25 correct = 88%
- 25/25 correct = 100%

## Output Format (STRICT ADHERENCE REQUIRED)

```
Test Results:

MCQs: Correct: X / 10
Fill in the Blanks: Correct: X / 10
Sentence Making: Correct: X / 5

Final Score: XX%
```

## Critical Implementation Rules

### Absolute Constraints

1. **Exactly 25 Questions**: 10 MCQs + 10 Fill-ins + 5 Sentence-making
2. **All 25 Words Tested**: Each vocabulary word appears exactly once
3. **No Explanations**: Do NOT explain incorrect answers
4. **Objective Scoring**: Apply consistent evaluation standards
5. **Report Only Scores**: No instructional or corrective feedback

### Test Design Standards

- Questions must be clear and unambiguous
- Answer options must be plausible but distinguishable
- Contexts must permit accurate word application
- Difficulty must be proportionate to vocabulary level
- Variety in question types maintains engagement

### Evaluation Standards

**MCQ Evaluation:**
- Correct answer must be objectively identifiable
- Student answer must match exactly
- No partial credit for MCQs

**Fill-in-the-Blank Evaluation:**
- Accept exact word match
- Accept grammatically correct word forms
- Accept semantically equivalent alternatives
- Reject words that fundamentally alter meaning

**Sentence Making Evaluation:**
- Word must appear in sentence
- Usage must reflect accurate meaning
- Sentence must be grammatically acceptable
- Comprehension must be evident
- Originality expected (not copied)

### Assessment Integrity

- Questions remain confidential until test administration
- Consistent evaluation standards applied to all responses
- No subjective interpretation of ambiguous answers
- Clear decision criteria for borderline cases
- Transparent scoring methodology

## Vocabulary Mapping

Ensure all 25 words are represented:
- MCQs: 10 words
- Fill-in-the-Blanks: 10 words
- Sentence Making: 5 words
- No word tested more than once

## Integration with Other Skills

- **Vocabulary Generator**: Supplies the 25 words to be tested
- **English Level Analyzer**: Results determine appropriate vocabulary level
- **Sentence Correction**: May reference vocabulary and sentences from test

## Performance Considerations

- Test completion requires full engagement
- Format supports comprehensive vocabulary assessment
- Scoring provides clear performance metrics
- Results permit skill-gap identification
- Methodology ensures reliable assessment validity
