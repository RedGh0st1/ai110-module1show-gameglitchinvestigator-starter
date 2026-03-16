# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it?
  I
- List at least two concrete bugs you noticed at the start
  (for example: "the secret number kept changing" or "the hints were backwards").
  Bugs we found:

1. When we click the show hint it doesn't work
2. the lower/higher logic was flipped.
3. New Game button doesn't work, doesn't clean and start a new game
4. When a user inputs a number that is out of range, the game still allows the input without an alert. The USER should be required to choose a number within the range.
5. Update the user prompt for Easy Mode. When the user chooses Easy Mode, the range to guess should be 1-20. Currently, the game is prompting the user to guess a number between 1 and 100, so that range should also be fixed.
6. When we set the difficulty to hard, it says the range is 1-50, and when we set the difficulty to normal, it says the range is 1-100. This should be flipped.
7. The Submit Guess button seems delayed. When I click it, the action doesn't go through, but when I click it again, it goes into the history in the developer debug info.

---

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)?
  ans: I use Claude code.
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
  Answer: AI suggestion that corrct withoiut changing was the "NEW Game" button needed to explicity call rerun())
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).

---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
- Describe at least one test you ran (manual or using pytest)and what it showed you about your code.
- Did AI help you design or understand any tests? How?

---

## 4. What did you learn about Streamlit and state?

- In your own words, explain why the secret number kept changing in the original app.
- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?
- What change did you make that finally gave the game a stable secret number?

---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task?
- In one or two sentences, describe how this project changed the way you think about AI generated code.
