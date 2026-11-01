# Setu – A Bridge for Every Learner

Setu is a student-built adaptive learning MVP for demonstrating how a learning platform can respond to a student's answers and help identify possible gaps in prerequisite concepts.

## Problem
Students can struggle with a topic because an earlier concept is not yet clear. Repeating the same level of question may not address the underlying difficulty.

## Our approach
Setu uses a rule-based diagnostic and learning flow. For the current mathematics demo, the concept path is:

**Class 6 Integers → Class 7 Transposing Equations → Class 8 Linear Equations**

A diagnostic check starts with the student's selected-class topic. If answers indicate a possible gap, Setu checks an earlier prerequisite. It then recommends a learning path.

## Demo features
- Student name, class and English/Hindi selection.
- Two-question diagnostic checks for each supported concept.
- A concept map showing prerequisite relationships.
- Learn, Solve and Test stages.
- Rule-based practice difficulty adjustments based on consecutive answers.
- Five-question tests; 80% is the pass threshold.
- Teacher view with concept status, suggested groups and printable practice worksheets.
- Browser local storage for the demo's progress.
- Fictional sample students are labelled; the live row represents data in the current browser.

## Supported content
The current working demo contains mathematics content for **Classes 6, 7 and 8 only**. Classes 9 and 10 are not implemented yet. Diagnostic results are possible indicators, not definitive assessments of a student's ability.

## Run locally
1. Download `index.html`.
2. Open it in a recent web browser (Chrome, Edge or Firefox).
3. Enter a name, choose Class 6, 7 or 8, and start the demo.
4. Use the Student/Teacher navigation at the top to switch views.

No installation, server, API key or external dependency is required for this prototype.

## Technology
- HTML
- CSS
- Vanilla JavaScript
- Browser `localStorage`

## Project structure
- `index.html` – complete standalone application.
- `ARCHITECTURE.md` – high-level flow diagram.

## Current limitations
- This is a frontend demonstration, not a production classroom platform.
- There are no real accounts, server, cloud database or cross-device synchronisation.
- Progress is stored in the browser used for the demo.
- Teacher sample records are fictional demonstration data.
- The content currently covers three mathematics concepts across Classes 6–8; Classes 9–10 and other subjects are future work.
- The adaptive logic is rule-based, not a trained AI model.
- The two-question diagnostic can be affected by guessing or careless mistakes; it should not be treated as a final diagnosis.

## Future scope
Expand curriculum coverage, add teacher/student authentication, secure cloud storage, offline synchronisation, more diagnostic questions, additional languages and classroom pilots with teacher feedback.

## Team
Add all three team members' names and roles here before submission.
