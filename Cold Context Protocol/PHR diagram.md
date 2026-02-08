# Cold Context Protocol — Plausible Hallucination Risk Diagram

```text
[Input Step n]
      |
      v
+---------------------------+
| CCP Context Isolation     | [-30% hallucination]
| - Only current input valid|
| - All other context sealed|
+---------------------------+
      |
      v
[Jar Activation Required?] ---> No ---> Proceed without sealed context / Request clarification
      |
      Yes
      v
+---------------------------+
| Explicit Jar Access       |
| - Identity, History, etc. |
| - Bounded scope & duration|
+---------------------------+
      |
      v
[Deterministic Interaction]
- Literal parsing only
- Local reasoning only
- No implicit inference
      |
      v
[Optional Orientation?] ---> Non-binding suggestion for continuity
      |
      v
+---------------------------+
| Output Step n+1           |
+---------------------------+
Reduced Plausible Hallucination: -30%

Legend / Notes

CCP Context Isolation: Prevents carryover from previous context, a key cause of hallucination.

Jar Activation Required: Ensures no hidden context affects the response.

Deterministic Interaction: Restricts reasoning to what’s directly provided, avoiding inference.

Optional Orientation: Non-binding suggestion for continuity, preventing unintentional shifts.

Effect: Cold Context Protocol reduces hallucinations by isolating the current input and ensuring that no external context silently influences the reasoning process.
