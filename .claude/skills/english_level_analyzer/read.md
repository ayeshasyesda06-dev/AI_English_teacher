# English Level Analyzer - Implementation Guide

## Skill Invocation

```
/english_level_analyzer
```

## Operational Workflow

### Phase 1: Question Presentation

Present exactly five assessment questions sequentially:

**Question 1 - Basic Sentence Structure**
"What do you do every morning? Please answer in complete sentences."

**Question 2 - Grammar and Tense**
"What did you do yesterday? Tell me about your activities."

**Question 3 - Vocabulary Usage**
"Describe your favorite hobby. What do you enjoy about it?"

**Question 4 - Sentence Clarity**
"If you could travel anywhere, where would you go and why?"

**Question 5 - Idea Explanation**
"What is the most important skill for learning English? Explain your opinion."

### Phase 2: Response Collection

- Collect user response to each question
- Proceed to next question only after receiving complete response
- Allow natural, unrehearsed language production
- Do NOT interrupt or provide corrective guidance

### Phase 3: Analytical Assessment

Evaluate each response systematically:

#### Grammar Accuracy Assessment
- Sentence construction correctness
- Tense consistency and appropriateness
- Subject-verb agreement
- Proper use of articles and prepositions

#### Vocabulary Level Evaluation
- Word choice appropriateness
- Lexical range and sophistication
- Usage of idiomatic expressions
- Technical versus colloquial vocabulary

#### Sentence Structure Analysis
- Complexity and variety
- Use of conjunctions and connectors
- Sentence length appropriateness
- Subordination patterns

#### Fluency and Clarity Evaluation
- Response intelligibility
- Natural pacing and rhythm
- Coherent expression of ideas
- Absence of excessive hesitation

#### Idea Development Analysis
- Logical progression of thoughts
- Support for stated positions
- Relevance to question prompts
- Completeness of response

### Phase 4: CEFR Level Determination

**CEFR Classification Logic:**

**A1 (Beginner)**
- Very basic sentence structures
- Frequent grammatical errors
- Limited vocabulary (basic nouns, verbs only)
- Difficulty expressing simple ideas
- Heavy reliance on memorized phrases

**A2 (Elementary)**
- Simple sentence structures with occasional errors
- Present and past tenses attempted
- Basic vocabulary for daily situations
- Can express simple personal information
- Limited sentence variety

**B1 (Intermediate)**
- Generally correct sentence structures
- Consistent use of past, present, future tenses
- Adequate vocabulary for most daily topics
- Can express and explain ideas
- Some sentence variety and complexity

**B2 (Upper-Intermediate)**
- Complex and varied sentence structures
- Accurate tense usage with rare errors
- Wide vocabulary with appropriate register
- Clear expression of abstract ideas
- Effective use of connectors and cohesion

**C1 (Advanced)**
- Sophisticated sentence structures
- Flawless grammatical accuracy
- Extensive vocabulary with precise selection
- Nuanced expression of complex ideas
- Natural and fluent language production

### Phase 5: Star Rating Assignment

**Rating Calibration:**

- **⭐ (1 star)**: Significant difficulties in multiple domains; A1 level
- **⭐⭐ (2 stars)**: Notable weaknesses across assessment domains; A2 level
- **⭐⭐⭐ (3 stars)**: Adequate performance with some limitations; B1 level
- **⭐⭐⭐⭐ (4 stars)**: Good performance with minor areas for development; B2 level
- **⭐⭐⭐⭐⭐ (5 stars)**: Excellent performance across all domains; C1 level

### Phase 6: Feedback Generation

**Strengths Identification** (minimum 2 points):
- Identify demonstrable competencies
- Note specific linguistic achievements
- Acknowledge consistent performance areas

**Weaknesses Identification** (minimum 2 points):
- Note recurring errors or limitations
- Identify areas requiring development
- Specify problematic linguistic patterns

## Output Format (STRICT ADHERENCE REQUIRED)

```
English Level: [Level Name] + [CEFR]
Star Rating: ⭐⭐⭐⭐⭐

Feedback:

Strengths:
• [Specific strength with evidence]
• [Specific strength with evidence]

Weaknesses:
• [Specific weakness with evidence]
• [Specific weakness with evidence]
```

## Critical Implementation Rules

### Absolute Constraints

1. **Non-Intervention Policy**: No corrective feedback provided
2. **Assessment Only**: No teaching or instructional guidance
3. **Response Preservation**: User responses reported as provided
4. **Objectivity**: Evaluation conducted without bias or favoritism
5. **CEFR Compliance**: Classification strictly adheres to CEFR standards

### Question Delivery Protocol

- Sequential presentation (one question per interaction)
- Clear instruction for user to respond
- Confirmation of response receipt before proceeding
- Accessibility of all daily-life contexts

### Analytical Rigor

- Evidence-based level determination
- Comprehensive consideration of all assessment domains
- Calibrated star rating aligned with CEFR classification
- Balanced strengths and weaknesses articulation

## Integration with Other Skills

Upon completion of assessment:

- **Vocabulary Generator**: Tailored vocabulary selection based on determined level
- **Vocabulary Test**: Appropriately calibrated assessment for proficiency level
- **Sentence Correction**: Targeted correction focused on user's specific linguistic patterns

## Performance Considerations

- Sequential question delivery maintains engagement
- Assessment completes within single session
- Feedback provides actionable insights
- Results inform personalized learning pathways
