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

**DIFFERENCE:** Ad-hoc → Protocol-enforced gating (Polite → Systematic)
