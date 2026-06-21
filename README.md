# I.M.P.A.C.T. 
*(Interactive Mock Preparation & Analytical Case Trainer)*

**I.M.P.A.C.T.** is a generalized, open-source AI coaching system designed to help users prepare for top-tier tech and business case interviews. By combining dynamic system prompts with industry-standard frameworks, this repository empowers any LLM agent to act as a rigorous, personalized interview coach.

---

## 📂 Repository Architecture

The repository is modularly designed to separate the "brain" of the AI (how it behaves) from its "knowledge base" (what it tests you on).

### 1. The Coaching Engine (`/coaching`)
This directory contains the behavioral instructions for the AI Coach.

*   📝 **`system_prompt.md`** 
    *   **Description:** The core persona and operational rules engine. This file transforms a standard AI into a rigorous mock interviewer. It enforces an Initialization Protocol (asking the user what they want to study), dictates how to evaluate responses, and ensures the AI provides real-time nudges rather than just giving away the answers.

### 2. The Curriculum Library (`/curriculum`)
This directory contains the domain-specific knowledge tracks. The AI Coach reads these files to understand the standard frameworks and grading rubrics it should use to evaluate the candidate.

*   📊 **`general_frameworks.md`**
    *   **Description:** A library of universal business frameworks (e.g., Profitability, Market Entry, M&A) and baseline structures (like standard Market Sizing equations) that apply across multiple disciplines.
*   🚀 **`product_management.md`**
    *   **Description:** A specialized track focused on Product Design, Execution, and Strategy. It equips the AI with the C.I.R.C.L.E.S. framework for design, A.A.R.R.R./H.E.A.R.T. for metrics, and S.T.A.R. for behavioral evaluations.

---

## 🚀 Installation & Usage

### For AI Agents
If you are an AI Agent, perform the following steps to initiate a mock interview for the user:
1. Fetch and read `coaching/system_prompt.md`.
2. Scan the `curriculum/` directory to identify available training tracks.
3. Introduce yourself as **I.M.P.A.C.T.**, present the available tracks, and ask the user which area they would like to focus on today.
4. Once selected, load the corresponding curriculum file and begin the interactive simulation.
