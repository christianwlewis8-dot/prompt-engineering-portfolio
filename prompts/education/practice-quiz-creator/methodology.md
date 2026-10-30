# Design Methodology: Practice Quiz Creator

## Design Goal

Help elementary school teachers make quizzes from what their students have learned. The teacher chooses the topic, grade, question type, and number of questions, and gets a simple answer sheet.

---

## Design Approach: Structure and Technique

**Structure I used:** RTF: Role, Task, Format.

**Why this structure fits my task:**

I chose the RTF format because in this case it is easy to understand. It can help the teacher or whoever is using this prompt edit and tweak it to get the output they want.

**Technique I used:** Zero shot. The prompt gives instructions without an example.

**Why this technique fits my task:**

The teacher gives the information for the quiz directly in the prompt. The tested prompt did not include a sample quiz for the AI to copy.

---

## Part by Part Justification

| Part | What I put here | Why the prompt needs it |
|---|---|---|
| Role | Helping elementary school teachers create quizzes. | Shows who the prompt is for. |
| Task | Topic, grade, number and type of questions, and what the students learned. | Lets the teacher change what they want the quiz to cover. |
| Material limit in Task | Use only what the students have learned, and ask for more information if needed. | I did not want the output to quiz kids on subjects they have not learned. That would be a bad test and would not be helpful. |
| Format | A paper quiz with name and date lines, numbered questions, and a separate answer sheet. | Helps teachers get a quiz they can print. |

---

## Testing and Iteration

The test used sixth grade science, 10 multiple choice questions, and evaporation, condensation, and precipitation in the water cycle.

**Baseline I compared against:**

I want you to create me a 10 question multiple choice science quiz for sixth grade students about evaporation, condensation, and precipitation in the water cycle. It should be on paper, and give me an answer key.

| Version | Result / score | Notes/What Changed. |
|---|---|---|
| Naive baseline | 35/100 | A plain request for a paper quiz and answer key. |
| Version 1 | 100/100 | Used Role, Task, and Format; limited questions to taught material; requested a print layout and separate answer sheet. |
| Final | Same as Version 1 | Kept the tested prompt because it scored 100/100 and was simple and easy to use. |

| Rubric category | Naive | Designed |
|---|---:|---:|
| Clarity & Specificity | 15/30 | 30/30 |
| Structure & Framework Use | 0/30 | 30/30 |
| Context & Inputs | 10/20 | 20/20 |
| Output Requirements | 10/20 | 20/20 |
| **Total** | **35/100** | **100/100** |

The Gem scored the prompts but did not generate quiz outputs. I then ran the prompts separately and collected both quizzes. The model name was not recorded.

The exact prompts, feedback, and quiz outputs are saved in [examples/](./examples/).

The 100/100 score belongs to the filled sixth grade example. Other grades, topics, and question types were not tested.

**What testing showed:**

The biggest difference was that the designed prompt outputs a quiz that stays on topic. For example, the naive quiz talks about transpiration when it was not supposed to. The designed quiz also does a better job of making a quiz that is easier to read for grade school kids.

**What I learned:**

Limiting the questions to material already taught helps keep the quiz useful. The RTF format also makes the prompt easy for the teacher to edit and tweak.

---

## Strengths and Limitations

**Works well when:**

The teacher gives the material the students have learned. In this test the designed quiz stayed focused on evaporation, condensation, and precipitation.

**Struggles when:**

The teacher needs a file that is ready to print. It sent the quiz as text with the answers attached.

**Would improve next:**

The output. I would make sure that it sends the quiz as pdf and the answer key as a separate PDF.
