# Quick Validation Testing Guide - All Skills

## Overview

This guide enables rapid validation of all four English teaching skills using predefined sample data. Expected completion time: 5-10 minutes.

---

## SKILL 1: English Level Analyzer - Quick Test

**Invocation:**
```
/english_level_analyzer
```

### Test Scenario: Intermediate Level Student

**Question 1 - Basic Sentence Structure**
- *Expected prompt:* "What do you do every morning?"
- **Your Test Response:** "I wake up at 7 o'clock. I have breakfast. Then I go to school."

**Question 2 - Grammar and Tense**
- *Expected prompt:* "What did you do yesterday?"
- **Your Test Response:** "Yesterday I went to school. I studied math and science. After school, I played football with my friends."

**Question 3 - Vocabulary Usage**
- *Expected prompt:* "Describe your favorite hobby."
- **Your Test Response:** "I really enjoy playing basketball. It is a fun sport. Basketball helps me stay healthy and strong. I play with my friends every weekend."

**Question 4 - Sentence Clarity**
- *Expected prompt:* "If you could travel anywhere, where would you go and why?"
- **Your Test Response:** "I would like to travel to Japan. Japan is very beautiful. I want to see the temples and mountains. I also want to eat Japanese food."

**Question 5 - Idea Explanation**
- *Expected prompt:* "What is the most important skill for learning English?"
- **Your Test Response:** "I think listening is the most important skill. When you listen to English, you understand how native speakers speak. You learn the correct pronunciation. You also learn new vocabulary."

### Expected Output Format:
```
English Level: Intermediate (B1)
Star Rating: ⭐⭐⭐☆☆

Feedback:

Strengths:
• Demonstrates consistent past tense usage with correct verb forms
• Can construct multi-sentence responses showing idea development
• Adequate vocabulary for daily topics and explanations

Weaknesses:
• Occasional missing articles (missing "the" before some nouns)
• Limited use of complex sentence connectors
• Simple sentence structures; minimal use of subordinate clauses
```

### Validation Checklist:
- [ ] Skill asks exactly 5 questions
- [ ] Output includes CEFR level (A1-C1)
- [ ] Output includes star rating (1-5 stars)
- [ ] Strengths section has 2+ points
- [ ] Weaknesses section has 2+ points
- [ ] No grammatical corrections provided (assessment only)

---

## SKILL 2: Vocabulary Generator - Quick Test

### Test Case 1: A1 Level

**Invocation:**
```
/vocabulary_generator A1
```

**Expected Output Sample:**
```
Vocabulary List for A1 - Beginner Level

1. Word: apple
   Meaning: A round, red or green fruit that grows on trees.
   Example: I eat an apple every morning.

2. Word: happy
   Meaning: Feeling good and smiling a lot.
   Example: She is very happy today because it is her birthday.

3. Word: run
   Meaning: To move very fast with your legs.
   Example: Children run and play in the park.

...

25. Word: [25th word]
    Meaning: [Simple definition]
    Example: [Daily life context]
```

### Test Case 2: B1 Level

**Invocation:**
```
/vocabulary_generator B1
```

**Expected Output Sample:**
```
Vocabulary List for B1 - Intermediate Level

1. Word: opportunity
   Meaning: A good chance to do something you want.
   Example: I got an opportunity to study abroad next year.

2. Word: develop
   Meaning: To grow or improve something over time.
   Example: Regular practice helps you develop your English skills.

...

25. Word: [25th word]
    Meaning: [Clear definition]
    Example: [Contextual example]
```

### Validation Checklist:
- [ ] Exactly 25 words generated
- [ ] Words match specified level (A1, B1, etc.)
- [ ] All definitions are simple and clear
- [ ] All examples are from daily life contexts
- [ ] No duplicate words in list
- [ ] Consistent formatting (Word, Meaning, Example)
- [ ] Format matches STRICT specification

---

## SKILL 3: Vocabulary Test - Quick Test

**Setup:** First run Vocabulary Generator for A1 level, then test with those words.

**Invocation:**
```
/vocabulary_test
```

### Test Responses (Use sample answers below):

**SECTION 1: Multiple Choice (10 questions)**

*Expected Q1:* "What does 'happy' mean?"
- **Your Answer:** b) Feeling good and smiling a lot

*Expected Q2:* "What does 'apple' mean?"
- **Your Answer:** a) A round, red or green fruit

*Expected Q3-Q10:* [Continue answering MCQs]
- **Your Strategy:** Answer 8-9 correctly, 1-2 incorrectly (to test scoring)

**SECTION 2: Fill in the Blanks (10 questions)**

*Expected Q1:* "I eat an __________ for breakfast." (Answer: apple)
- **Your Answer:** apple

*Expected Q2:* "She is very __________ on her birthday." (Answer: happy)
- **Your Answer:** happy

*Expected Q3-Q10:* [Continue filling blanks]
- **Your Strategy:** Answer 7-8 correctly (to test scoring)

**SECTION 3: Sentence Making (5 questions)**

*Expected Q1:* "Make a sentence using the word: apple"
- **Your Answer:** "I like to eat red apples."

*Expected Q2:* "Make a sentence using the word: happy"
- **Your Answer:** "My friend is happy because she passed the test."

*Expected Q3-Q5:* [Continue making sentences]
- **Your Strategy:** Create 4 correct, 1 with potential error (to test evaluation)

### Expected Output Format:
```
Test Results:

MCQs: Correct: 8 / 10
Fill in the Blanks: Correct: 7 / 10
Sentence Making: Correct: 4 / 5

Final Score: 76%
```

### Validation Checklist:
- [ ] Exactly 25 questions presented (10+10+5)
- [ ] All 25 vocabulary words tested once
- [ ] MCQs have clear options
- [ ] Fill-in-the-blank sentences are clear
- [ ] Sentence-making prompts are unambiguous
- [ ] Score calculation is mathematically correct
- [ ] Percentages match: (19/25) × 100 = 76%
- [ ] Output format matches STRICT specification

---

## SKILL 4: Sentence Correction - Quick Test

### Test Case 1: Single Sentence with Grammar Error

**Invocation:**
```
/sentence_correction "I are going to store"
```

**Expected Output:**
```
Original: I are going to store
Corrected: I am going to the store
Explanation: Use "am" with "I", and add the article "the" before "store" in this context.
```

### Test Case 2: Multiple Sentences

**Invocation:**
```
/sentence_correction "She don't like pizza" "Yesterday I go to park"
```

**Expected Output:**
```
Correction 1:
Original: She don't like pizza
Corrected: She doesn't like pizza
Explanation: With singular subjects (she, he, it), use "doesn't" not "don't".

Correction 2:
Original: Yesterday I go to park
Corrected: Yesterday I went to the park
Explanation: Use past tense for actions that happened in the past. Also add "the" before "park".
```

### Test Case 3: Spelling Error

**Invocation:**
```
/sentence_correction "I recieved your email yesterday"
```

**Expected Output:**
```
Original: I recieved your email yesterday
Corrected: I received your email yesterday
Explanation: The correct spelling is "received" with "ei" in the middle.
```

### Test Case 4: Word Order Error

**Invocation:**
```
/sentence_correction "I like very much pizza"
```

**Expected Output:**
```
Original: I like very much pizza
Corrected: I like pizza very much
Explanation: Adverbs of degree usually come after the verb and its object.
```

### Test Case 5: Naturalness Issue

**Invocation:**
```
/sentence_correction "I am boring in mathematics"
```

**Expected Output:**
```
Original: I am boring in mathematics
Corrected: I find mathematics boring
Explanation: "Boring" describes the subject (mathematics); use "find something boring" to express your feeling about it.
```

### Validation Checklist:
- [ ] Single sentence corrections work
- [ ] Multiple sentence corrections work
- [ ] Grammar errors correctly identified
- [ ] Spelling errors correctly identified
- [ ] Word order errors correctly identified
- [ ] Naturalness issues correctly addressed
- [ ] Corrections preserve original meaning
- [ ] Explanations are simple (1-2 sentences)
- [ ] Format matches STRICT specification (Original → Corrected → Explanation)

---

## Complete Testing Workflow

### Step 1: Test English Level Analyzer (1-2 min)
```
/english_level_analyzer
[Provide 5 responses as sample data above]
```
✓ Verify output format and CEFR level

### Step 2: Test Vocabulary Generator (1 min)
```
/vocabulary_generator A1
```
✓ Verify exactly 25 words generated

### Step 3: Test Vocabulary Test (2-3 min)
```
/vocabulary_test
[Use words from Step 2]
[Provide test answers]
```
✓ Verify scoring calculation and format

### Step 4: Test Sentence Correction (1-2 min)
```
/sentence_correction "I are going"
/sentence_correction "She don't like pizza" "Yesterday I go"
/sentence_correction "I recieved email"
/sentence_correction "I like very much pizza"
/sentence_correction "I am boring"
```
✓ Verify all error types handled correctly

---

## Success Criteria

All skills pass if:

✓ **English Level Analyzer**
- Asks 5 questions sequentially
- Analyzes responses correctly
- Outputs CEFR level + star rating
- Provides 2+ strengths and 2+ weaknesses
- No corrections or teaching provided

✓ **Vocabulary Generator**
- Generates exactly 25 words
- Definitions are simple and clear
- Examples are from daily life
- Formatting is consistent
- No duplicates

✓ **Vocabulary Test**
- Creates 25 questions (10+10+5)
- Tests all vocabulary words
- Calculates score accurately
- Shows sectional breakdown
- Shows final percentage

✓ **Sentence Correction**
- Identifies grammar errors
- Identifies spelling errors
- Identifies word order errors
- Preserves meaning in corrections
- Provides simple explanations (1-2 sentences)
- Handles single and multiple corrections

---

## Quick Reference: Command Summary

```bash
# Test English Level Analyzer
/english_level_analyzer

# Test Vocabulary Generator
/vocabulary_generator A1
/vocabulary_generator B1

# Test Vocabulary Test
/vocabulary_test

# Test Sentence Correction
/sentence_correction "I are happy"
/sentence_correction "She don't like pizza" "I go to park"
/sentence_correction "I recieved email"
```

---

## Notes

- Testing should take 5-10 minutes total
- Use sample data provided above
- Verify each output matches STRICT format requirements
- Document any deviations or errors
- All skills should maintain professional, academic tone
