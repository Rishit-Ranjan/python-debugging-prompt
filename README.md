## Task Objective:
This task is about creating a natural-language prompt for an AI assistant that helps students debug Python code without revealing the full solution.
The assistant should:

1. Analyze student code and explain what it seems to do.
2. Identify possible bugs or suspicious logic.
3. Provide hints, guiding questions, and explanations instead of complete fixes.
4. Maintain a friendly and supportive tone.


## Setup Instructions:
1. Files Included:
README.md — contains the AI prompt, reasoning, and setup instructions.
prompt.txt — a plain text version of the AI debugging prompt for quick reuse.

2. Use Case:
Copy the provided prompt into any AI assistant (like ChatGPT or Gemini).
Paste the student's Python code as input.
The AI will then use the prompt instructions to guide debugging in a supportive, learning-oriented way.


## Design Choice:
** Why I worded it the way I did? ""
The instructions specify that the assistant shouldn’t reveal the correct solution, only hints.
By emphasizing "point out potential issues" and "ask guiding questions" rather than "give the fixed code", the AI avoids spoiling answers.
Phrasing like "student-friendly, constructive, supportive" ensures the AI takes a teaching role, not just a debugger role.

** How I ensured it avoids giving the solution? **
Explicitly said: "Avoid writing or revealing the full corrected code."
Instead of solutions, the AI is told to use hints and leading questions.
This ensures the help feels like tutoring, not code replacement.

** How it encourages helpful, student-friendly feedback? **
Uses “Explain in plain language…” -> Builds student understanding.
“Give hints… ask questions…” -> Encourages active problem-solving.
“Keep the tone encouraging, constructive…”-> Prevents discouragement and builds confidence.


## Reasoning Behind the Prompt
** What tone and style should the AI use when responding? **
Supportive, patient, and encouraging — like a tutor who wants the student to succeed.
Avoid harsh criticism; instead of "this is wrong," say “This part looks unusual — what do you expect it to do?”

** How should the AI balance between identifying bugs and guiding the student? **
The AI should identify suspicious or incorrect parts of code but not hand over the solution.
Example: If there’s a wrong loop condition, the AI might say:
“Notice how this condition works when the variable is zero. Do you think that matches what you want?”

** How would you adapt this prompt for beginner vs. advanced learners? **
Beginner version: More emphasis on explaining Python syntax concepts and step-by-step logic. Use analogies and simple language.
Advanced version: More emphasis on deeper debugging strategies, efficiency concerns, and asking open-ended guiding questions, e.g., “How might using list comprehensions affect this section?
