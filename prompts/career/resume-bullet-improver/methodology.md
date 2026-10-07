# Design Methodology: Resume Bullet Improver

## Design Goal

Help a high school student applying for a part-time job turn a basic work-experience statement into concise, professional resume bullets without inventing details.

---

## Design Approach: Structure and Technique

**Structure I used:** C-A-R-E Framework (Context, Action, Result, Example)

**Why this structure fits my task:**

- Context supplies the applicant's experience, and Action defines the requested improvement.
- Result sets output limits, while Example demonstrates the desired writing style.

**Technique I used:** Few-shot prompting

**Why this technique fits my task:**
Few-shot prompting was selected because the included weak-to-strong example gives the model a pattern to follow. This helps produce concise, action-oriented writing without requiring the model to guess the desired style.


---

## Part-by-Part Justification

| Part | What I put here | Why the prompt needs it |
|------|-----------------|-------------------------|
| Context | Applicant description, target job, original bullet, and actual responsibilities. | Provides the facts and intended employer context. |
| Action | A stronger bullet with a strong action verb and no invented details. | Defines the improvement and accuracy guardrails. |
| Result | Three options, one sentence each, under 30 words, with a natural professional tone. | Sets measurable output requirements. |
| Example | A weak-to-strong lawn-care bullet. | Demonstrates the intended pattern and style. |

---

## Testing and Iteration

**Baseline I compared against:**
```text
Improve this resume bullet: Detailed cars for customers.
```

| Version | Result / score | What changed |
|---------|----------------|--------------|
| Naive baseline | Recorded score: 25/100 | Plain request without the designed structure or technique. |
| Version 1 | Recorded score: 100/100 | Added applicant background, actual duties, accuracy rules, three-option output, a word limit, and a worked example. |
| Final | Same as Version 1; no separate retest documented | No further prompt revision is recorded. This formatting update does not constitute a new test. |

**What testing showed:** Adding the applicant's background, actual responsibilities, output count, word limit, tone, and example improved the score by 75 points. The designed prompt produced three concise bullets that accurately highlighted independence, scheduling, customer communication, and detailing experience.

The existing records contain one baseline and one designed run. They do not document a subsequent revision and retest. See [`examples/`](./examples/) for the saved prompts and outputs.

Existing baseline evaluation record:
- **Score:** 25/100
- **Rubric Breakdown:**
  - Clarity & Specificity: 15/30
  - Structure & Framework Use: 0/30
  - Context & Inputs: 10/20
  - Output Requirements: 0/20
- **Evaluator Feedback:** The task was understandable, but it lacked a framework, job context, responsibility details, and requirements for tone, length, or output structure.

Existing designed evaluation record:
- **Score:** 100/100
- **Rubric Breakdown:**
  - Clarity & Specificity: 30/30
  - Structure & Framework Use: 30/30
  - Context & Inputs: 20/20
  - Output Requirements: 20/20
- **Evaluator Feedback:** The complete C-A-R-E framework supplied relevant background and strict constraints. The example demonstrated the intended style, while the accuracy guardrail prevented invented metrics or responsibilities.


**What I learned:** The C-A-R-E framework was selected because resume writing requires both personal background and strict output rules. The **Context** supplies the applicant's experience and original bullet. The **Action** explains how the bullet should be improved. The **Result** sets the number, tone, and length of the responses. The **Example** demonstrates the expected style.

---

## Strengths and Limitations

The observations below describe the current prompt and saved example; they are not additional test results.

**Works well when:** The applicant supplies actual responsibilities and a target job.

**Struggles when:** Responsibility details are vague. The lawn-care example also includes scheduling and communication that the weak example alone does not establish; the model could copy unsupported details.

**Would improve next:** Give the example its own factual background and test that unrelated example details do not appear in the applicant's bullets.
