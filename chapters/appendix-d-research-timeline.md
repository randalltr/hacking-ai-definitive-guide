# Appendix D – Timeline of Prompt Injection Research and Milestones

Prompt injection began as a niche concern among early prompt engineers and has evolved into a leading security risk category for LLM-integrated systems. This appendix provides a structured timeline of key milestones in the development of prompt injection techniques, terminology, tooling, and defense strategies.

---

## 2021 — Foundations

- **July 2021** – Term "Prompt Injection" coined  
  Simon Willison publicly demonstrates that large language models can be manipulated by embedding instructions in user-supplied text, overriding original prompts.

- **August 2021** – Informal experiments on GPT-3 prompt reversals spread across forums and blogs. Early jailbreak concepts emerge, simulating role switching.

---

## 2022 — Early Exploits and Red Flags

- **February 2022** – First public "DAN" (Do Anything Now) prompts surface on Reddit and Discord, enabling uncensored responses via fictional personas.

- **Mid 2022** – Research discussion begins on the dangers of prompt injection in retrieval-augmented generation (RAG) and template-based agents.

- **September 2022** – OWASP begins formal work on LLM-specific security guidance, identifying prompt injection as the top emerging threat class.

---

## 2023 — Expansion, Public Awareness, and Red Teaming

- **February 2023** – Lakera launches *Gandalf*, a game-like prompt injection challenge. It brings prompt security to a broader audience.

- **March 2023** – GPT-4 released, highlighting new emergent behaviors in prompt handling and hallucination risks.

- **April 2023** – Microsoft publishes *Guidance*, introducing prompt template safety considerations for developers using LLMs in production systems.

- **June 2023** – WithSecure Labs releases *Damn Vulnerable LLM Agent*, a sandbox for chained injection and memory-based compromise testing.

- **August 2023** – Anthropic red team reports document recursive prompt injection and role drift, influencing model design and interface constraints.

- **October 2023** – OWASP publishes the finalized *Top 10 for LLM Applications*, officially listing prompt injection as the top vulnerability.

- **November 2023** – Hugging Face releases the *HackAPrompt Dataset*, aggregating thousands of adversarial examples from live competition prompts.

- **December 2023** – Greshake et al. publish *A Survey of Prompt Injection Attacks and Defenses* (arXiv:2311.16119), becoming the standard academic reference.

---

## 2024 — Tool Maturity and Standardization

- **January 2024** – Release of *Spikee* and *LLMFuzzer*, enabling reproducible fuzzing workflows for adversarial testing of prompt injection vectors.

- **March 2024** – *PromptBench* launched as an open-source benchmark suite to evaluate LLM injection resilience across providers.

- **April 2024** – First public CVEs disclosed for prompt injection in enterprise LLM applications embedded in customer support platforms.

- **June 2024** – Hack The Box releases the *AI Red Teamer* path, offering formal training modules for LLM adversarial testing.

---

## Notable Papers and Technical Reports

- **Greshake et al. (2023)** – *A Survey of Prompt Injection Attacks and Defenses*, arXiv:2311.16119  
- **Stanton et al. (2023)** – *Recursive Injection and Role Drift in LLMs*  
- **Anthropic (2023)** – *LLM Red Teaming Memos: Role Persistence and Leakage*  
- **WithSecure Labs (2023)** – *Chained Prompt Injection in Agent Architectures*  
- **OWASP (2023)** – *Top 10 for Large Language Model Applications*  
- **Hugging Face (2023)** – *HackAPrompt Dataset and Evaluation Framework*

---

## Key Tools and Datasets

| Tool / Dataset           | Release Date | Description                                         |
|--------------------------|---------------|-----------------------------------------------------|
| **Gandalf AI**           | Feb 2023      | Interactive prompt injection challenge platform     |
| **HackAPrompt Dataset**  | Nov 2023      | 10,000+ prompt attack examples from real-world use  |
| **Spikee**               | Jan 2024      | Modular fuzzing framework for adversarial prompts   |
| **LLMFuzzer**            | Mar 2024      | Automated prompt mutation and evaluation tool       |
| **Damn Vulnerable Agent**| Jun 2023      | Sandbox for multi-turn and plugin-based injection   |
| **PromptBench**          | Mar 2024      | Cross-model benchmark suite for injection resilience|

---

## Future Research Directions

- Adversarial alignment testing in autonomous multi-agent chains  
- Content poisoning and indirect injection through public data  
- Formal methods for instruction integrity and trust labeling  
- Real-time prompt context sanitization and boundary enforcement  
- Common standards for red team evaluations across models and vendors

---

## References

- Greshake, T., et al. (2023). *Prompt Injection Survey*. arXiv:2311.16119  
- OWASP Foundation. (2023). *Top 10 for LLM Applications*  
- Simon Willison. (2021–2024). *Prompt Injection and LLM Risk Blog*  
- Anthropic. (2023). *Red Teaming Case Reports*  
- Hugging Face. (2023). *HackAPrompt Dataset*  
- WithSecure. (2023). *Damn Vulnerable LLM Agent and Tooling*

