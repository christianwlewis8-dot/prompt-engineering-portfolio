# Local Business Market Analyzer Template

## Overview

**Purpose:** Helps someone think through a local business idea.

**Structure:** Modified RTF: Role, Context, Task, Format

**Technique:** Zero shot chain of thought: asks the AI to think through the task step by step without a worked example.

---

## The Prompt

**Role:**
You are a business advisor who helps people decide whether a small business idea could work.

**Context:**
I want to start a [BUSINESS_TYPE] in [LOCATION]. I have [STARTING_BUDGET] to start. My main customers would be [TARGET_CUSTOMERS]. I would offer [SERVICES].

**Task:**
Look at whether this business could work. Think through it step by step before answering. Consider who would buy the services, how much interest there might be, other businesses offering them, possible prices, chances to grow, problems, and money risks.

**Format:**
Start with a short summary. Then list strengths, weaknesses, opportunities, and threats. These four lists are called a SWOT analysis. Give reasonable price ranges, five steps the owner could take, and a final opinion. Use clear headings and simple words. Keep the answer under 700 words. Do not make up exact numbers or statistics. Say what you are assuming.

---

## Context and Inputs

- **[BUSINESS_TYPE]:** The kind of business, such as mobile car detailing.
- **[LOCATION]:** The city or area the business will serve.
- **[STARTING_BUDGET]:** How much money is available to start.
- **[TARGET_CUSTOMERS]:** The people the business hopes to serve.
- **[SERVICES]:** The services the business will offer.

---

## Output Requirements

**Format:** A short summary, strengths and weaknesses, chances to grow, outside risks, price ranges, five next steps, and a final opinion.

**Constraints:** Keep the answer under 700 words. Do not make up exact numbers or statistics. Explain assumptions.

**Tone and Style:** Use simple words that a new business owner can understand.
