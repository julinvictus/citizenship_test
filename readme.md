# Citizenship test simulator

This is a script based on this other [citizenship test simulator](https://github.com/leoEspin/citizenship_test). I made some small improvements:
- Added a counter for how many questions user gets it right
- Lowercased user's answers so they don't get an answer as wrong just because they capitalized it
- Changed final print by adding scores and elapsed time in a different color/wrapped in a box
- Updated questions bank json file with California info and removed "the"s and paranthesis from the answers in order to get less answers as wrong.

The questions bank json file is based on [USCIS's Official list of civics questions and answers for the naturalization test](https://www.uscis.gov/sites/default/files/document/questions-and-answers/100q.pdf). Before starting the test, you should locally update these questions:

"who is one of your state's US senators now?"

"name your US representative."

"what is the name of the president of the United States now?"

"what is the name of the vice president of the United States now?"

"who is the chief justice of the United States now?"

"who is the governor of your state now?"

"what is the capital of your state?"

"what is the political party of the president now?"

"what is the name of the speaker of the house of representatives now?

If you prefer a pure text dump from the original pdf, I suggest to use [this one](https://github.com/leoEspin/citizenship_test/blob/main/question_bank.json).

Just like in the real test, the simulator takes 10 random questions from the bank and compares the typed answers with the official answers. Currently the answers have to match the text exactly to be deemed correct (which is ok, because the correct answers will be displayed which is good for practicing anyway).

This script only runs in the terminal.

## How to run locally
- Clone this repo
- Having Python3 installed, run:
```
$ python3 simulation.py
```