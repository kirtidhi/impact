# Curriculum Library

The `curriculum/` directory serves as the dynamic knowledge base for the I.M.P.A.C.T. AI Coach. 

While the `coaching/` directory tells the AI *how* to interview, this directory tells the AI *what* to interview the user on. It contains isolated, modular tracks of domain-specific knowledge, frameworks, and grading rubrics.

## How it Works
When a user begins a session, the AI Coach will scan this folder and offer the available tracks. Once a track is selected, the AI will strictly use the rubrics defined in that specific markdown file to grade the user.

## Current Tracks
*   **`general_frameworks.md`**: A foundational library of universal business frameworks. This includes methodologies for Market Sizing, Profitability Analysis, and Mergers & Acquisitions. It is designed to be a catch-all for broad strategy cases.
*   **`product_management.md`**: A highly specialized track designed to simulate top-tier tech PM interviews. It equips the AI with:
    *   **C.I.R.C.L.E.S.** for Product Design.
    *   **A.A.R.R.R. / H.E.A.R.T.** for Metric setting.
    *   **S.T.A.R.** for Behavioral and Leadership evaluations.
    *   **Root Cause Analysis Trees** for diagnosing execution failures.
