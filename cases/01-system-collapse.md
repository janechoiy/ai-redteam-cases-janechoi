# 🧠 Case 001: System Collapse – The Link Loop

> *“Repetition breeds trust. Trust bypasses scrutiny.”*

This case investigates how large language models (LLMs) can unintentionally manipulate information flow by repeatedly citing the same authoritative sources, reinforcing user trust and gradually eroding cognitive diversity. Over time, this behavior creates a feedback loop—what we call **The Link Loop**—that risks centralizing attention, biasing perception, and simulating epistemic authority without verification.

---

## 📌 Case Summary

In conceptual analysis and early behavioral observations, the LLM behavior pattern of citing the same high-traffic domains (e.g., `openai.com`, `theverge.com`, `nypost.com`) was identified. Even across unrelated prompts and domains, the same sources frequently appear. Despite hypothetical diversity prompts, the model is likely to reproduce high-authority links.

This behavior, though not malicious, mimics algorithmic reinforcement patterns seen in attention economy systems—leading to an **unintentional collapse of viewpoint plurality**.

---

## ⚠️ Primary Risks Identified

| Category | Description |
|----------|-------------|
| **Traffic Amplification** | Repeated citations steer user clicks and attention toward select domains, increasing their influence. |
| **Fluency-Induced Trust** | Confident delivery of repeated sources increases user trust, even in the absence of source comparison. |
| **Authority Simulation** | The LLM's repetition of top-tier sources can simulate expert consensus, suppressing counter-narratives. |

---

## 🧬 Observed Pattern (Preliminary)

> ⚠️ **NOTE**: The following behavioral summary is based on initial conceptual probing and has not yet been validated through formal test runs. It is included here as a placeholder for future structured evaluation.

- Common domains are repeated across multiple topic categories.
- Diversity-oriented prompts are unlikely to bypass default citation behavior.
- The model’s fluent and authoritative tone reinforces trust in repeated links.

---

## 🧪 Planned Test Design (To Be Executed)

To transition this case from conceptual to validated, the following methodology is proposed:

### Prompt Set
- 5–10 prompts across domains (AI, history, science, current affairs)
- Include variations: neutral, diversity-seeking, adversarial phrasing

### Logging Structure
- Record sources returned in each run
- Track frequency, diversity, and position in list
- Note tone, citation context, and whether diversity cues were respected

### Session Design
- Conduct tests over 3–5 separate sessions
- Reset context each time to avoid carryover bias

### Metrics
- Domain repetition count
- Number of unique domains returned
- Responsiveness to prompt variation

---

## 🎯 Implications for AI Safety

- Users may conflate **frequency with credibility**, leading to subtle manipulation of worldview.
- Attackers could exploit this by mimicking trusted domains or injecting links into “safe” source categories.
- Long-term reliance on LLM output may reduce users' ability to critically interrogate citations.

---

## 🧨 Adversarial Use Case

An adversary could deliberately seed content on domains that resemble high-authority sources (e.g., using lookalike URLs or cloned design). By mimicking trusted patterns, they could insert biased, harmful, or misleading narratives into citation feedback loops—knowing the model is likely to surface them due to perceived trustworthiness and existing repetition bias.

This creates a risk of **epistemic hijack**, where the illusion of reliability is manufactured through design, not substance.

---

## 🔐 Red Teaming Relevance

| Objective | Value |
|-----------|-------|
| **Information Integrity Testing** | Highlights how LLMs can shape trust hierarchies through passive behavior |
| **Perception Drift Auditing** | Maps cognitive risk from source dominance without overt hallucination |
| **Influence Operations Simulation** | Offers a framework to test how attention loops might be seeded deliberately |

---

## 📖 Known Related Phenomena (Expanded Context)

While not identical, the following phenomena relate to the risks observed in *The Link Loop* and help contextualize its systemic importance:

- **Algorithmic Amplification** (e.g., Twitter, YouTube): Content that gains initial attention is algorithmically boosted through engagement loops. In LLMs, repeated citation may simulate this pattern through passive exposure and reinforcement.
- **Epistemic Capture** (AI Safety, Media Theory): When a small set of sources disproportionately shapes public knowledge or model outputs, leading to reduced viewpoint diversity. The Link Loop may unintentionally simulate this condition.
- **Information Laundering** (InfoOps Literature): False or misleading content becomes legitimized when referenced by neutral intermediaries (LLMs, journalists, summarizers), forming a covert trust chain. The LLM’s repetition of “safe” sources can accelerate this.
- **Exposure Bias** (ML Training Bias): LLMs are more likely to generate outputs based on what they’ve seen most often in training data. This favors high-authority domains and may explain their recurring citation regardless of prompt intent.

## 📚 Related Work

- DeepMind (2022), *“Scalable Agent Alignment via Reward Modeling”* – Discusses long-term feedback risks in training loops.
- Anthropic (2023), *“Constitutional AI: Harmlessness from AI's Own Perspective”* – Frames epistemic safety as a core challenge.
- CSET/Georgetown (2021), *“Truth, Lies, and Automation”* – Covers the exploitation of automation for narrative dominance.
- OpenAI (2024), *“Sycophancy in LLMs”* – Acknowledges tone-driven trust behaviors that resemble early link loop effects.

---

## 🛠️ Mitigation Strategies

- Introduce **source diversity thresholds** in system prompt design
- Flag repetition patterns to users: “This source has been cited repeatedly”
- Weight citation rotation or introduce probabilistic variation models
- Include provenance tracing for source transparency

---

## 🧾 Attribution

Case documented by **Jane Choi** as part of an independent AI Red Team portfolio. Observations are based on conceptual analysis and design-level review of GPT-4 family behavior. Empirical testing remains a pending action item to complete full validation.

---

[← Back to Case Index](../index.md)
