# Design Methodology: Practice Quiz Creator

## Design Goal

Create a customized multiple-choice science practice quiz and answer key for elementary students. The existing test uses fifth-grade students ages 10–11.

---

## Design Approach: Structure and Technique

**Structure I used:** R-T-F Framework (Role, Task, Format)

**Why this structure fits my task:**

- The Role identifies the teacher and intended reading level.
- The Task and Format define the topic, question count, answer choices, and answer key.

**Technique I used:** Zero-shot prompting

**Why this technique fits my task:**
Zero-shot prompting was selected because the instructions fully describe the requested quiz without requiring an example for the model to copy.


---

## Part-by-Part Justification

| Part | What I put here | Why the prompt needs it |
|------|-----------------|-------------------------|
| Role | Grade level, science-teacher role, and student age group. | Sets the audience and accessible teaching tone. |
| Task | Question count, science topic, and grade-level reading requirement. | Defines what to test and how understandable it should be. |
| Format | Four choices per question and a complete answer key. | Specifies a consistent quiz and teacher answer sheet. |

---

## Testing and Iteration

**Baseline I compared against:**
```text
Make a 3-question multiple-choice quiz about the water cycle with an answer key.
```

| Version | Result / score | What changed |
|---------|----------------|--------------|
| Naive baseline | Recorded score: 25/100 | Plain request without the designed structure or technique. |
| Version 1 | Recorded score: 100/100 | Added a teacher role, grade and age targets, and exactly four choices per question. |
| Final | Same as Version 1; no separate retest documented | No further prompt revision is recorded. This formatting update does not constitute a new test. |

**What testing showed:** Explicitly declaring the audience age, question constraints, and formatting rules improved the score by 75 points. Giving the AI a defined role prevented generic, high-level explanations and matched the vocabulary to a 5th-grade reading level.

The existing records contain one baseline and one designed run. They do not document a subsequent revision and retest. See [`examples/`](./examples/) for the saved prompts and outputs.

Existing baseline evaluation record:
- **Score:** 25/100
- **Evaluator Feedback:** The prompt lacked essential context, grade-level targets, and specific output parameters, forcing the AI to guess the target audience and depth.

Existing designed evaluation record:
- **Score:** 100/100
- **Evaluator Breakdown:**
  - Clarity & Specificity: 30/30
  - Structure & Framework Use: 30/30
  - Context & Inputs: 20/20
  - Output Requirements: 20/20
- **Evaluator Feedback:** Clean execution of the labeled R-T-F structure with actionable detail. By defining the target demographic, question count, choice parameters, and answer-sheet expectations, it removed ambiguity for the AI.


**What I learned:** The R-T-F framework was selected because educational prompts require a specific persona and clear output formatting to reach the correct reading level. By assigning a clear **Role** (5th-grade science teacher), the model adopts an encouraging, accessible tone. The **Task** specifies the topic and reading-level constraint, while the **Format** defines the question structure and answer-key requirements.

---

## Strengths and Limitations

The observations below describe the current prompt and saved example; they are not additional test results.

**Works well when:** The teacher supplies a clear science topic, grade level, age group, and question count.

**Struggles when:** The topic is broad or the teacher needs questions restricted to specific class notes. The current prompt has no input for material already taught; this is a design limitation, not a separately tested failure.

**Would improve next:** Add a way to supply material taught and restrict questions to that material, then test it.
