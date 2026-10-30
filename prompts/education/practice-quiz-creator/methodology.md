# Design Methodology: Practice Quiz Creator

## Design Goal

Make a science quiz and answer key that fit the students' grade and age. The original saved test used fifth grade students ages 10 and 11.

---

## Design Approach: Structure and Technique

**Structure I used:** RTF: Role, Task, Format

**Why this structure fits my task:**

- Role tells the AI who it is helping and the students' ages.
- Task and Format explain the topic, question count, choices, and answer key.

**Technique I used:** Zero shot: gives instructions without an example.

**Why this technique fits my task:**
The request is simple enough to explain without showing a sample quiz.

---

## Part by Part Justification

| Part | What I put here | Why the prompt needs it |
|---|---|---|
| Role | Teacher role, grade, and student age. | Helps the AI choose words that fit the class. |
| Task | Topic, number of questions, and reading level. | Tells the AI what quiz to make. |
| Format | Four choices per question and an answer key. | Tells the AI how to lay out the answer. |

---

## Testing and Iteration

These scores belong to the original prompts saved in [`examples/output_comparison.md`](./examples/output_comparison.md). The simpler wording in the current prompt has not been tested. The [original notes](./examples/original-methodology.md) keep the earlier scores and feedback.

**Baseline I compared against:**

```text
Make a 3-question multiple-choice quiz about the water cycle with an answer key.
```

| Version | Result / score | What changed |
|---|---|---|
| Naive baseline | Original recorded score: 25/100 | A plain request. |
| Version 1 | Original recorded score: 100/100 | Added the teacher role, student grade and age, and four choices per question. |
| Final | Current wording has no new score | The wording was made simpler. No new test is claimed. |

**What testing showed:** The original records list 25/100 for the basic request and 100/100 for the prompt with labeled parts. The saved quiz adds examples to its questions and explanations to the answer key.

Original basic prompt scores:

The original file did not include scores for each category of the basic prompt. They have not been filled in from its total.

Original designed prompt scores:

| Category | Designed prompt |
|---|---:|
| Clarity & Specificity | 30/30 |
| Structure & Framework Use | 30/30 |
| Context & Inputs | 20/20 |
| Output Requirements | 20/20 |

**What I learned:** The Role part sets the audience. The Task part sets the topic and reading level. The Format part explains the questions and answer key.

---

## Strengths and Limitations

These points describe the prompt and saved example. They are not extra test results.

**Works well when:** The teacher gives a clear topic, grade, age, and question count.

**Struggles when:** A broad topic can include things the students have not learned. The original prompt does not take class notes.

**Would improve next:** Let the teacher add class notes and limit the quiz to those notes.
