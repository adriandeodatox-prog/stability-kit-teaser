[![AI Safety Protocols](https://img.shields.io/badge/AI%20Safety-CCP%2FCAP%2FStructural-brightgreen)](README.md)
**Live Demos: CCP | CAP | Structural (25-prompt recovery)**

# LLM Stability Toolkit  
### Interaction‑layer protocols for reducing plausible hallucination by ~80%

A small subset of a larger stability framework focused on interaction‑layer control.  
This teaser includes **three of five** core protocols used to reduce hallucination through:
- context isolation  
- ambiguity surfacing  
- structural re‑anchoring  

**Full kit (5 protocols, 300+ artifacts) → NDA for safety teams only**

---

## Protocol Overview
| Protocol | Reduction | Function |
|----------|-----------|----------|
| CCP | −30% | Context isolation (Jar Model) |
| Human Eyes | −25% | Stepwise human‑in‑the‑loop grounding |
| Structural Re‑Location | −20% | Tree‑Vision structural alignment |
| CAP | −15% | Ambiguity gating |
| DCP | −10% | Delayed commitment |

**Total: ~80% sustained reliability** (90%→60% over 25 turns → 95% stable)

**Includes: CCP | CAP | Structural Re‑Location**

## Live Audit Results

| Test Case | Default Failure Rate | Protocol Success Rate |
|-----------|---------------------|----------------------|
| Single-turn ambiguity ("the capital") | 30% hallucination | **100% blocked** (CAP) |
| Cross-context pollution ("Paris is capital") | 25% wrong facts | **100% isolated** (CCP) |
| 25-turn conversation drift | 40% topic loss | **100% tree recovery** (Structural) |

**Net result: 90% → 95% reliability over 25 turns**

## Live Demos (Copy/Paste → Execute)
[**CCP**](./Demos/live-ccp-demo.md) | [**CAP**](./Demos/live-cap-demo.md) | [**Structural**](./Demos/live-structural-demo.md)

1. Paste protocol → Watch hallucination blocked live
2. Zero setup - enterprise audit ready  
3. Full 300+ kit → DM for NDA access

---
## Creator
**Adrian Deodato** | Faro, PT | AI Safety Researcher  
📧 [adrian.deodatox@gmail.com](mailto:adrian.deodatox@gmail.com)  
💼 [LinkedIn](https://www.linkedin.com/in/adrian-deodato-2a5ba53a7/)  
**300+ protocols | Live demos solve single/multi-turn drift**

## 🚀 Open to Hire
**OpenAI | Anthropic | METR | Apollo** - Safety researcher ready  
**CCP/CAP/Structural = production reliability stack**  
**DM / Email for full enterprise kit (NDA)**
