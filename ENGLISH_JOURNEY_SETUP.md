# English Learning Journey - Setup and Usage Guide

## Overview

You now have a complete English learning system with a master skill (`English Learning Journey`) that automatically orchestrates all four English teaching skills in the optimal pedagogical sequence.

## What Was Created

### New Master Skill: English Learning Journey

**Location:** `D:\AI_English_teacher\.claude\skills\english_learning_journey\`

**Files:**
- `skill.md` - Master skill specification
- `read.md` - Comprehensive documentation

**Purpose:** Orchestrates all four skills into one seamless learning experience

### Existing Skills (Already Available)

1. **English Level Analyzer** - Assesses your English proficiency
2. **Vocabulary Generator** - Creates 25-word vocabulary lists
3. **Vocabulary Test** - Tests vocabulary knowledge
4. **Sentence Correction** - Identifies and corrects English errors

---

## How to Use

### Option 1: Run Manually (Recommended for First Use)

Simply invoke the master skill:

```
/english_learning_journey
```

**What happens:**
1. Answers 5 assessment questions (you provide English responses)
2. Automatic vocabulary generation based on your level
3. Vocabulary test with 25 questions
4. Sentence correction with explanations
5. Complete feedback report

**Duration:** 10-15 minutes

**No preparation needed - just type the command and follow prompts**

---

### Option 2: Automatic Startup (Optional)

To run the English Learning Journey automatically whenever you open your Claude Code project, follow these steps:

#### Step 1: Locate Your Claude Settings

**On Windows:**
```
%APPDATA%\claude\settings.json
```

Or:
```
C:\Users\[YourUsername]\AppData\Roaming\claude\settings.json
```

#### Step 2: Add Hook Configuration

Open `settings.json` and add this configuration:

```json
{
  "hooks": {
    "on_open": "/english_learning_journey"
  }
}
```

**Complete example settings.json:**
```json
{
  "cwd": "D:\\AI_English_teacher",
  "model": "claude-opus-4-5",
  "hooks": {
    "on_open": "/english_learning_journey"
  }
}
```

#### Step 3: Save and Restart

1. Save the settings.json file
2. Close Claude Code completely
3. Reopen Claude Code
4. The English Learning Journey will start automatically

#### Step 4: Verify It's Working

You should see the welcome message:
```
Welcome to your English Learning Journey!

This comprehensive learning session will:
1. Assess your English proficiency level (2-3 minutes)
2. Generate vocabulary for your level (1 minute)
3. Test your vocabulary knowledge (3-5 minutes)
4. Correct your English sentences (2-3 minutes)
5. Provide complete feedback report
```

---

## Complete Session Workflow

### Phase 1: English Level Analyzer (2-3 minutes)

Claude asks exactly 5 questions:

1. "What do you do every morning?"
2. "What did you do yesterday?"
3. "Describe your favorite hobby."
4. "If you could travel anywhere, where would you go and why?"
5. "What is the most important skill for learning English?"

**Your task:** Answer in English as naturally as possible.

**Output:** Your proficiency level (A1-C1 on CEFR scale) + star rating

---

### Phase 2: Vocabulary Generation (1 minute)

Claude generates 25 vocabulary words matched to your proficiency level.

**Example output:**
```
Vocabulary List for B1 - Intermediate Level

1. Word: opportunity
   Meaning: A good chance to do something you want.
   Example: I got an opportunity to study abroad next year.

2. Word: develop
   Meaning: To grow or improve something over time.
   Example: Regular practice helps you develop your English skills.

[... continues to word 25]
```

**Your task:** Review and memorize the vocabulary words.

---

### Phase 3: Vocabulary Test (3-5 minutes)

Claude administers a 25-question test in three sections:

**Section 1: Multiple Choice (10 questions)**
```
Question 1: What does "opportunity" mean?
a) A problem you must solve
b) A good chance to do something you want
c) A difficult situation
```

**Section 2: Fill in the Blank (10 questions)**
```
Question 1: I got an __________ to study abroad.
(Answer: opportunity)
```

**Section 3: Sentence Making (5 questions)**
```
Question 1: Make a sentence using the word "opportunity"
(Your answer: I was given an opportunity to learn French.)
```

**Your task:** Answer all 25 questions.

**Output:** Test score with breakdown:
```
MCQs: 8 / 10
Fill in the Blanks: 7 / 10
Sentence Making: 4 / 5

Final Score: 76%
```

---

### Phase 4: Sentence Correction (2-3 minutes)

Claude corrects English sentences with explanations.

**Example:**
```
Original: I are happy very much
Corrected: I am very happy
Explanation: Use "am" with "I". Place adverbs before adjectives or after the verb.

Original: She go to school yesterday
Corrected: She went to school yesterday
Explanation: Use past tense for actions that happened in the past.
```

**Your task:** Submit sentences for correction, or allow Claude to use your answers from Phase 1.

**Output:** Corrected sentences with explanations for each error.

---

### Phase 5: Session Summary (1 minute)

Claude provides comprehensive feedback:

```
English Learning Journey - Session Summary

✓ COMPLETED:
  1. English Proficiency Assessment
  2. Vocabulary Generation (25 words)
  3. Vocabulary Testing (76% score)
  4. Sentence Correction (5 corrections)

YOUR PROGRESS:
  Current Level: B1 (Intermediate)
  Strengths: Consistent verb usage, good vocabulary range
  Areas for Development: Complex sentence structures, articles

RECOMMENDATIONS:
  - Practice subordinate clause construction
  - Learn phrasal verbs at your level
  - Focus on article usage
  - Continue daily practice

Next Steps: Run again next week to track progress!
```

---

## Quick Reference: All Commands

### Master Skill (Recommended)
```
/english_learning_journey
```
Runs all 4 skills in sequence (10-15 minutes)

### Individual Skills (For Focused Practice)

**English Level Analyzer**
```
/english_level_analyzer
```

**Vocabulary Generator**
```
/vocabulary_generator A1
/vocabulary_generator A2
/vocabulary_generator B1
/vocabulary_generator B2
/vocabulary_generator C1
```

**Vocabulary Test**
```
/vocabulary_test
```

**Sentence Correction**
```
/sentence_correction "I are happy"
/sentence_correction "She don't like pizza" "I go to park"
```

**Skill Maker (Create Custom Skills)**
```
/skill_maker
```

---

## Recommended Usage Schedule

### Weekly Plan
- **Monday:** Run `/english_learning_journey` for comprehensive assessment
- **Tuesday-Thursday:** Use individual skills for focused practice
- **Friday:** Run `/vocabulary_generator` + `/vocabulary_test` for reinforcement
- **Weekend:** Review vocabulary and practice speaking

### Monthly Plan
- **Week 1:** Establish baseline with English Learning Journey
- **Weeks 2-3:** Focused practice on weaknesses identified in Week 1
- **Week 4:** Run English Learning Journey again to measure progress

### Progression
- When consistently scoring 85%+ on vocabulary tests → advance to next CEFR level
- When proficiency assessment shows improvement → move up to B1, B2, C1 vocabulary

---

## Tips for Best Results

### During Assessment (Phase 1)
- Answer naturally without overthinking
- Don't translate from another language
- Provide complete sentences
- Take your time, think about your responses

### Vocabulary Learning (Phase 2)
- Write down the vocabulary list
- Create your own sentences with each word
- Practice saying the words aloud
- Review the list for 5-10 minutes before testing

### Vocabulary Testing (Phase 3)
- Don't use dictionaries or translation tools
- Rely on your memory and understanding
- It's okay to guess if unsure
- This is honest assessment, not a performance test

### Sentence Correction (Phase 4)
- Submit real sentences you've written
- Don't create perfect sentences (nothing to correct)
- Include sentences with errors you're unsure about
- Pay attention to the explanations

---

## Troubleshooting

### "Command not found: english_learning_journey"
**Solution:** Ensure the skill files are in the correct location:
```
D:\AI_English_teacher\.claude\skills\english_learning_journey\
├── skill.md
└── read.md
```

### Automatic startup isn't working
**Solution:**
1. Verify settings.json location is correct
2. Check JSON syntax (proper quotes, brackets)
3. Restart Claude Code completely (not just refresh)
4. Try manual command first: `/english_learning_journey`

### Vocabulary test seems too easy/hard
**Solution:**
- Too easy? Advance to next CEFR level: `/vocabulary_generator B1`
- Too hard? Go back one level: `/vocabulary_generator A2`

### Not seeing expected output format
**Solution:**
- The skills should display consistently
- If formatting looks different, verify skill files are complete
- Run skills individually first to test each one

---

## Next Steps

### To Begin Your English Learning Journey:

1. **Right now:** Type `/english_learning_journey` and follow the prompts
2. **First session:** Complete all 5 phases (10-15 minutes)
3. **Review results:** Analyze your proficiency level and weaknesses
4. **Plan practice:** Focus on identified areas for improvement
5. **Weekly routine:** Run the journey every week to track progress

### Files You Now Have:

**Master Skill:**
- `/skills/english_learning_journey/skill.md`
- `/skills/english_learning_journey/read.md`

**Existing Skills:**
- `/skills/english_level_analyzer/`
- `/skills/vocabulary_generator/`
- `/skills/vocabulary_test/`
- `/skills/sentence_correction/`
- `/skills/skill_maker/`

**Documentation:**
- `/TESTING_GUIDE.md` - Detailed testing procedures
- `/ENGLISH_JOURNEY_SETUP.md` - This file
- `/CLAUDE.md` - Professional communication guidelines

---

## Summary

You now have a complete, professional English learning system:

✓ **English Level Analyzer** - Diagnoses proficiency level
✓ **Vocabulary Generator** - Creates level-appropriate word lists
✓ **Vocabulary Test** - Validates vocabulary knowledge
✓ **Sentence Correction** - Provides grammar and correction guidance
✓ **English Learning Journey** - Master skill that orchestrates everything

**Start now:** Type `/english_learning_journey` to begin your first comprehensive English learning session!

**Estimated time:** 10-15 minutes

**What you'll receive:** Complete proficiency assessment, 25 vocabulary words, test results, and corrective feedback.

Good luck with your English learning!
