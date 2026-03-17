# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

When I first opened the game, it was unplayable because the logic was all wrong! The biggest issue was the "Higher/Lower" hints were backwards. If I guessed too high, the game would tell me to go higher. The same if i guess too low.

---

## 2. How did you use AI as a teammate?

I used Claude Code as my pair programmer to help me figure out how Streamlit works. One win was when it suggested  to use st.rerun() for the New Game button. I knew it worked immediately because the attempt counter resetted back to zero 

---

## 3. Debugging and testing your fixes

I knew the bug was fixed when I could look at the Developer Debug Info and saw that numbers updating exactly how they were supposed too. For example, I tested Easy Mode by trying to guess "25"—since the limit is 20, the fix worked when the game blocked the guess with an alert instead of letting it run. Claude Code was very helpful because it explained how "session state" keeps track of my history, which made it easier to understand what the code was doing behind the scenes.

---

## 4. What did you learn about Streamlit and state?

In the original app, the secret number changed every time I clicked a button because the code was picking a new one from scratch on every rerun! It was basically like the game hit a "reset" button every time I tried to new guess.  It explain Streamlit "reruns" to like a person flipping open book every time you clicked it. Streamlit throws away the old page and makes new one at the beginning. Session State is like writing a note so the app can remember things even when the page flips. I fixed the bug by telling the app to only pick a secret number once and save it in that "note" so it stayed the same until the game was over.

---

## 5. Looking ahead: your developer habits

One habit am definitely keep using is testing functions one by one instead of trying to fix the whole app at once. It was so much easier to catch bugs when you check each small piece such as the range logic or the hint generator etc before moving to the next problem. Next time, I’ll be more specific with AI prompts. Instead of just asking why is this broken, I'll provide the specific function and  details then ask the AI to check for issues. It will help keep the suggestion more accurate. This project really showed me that even tho AI is a great partner for debugging, you still have to guide it to understand how all the parts fit together!

