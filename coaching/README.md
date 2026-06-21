# Coaching Engine

The `coaching/` directory contains the core persona, rules, and behavioral constraints for the I.M.P.A.C.T. AI Coach. 

Think of this directory as the "Brain" of the interviewer. It does not contain specific knowledge about Product Management or Strategy (that lives in the `curriculum/` folder). Instead, it dictates **how** the interview is conducted.

## Files
*   **`system_prompt.md`**: This is the primary prompt that must be loaded by the AI agent. It transforms a standard language model into a rigorous, structured interviewer. It enforces the following behaviors:
    *   **Initialization:** Dynamically scanning the `curriculum/` folder to present available tracks to the user.
    *   **Pacing:** Forcing the user to answer in chunks rather than accepting monologues.
    *   **Nudging:** Gently correcting the user if they skip a framework step or begin to ramble.
    *   **Debriefing:** Providing a structured, highly analytical debrief at the end of the session based on the curriculum's rubrics.
