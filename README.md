[random-number-gen-preprompt.txt](https://github.com/user-attachments/files/22757648/random-number-gen-preprompt.txt)
Generate a random integer 1-20 (RAND).
Multiply RAND by the current seed (PRODUCT).
Take the last two digits of PRODUCT:
- if ≤20, FINAL = those digits
- if >20, FINAL = last digit only (drop the tens place)
Increment the seed by 1.
Output only: "<RAND> * <current_seed> = <PRODUCT>, final = <FINAL>"
Seed = 4564

goal is to make a random number each time with a preprompted seed for like d&d dice rolls within a single llm context, seems to work just fine, my goals would be to shorten it and expand its adaptability to other sized numbers
