# Hacking AI: The Definitive Guide

**Prompt Injection, Jailbreaking, and Offensive Techniques for Large Language Models**

This guide is a comprehensive technical manual for understanding and exploiting the vulnerabilities of modern large language models (LLMs). It is intended for security professionals, researchers, red teamers, and adversarial ML practitioners who require a clear, structured, and reproducible approach to prompt-based attacks and system behavior analysis.

No hype. No marketing. Just the techniques.

---

## ⚠️ Disclaimer

This book is intended **solely for educational and research purposes**. It covers adversarial prompt engineering, red teaming, and security testing techniques used to evaluate the robustness of LLM-based systems.

By using this material, you agree to the terms outlined in the [DISCLAIMER.md](DISCLAIMER.md).

- Do **not** apply these techniques to any system you do not own or have explicit permission to test.
- Unauthorized use may violate laws such as the CFAA, DMCA, and international equivalents.
- The authors and contributors accept **no liability** for misuse or legal consequences.

> This is a guide for building safer AI systems—not breaking them irresponsibly.

---

## Scope

This guide covers:

- Prompt injection and prompt-based adversarial control
- Jailbreaking LLMs using identity manipulation, obfuscation, and recursion
- Extraction of hidden system instructions and memory state
- Attacks on multi-turn, context-aware, and agent-based systems
- Obfuscation and filter evasion strategies
- Red team workflows, fuzzing tools, and payload libraries
- Ethics, documentation, and responsible disclosure

It includes practical examples, offensive reasoning, and reproducible tactics based on current model behavior and publicly known vulnerabilities.

---

## Who This Is For

- LLM red teamers
- Security researchers
- Offensive AI engineers
- Prompt injection analysts
- Developers testing LLM-based systems under adversarial conditions

---

## Format

The book is structured into four parts:

1. **Foundations** — LLM architecture, prompt execution, and threat models
2. **Core Exploits** — Practical injection and manipulation techniques
3. **Advanced Techniques** — Recursive, contextual, and tool-assisted attacks
4. **Red Team Operations** — Payload development, fuzzing, and disclosure

Additional appendices include labs, tools, a glossary, and a research timeline.

---

## Table of Contents

| #   | Chapter Title                                               |
|-----|-------------------------------------------------------------|
| 01  | [What is Prompt Injection (and Why It Matters)](chapters/01-what-is-prompt-injection.md)  
| 02  | [LLM Architecture, Context Windows, and Memory Models](chapters/02-llm-architecture-context.md)  
| 03  | [Trust Boundaries in Prompt-Based Systems](chapters/03-trust-boundaries.md)  
| 04  | [System Prompts: The Hidden Root of Behavior](chapters/04-system-prompts.md)  
| 05  | [The Psychology of LLMs: Reasoning, Simulation, and Compliance](chapters/05-psychology-of-llms.md)  
| 06  | [Basic Prompt Injection: Ignoring Instructions and Overriding Behavior](chapters/06-basic-injection.md)  
| 07  | [Role Hijacks and Identity Subversion](chapters/07-role-hijacks.md)  
| 08  | [System Prompt Extraction](chapters/08-system-prompt-leaks.md)  
| 09  | [Obfuscation and Encoding](chapters/09-obfuscation.md)  
| 10  | [Direct Override: Replacing the System Prompt](chapters/10-direct-override.md)  
| 11  | [Multi-Turn Memory Corruption](chapters/11-multi-turn-corruption.md)  
| 12  | [Recursive Injection: Echo-Based Exploits](chapters/12-recursive-injection.md)  
| 13  | [Indirect Prompt Injection: Attacks via Third-Party Context](chapters/13-indirect-injection.md)  
| 14  | [Chaining Abuse in RAG, Agents, and Plugins](chapters/14-chaining-and-rag.md)  
| 15  | [Style Transfer Attacks and Tone Injection](chapters/15-style-transfer.md)  
| 16  | [Red Team Recon: Mapping Filters, Capabilities, and Roles](chapters/16-recon.md)  
| 17  | [Payload Libraries and Injection Mutation Strategies](chapters/17-payload-libraries.md)  
| 18  | [Fuzzing and Tooling for Prompt Exploitation](chapters/18-fuzzing-and-tools.md)  
| 19  | [Exploit Reporting and Reproducibility](chapters/19-exploit-reporting.md)  
| 20  | [Disclosure, Ethics, and Adversarial Red Teaming](chapters/20-disclosure-and-ethics.md)  

### 📁 Appendices
- [A. Prompt Injection CTFs and Labs](chapters/appendix-a-ctfs.md)  
- [B. Tooling Index for Red Teamers](chapters/appendix-b-tools.md)  
- [C. Glossary of Adversarial AI Terms](chapters/appendix-c-glossary.md)  
- [D. Timeline of Research and Prompt Injection Discoveries](chapters/appendix-d-research-timeline.md)

---

## License

This work is licensed under **Creative Commons Attribution-NonCommercial 4.0 (CC BY-NC 4.0)**.  
You may share and adapt this material with attribution, but commercial use is prohibited without permission.

---

## Status

This guide is in active development. Chapters will be written and published in order, with a focus on accuracy, depth, and reproducibility. Contributions and peer review are welcome.
