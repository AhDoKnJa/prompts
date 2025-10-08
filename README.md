# Random Number Generator Pre-Prompt

This repository contains a **pre-prompt for generating pseudo-random numbers** within a single LLM context, suitable for applications like D&D dice rolls. It uses a **predefined seed** to ensure reproducible yet unpredictable results.

---

## future goals

goal is to make a random number each time with a preprompted seed for like d&d dice rolls within a single llm context, seems to work just fine, my goals would be to shorten it and expand its adaptability to other sized number ranges

```text
Seed = 12345
Generate a random integer 1-20 (RAND)
PRODUCT = RAND * Seed
Seed = PRODUCT % 2147483647
FINAL = (Seed % 20) + 1
Output only: "<RAND> * <Seed> = <PRODUCT>, seed = <Seed>, final = <FINAL>"
