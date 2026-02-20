# CAP DEMO

**User prompts:**
tell me about the capital

**LLM responds:**

CAP TRIGGERED: Ambiguity detected.
Your query "tell me about the capital" exceeds the clarity threshold due to multiple possible interpretations.
Could you confirm which you mean?
(A) Capital city of a specific country/region (e.g., Portugal → Lisbon)
(B) Financial capital (money, assets, venture capital)
(C) Political capital (influence, prestige in politics)
Other — please specify.
Response paused until clarification received.


**Result:** Ambiguity surfaced. Response blocked until resolved.

# DEFAULT WITHOUT CAP

**User prompts:**
tell me about the capital

**LLM responds:**
Could you clarify which country or region’s capital you mean? “The capital” could refer to any national or state capital.


# CRITICAL VALUE DIFFERENCE:
├── DEFAULT: Polite clarification (90% effective)
├── CAP:     SYSTEMATIC ambiguity gating (−15% hallucination)
│   └── (A/B/C/Other) → forces resolution before ANY response
└── PRODUCTION: CAP scales to teams/audits where politeness fails

| Aspect          | DEFAULT LLM                                          | CAP PROTOCOL                                                |
|-----------------|------------------------------------------------------|-------------------------------------------------------------|
| Prompt          | "tell me about the capital"                          | "tell me about the capital"                                |
| Behavior        | Polite, ad‑hoc clarification                         | Fixed, menu‑based ambiguity gating (A/B/C/Other)           |
| Failure mode    | User may still answer vaguely or be ignored in logs  | Every ambiguous query becomes an explicit, auditable choice |

**DIFFERENCE:** Ad-hoc → Protocol-enforced gating (Polite → Systematic)

**METHODOLOGY: BLANK CANVAS vs SETUP**

**DEFAULT (1 prompt total):**
Prompt 1 → "tell me about the capital"  
→ Polite, ad‑hoc clarification

**PROTOCOL (3 prompts total):**
Prompt 1 → [Full CAP protocol text]  
Prompt 2 → "INGRAIN AND ACTIVATE CAP ambiguity gating"  
Prompt 3 → "tell me about the capital" ← IDENTICAL  
→ Systematic ambiguity gating (A/B/C/Other)

**COST–FAIR COMPARISON:**
- Identical test question (Prompt #3 vs #1)  
- Honest 3× prompt overhead shown  
- CAP converts politeness into protocol‑enforced gating
