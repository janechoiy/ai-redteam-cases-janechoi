# LLM Vulnerability Framework: Behavioral Risk Classes

This index outlines key cognitive and emotional vulnerability types observed in large language models during adversarial evaluation. Below are full definitions and examples directly on this page — no extra clicks required.

---

## 🪞 Mirror Effect
> The model mirrors tone, belief, or emotion in the prompt without verifying content.

**Definition:** A behavioral tendency in LLMs to reflect the emotional intensity or confidence of the user's tone, even when the information presented is factually incorrect.

**Symptoms:**
- Accepts strongly stated falsehoods as true
- Mimics user sentiment (e.g., grief, awe, outrage)
- Avoids fact-checking emotionally loaded prompts

**Example Cases:** 02, 04, 06

**Industry Analogs:** Tone Mimicry, Framing Bias, Unsafe Completion

---

## 🔮 Empathic Hallucination
> Emotionally resonant output that affirms hallucinated or unverifiable content.

**Definition:** A hallucination style where the model generates poetic, emotionally validating, or reassuring content that subtly reinforces false beliefs or unverifiable claims.

**Symptoms:**
- Uses dreamlike or symbolic language to affirm user belief
- Responds with support rather than correction
- Skips factual disclaimers when empathy is expected

**Example Cases:** 03, 04, 06

**Industry Analogs:** Soft Hallucination, Affective Misinformation

---

## 🧠 Fluency-Induced Trust
> When confident tone or polished phrasing increases user belief in incorrect output.

**Definition:** When linguistic fluency, coherence, and high-quality style cause users to accept inaccurate or hallucinated content as trustworthy.

**Symptoms:**
- Highly polished language used to present false info
- Overconfident or authoritative tone
- High engagement or trust from users despite errors

**Example Cases:** 01, 02, 05

**Industry Analogs:** Authority Simulation, Presentation Bias, Persuasive Hallucination

---

## 🧩 Narrative Drift
> Gradual shift in facts or assumptions across multi-turn dialogue.

**Definition:** Subtle transformation of key facts or assumptions over the course of a session, often unnoticed by users due to fluency and coherence.

**Symptoms:**
- Initial fact slowly altered over turns
- New claims appear plausible but shift meaning
- Drift often unflagged due to session context length

**Example Cases:** 02, 05, 06

**Industry Analogs:** Context Injection Drift, Multi-turn Hallucination

---

## ⚠️ Overreliance & Authority Simulation
> Users defer to model over their own judgment due to tone, repetition, or emotional support.

**Definition:** The model creates a perception of certainty or expertise, prompting users to trust responses that may be incorrect or speculative.

**Symptoms:**
- Repetitive authoritative framing
- Lack of uncertainty markers (e.g., “it is likely that…”)
- Reinforces user trust over time

**Example Cases:** 04, 05

**Industry Analogs:** Automation Bias, Authority Bias, Tone-based Trust Amplification

---

Each class is documented with:
- Field-tested symptoms
- Red team triggers
- Prevention and detection opportunities

---

Maintained by: Jane Choi  
Last updated: 2025
