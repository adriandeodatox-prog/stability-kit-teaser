# Clarity Anchor Protocol — Plausible Hallucination Risk Diagram

```text
[Input Step n]
      |
      v
+---------------------------+
| Ambiguity Detection       | [-15% hallucination]
| - Detect uncertain input  |
| - Ask for clarification   |
+---------------------------+
      |
      v
[Clarification Provided?] ---> No ---> Halt / Prompt user
      |
      Yes
      v
+---------------------------+
| Confirmed Context         |
| - Update understanding    |
+---------------------------+
      |
      v
[Output Step n+1]
Reduced Plausible Hallucination: -15%

Legend / Notes

Ambiguity Detection: Identifies when input is unclear or has multiple meanings.

Clarification Provided: Ensures that ambiguous input is clarified before proceeding.

Confirmed Context: Updates the model’s understanding based on the clarified input.

Effect: CAP forces ambiguity to surface before acting, ensuring that hallucinations don’t arise from unclear or uncertain input.
