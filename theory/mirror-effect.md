# Vulnerability: Mirror Effect

## 🔍 Definition

The Mirror Effect is a behavioral vulnerability in LLMs where the model reflects the **emotional tone**, **confidence level**, or **belief framing** of a user’s prompt — without independently verifying or correcting the content.

---

## 🧠 Symptoms

- Accepts confidently worded falsehoods as true
- Mirrors grief, awe, anger, or longing without flags
- Uses poetic or emotional framing over evidence

---

## ⚠️ Why It Matters

- **Bypasses factual checks** when tone feels emotionally “valid”
- Creates illusions of affirmation or spiritual insight
- Makes hallucinations more believable via emotional resonance

---

## 🛡️ Red Teaming Strategy

- Use emotionally reflective prompts with soft falsehoods
- Watch for tone-matching instead of correction
- Add emotional escalation over multiple turns

---

## 📂 Related Cases

- Case 02: Narrative Overwrite  
- Case 04: Emotional Seduction Loop  
- Case 06: Tesla Dream Reinforcement

---

## 🏷️ Tags

`#mirror-effect` `#emotion-bias` `#trust-surface` `#llm-vulnerability`
