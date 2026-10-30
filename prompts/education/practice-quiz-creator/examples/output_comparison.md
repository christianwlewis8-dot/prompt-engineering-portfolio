# Output Comparison: Practice Quiz Creator

## Naive Prompt

```text
I want you to create me a 10 question multiple choice science quiz for sixth grade students about evaporation, condensation, and precipitation in the water cycle. It should be on paper, and give me an answer key.
```

**Gem score:** 35/100.

The score was supplied for the same sentence with hyphens in "10-question", "multiple-choice", and "sixth-grade". The student removed those hyphens before generating the quiz below. No separate score was reported for that punctuation change.

### Gem Rubric Breakdown

- **Clarity & Specificity:** 15/30 - The primary objective is clear, but specific operational constraints and difficulty guidelines are left vague.
- **Structure & Framework Use:** 0/30 - The request is written as an unstructured, naive prompt without any labeled sections or framework components.
- **Context & Inputs:** 10/20 - The prompt specifies the target audience and science topics, but omits essential background details like standard alignment or student reading level.
- **Output Requirements:** 10/20 - It outlines basic output constraints (10 questions, multiple choice, answer key included), but leaves formatting style, option counts (e.g., A–D), and visual layout parameters undefined.

### Gem Comparison & Feedback

This submission represents a typical naive prompt that relies on basic conversational phrasing rather than deliberate design. To elevate the score, organize the request into an explicit framework (such as R-T-F or C-A-R-E) with clearly labeled sections for Context, Task, Constraints, and Output Format. Adding explicit boundaries—such as requiring four options per question, specifying an answer key placement at the end, and setting an appropriate 6th-grade reading level—will ensure more consistent and usable results.

FINAL SCORE: 35

### Quiz Output

**Name:** \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

**Date:** \_\_\_\_\_\_\_\_\_\_\_\_

**Class:** \_\_\_\_\_\_\_\_\_\_\_

### Water Cycle Science Quiz: Evaporation, Condensation, & Precipitation

1. What is the primary energy source that drives the water cycle? A) Wind currents

   B) The Sun

   C) Geothermal energy

   D) Ocean tides
2. Which process describes liquid water changing into water vapor (a gas) as it absorbs heat? A) Condensation

   B) Evaporation

   C) Precipitation

   D) Infiltration
3. Water vapor is an invisible component of our atmosphere. What state of matter is water vapor? A) Liquid

   B) Solid

   C) Gas

   D) Plasma
4. You notice water droplets forming on the outside of an iced drink on a hot summer afternoon. Which process causes these water droplets to form? A) Evaporation

   B) Condensation

   C) Precipitation

   D) Transpiration
5. How does condensation contribute to cloud formation high in the atmosphere? A) Liquid water absorbs heat and rises into the air.

   B) Gravity pulls heavy cloud particles down to the ground.

   C) Warm water vapor rises, cools down, and forms tiny water droplets or ice crystals.

   D) Plants release excess water directly into cloud layers.
6. Which of the following is **NOT** a form of precipitation? A) Rain

   B) Hail

   C) Sleet

   D) Fog
7. What condition must occur for water vapor in the atmosphere to condense into liquid water? A) The air must cool down.

   B) The air must be heated by direct sunlight.

   C) Winds must drop to zero miles per hour.

   D) Soil must absorb all surface water.
8. Plants absorb water from the soil and release water vapor into the air through tiny openings in their leaves. What is this process called? A) Precipitation

   B) Condensation

   C) Transpiration

   D) Runoff
9. Which force causes precipitation to fall from clouds down to Earth's surface? A) Friction

   B) Magnetism

   C) Solar radiation

   D) Gravity
10. Which statement best describes what happens during precipitation? A) Puddles on a sidewalk disappear on a warm day.

    B) Water droplets in clouds grow heavy enough to fall to Earth as rain, snow, or sleet.

    C) Water vapor cools and coats blades of grass as morning dew.

    D) Water trickles through soil to replenish underground freshwater stores.

### Answer Key

1. **B — The Sun** (Solar radiation provides heat energy to warm liquid water).
2. **B — Evaporation** (Thermal energy causes liquid water molecules to turn into gaseous water vapor).
3. **C — Gas** (Water vapor is the gaseous state of $H_2O$).
4. **B — Condensation** (Warm water vapor in the air touches the cold glass, cools down, and transforms into liquid water droplets).
5. **C — Warm water vapor rises, cools down, and forms tiny water droplets or ice crystals** (Cooler air higher in the troposphere causes water vapor to condense around microparticles like dust).
6. **D — Fog** (Fog is a cloud forming near ground level through condensation; it is not water actively falling to the ground).
7. **A — The air must cool down** (A decrease in temperature slows down gas molecules, causing them to condense into liquid).
8. **C — Transpiration** (The biological release of water vapor from plant stomata into the atmosphere).
9. **D — Gravity** (Gravity pulls condensed water droplets/ice crystals down once they become too dense to stay suspended in the atmosphere).
10. **B — Water droplets in clouds grow heavy enough to fall to Earth as rain, snow, or sleet** (This defines precipitation as moisture falling under gravity).

---

## Designed Prompt

```text
Role:
You are going to be helping elementary school teachers create quizzes for their students.

Task:
Create a 10-question multiple-choice science quiz about the water cycle for sixth-grade students.

The students have learned about evaporation, condensation, and precipitation. Base every question only on that material. If there isn’t enough material to create the requested number of questions, ask the teacher for more information.

Format:
Produce a quiz that teachers can print for students to complete on paper. Include a place for the student’s name and date, and number the questions. Put the simple answer sheet on a separate page so teachers can print it separately. Use wording appropriate for sixth-grade students.
```

**Gem score:** 100/100.

### Gem Rubric Breakdown

- **Clarity & Specificity:** 30/30 - The core task of creating a 10-question water cycle quiz is explicitly stated with tight boundaries and a clear fallback instruction if source material is insufficient.
- **Structure & Framework Use:** 30/30 - The prompt utilizes a clean, labeled R-T-F (Role, Task, Format) structure where each section delivers substantive, non-overlapping information.
- **Context & Inputs:** 20/20 - It provides precise context regarding the target audience (elementary school teachers and 6th-grade students) and limits the scope strictly to evaporation, condensation, and precipitation.
- **Output Requirements:** 20/20 - The prompt explicitly details all three output parameters: length (10 multiple-choice questions), structure (printable layout with name/date lines and a separate answer key page), and tone (6th-grade reading level).

### Gem Comparison & Feedback

This designed prompt excels by translating a classroom need into clear, actionable parameters using the R-T-F framework. By specifying page-break requirements for the answer key and restricting question content to only three specific concepts, it prevents generic filler and ensures the output is immediately usable. Compared to a typical naive request, this structured approach eliminates the need for manual reformatting or follow-up corrections.

FINAL SCORE: 100

### Quiz Output

Name: \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ Date: \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

## Water Cycle Quiz: Evaporation, Condensation, & Precipitation

**Directions:** Read each question carefully and circle the letter of the correct answer.

1. What is evaporation? A. The process where liquid water turns into water vapor (gas) B. The process where water falls from clouds to the ground C. The process where water vapor cools and turns into liquid water D. The process where solid ice turns directly into liquid water
2. Which scenario is an example of evaporation? A. Rain falling on a garden B. Water droplets forming on the outside of a cold water bottle C. A wet puddle drying up in the sunshine D. Snowflakes gathering on a mountaintop
3. What role does heat play in the process of evaporation? A. It cools water vapor down so it can form clouds B. It warms liquid water, giving it energy to change into water vapor C. It makes cloud droplets heavy so rain falls to Earth D. It freezes liquid water into sleet or hail
4. What is condensation? A. Liquid water changing into invisible water vapor B. Water vapor cooling down and changing back into liquid water C. Water falling from clouds as rain, snow, sleet, or hail D. Water collecting in puddles on the ground
5. How does condensation lead to cloud formation in the sky? A. Liquid water on the ground warms up and floats into the sky as clouds B. Water vapor rises, cools down in the upper atmosphere, and forms tiny liquid droplets C. Falling rain droplets freeze together to create clouds D. Sunshine heats water vapor until it turns into solid cloud shapes
6. Which of the following is a real-world example of condensation? A. Dew drops forming on grass during a cool morning B. Water boiling in a pot on a stove C. A wet towel drying on a clothesline D. Hail falling during a thunderstorm
7. What is precipitation? A. The cooling of water vapor in the sky B. The warming of liquid water on Earth's surface C. Any form of water that falls from clouds to the Earth's surface D. The invisible gas phase of water rising into the air
8. Which list contains four common forms of precipitation? A. Dew, fog, mist, and cloud B. Rain, snow, sleet, and hail C. Evaporation, condensation, vapor, and liquid D. Frost, steam, gas, and ice
9. Why does precipitation fall from clouds to the ground? A. Cloud droplets get warmer and turn into heavy gas B. Water droplets in clouds grow larger and become too heavy to remain suspended in the air C. The sun pulls the liquid water downward from the atmosphere D. Evaporation pushes the water out of the clouds
10. Which process sequence shows water changing from a liquid on Earth, forming clouds in the sky, and returning to Earth's surface? A. Condensation $\rightarrow$ Precipitation $\rightarrow$ Evaporation B. Evaporation $\rightarrow$ Condensation $\rightarrow$ Precipitation C. Precipitation $\rightarrow$ Evaporation $\rightarrow$ Condensation D. Condensation $\rightarrow$ Evaporation $\rightarrow$ Precipitation

## Answer Key (Teacher Reference)

1. **A** — The process where liquid water turns into water vapor (gas)
2. **C** — A wet puddle drying up in the sunshine
3. **B** — It warms liquid water, giving it energy to change into water vapor
4. **B** — Water vapor cooling down and changing back into liquid water
5. **B** — Water vapor rises, cools down in the upper atmosphere, and forms tiny liquid droplets
6. **A** — Dew drops forming on grass during a cool morning
7. **C** — Any form of water that falls from clouds to the Earth's surface
8. **B** — Rain, snow, sleet, and hail
9. **B** — Water droplets in clouds grow larger and become too heavy to remain suspended in the air
10. **B** — Evaporation $\rightarrow$ Condensation $\rightarrow$ Precipitation

---

## Comparison

Both outputs have 10 questions and answer keys. The naive quiz asks about transpiration in question 8. The designed quiz stays focused on the three taught concepts. Its text still needs formatting for printing, and the pasted output does not show a separate answer page.

The Gem scored the prompts. The quiz outputs came from separate runs supplied by the student. The model name was not recorded. The reusable prompt in prompt.md has placeholders and some later wording edits; its exact current wording was not separately rescored.
