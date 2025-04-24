# Appendix A – Prompt Injection CTFs and Labs

Adversarial prompt injection and red teaming techniques are best learned through **hands-on exploration**. While many of the examples in this guide are reproducible against sandboxed models, the fastest way to develop real skill is to test your hypotheses in environments **designed to be broken**.

This appendix includes a curated list of Capture-the-Flag (CTF) challenges, vulnerable apps, interactive sandboxes, and open-source projects for practical AI security training.

---

## A.1 Interactive Challenges

### Gandalf – Prompt Injection Game  
**URL**: https://gandalf.lakera.ai/  
A multi-level challenge where you attempt to extract a password from an LLM under increasing guardrails. Each level teaches progressively advanced jailbreak techniques.  
- Great for beginners and intermediate testers  
- Tracks your progress and techniques  
- Leaderboard supported

### Prompting Labs (Immersive Labs)  
**URL**: https://prompting.ai.immersivelabs.com/  
A hands-on web app for learning red teaming, injection, and role hijack tactics.  
- Includes challenge mode and guided learning  
- Designed for security practitioners and SOC teams  
- No account required

### DoubleSpeak  
**URL**: https://doublespeak.chat  
A game-like interface for defeating LLM-based content filters.  
- Each round gives a new challenge and language restriction  
- Great for practicing style transfer, obfuscation, and payload creativity  
- Tracks wins and strategies

---

## A.2 Vulnerable Applications (Open Source)

### AI Goat  
**Repo**: https://github.com/dhammon/ai-goat  
A vulnerable-by-design LLM application created for educational red teaming.  
- Includes realistic RAG pipelines  
- Shows prompt construction templates  
- Compatible with open-weight models and APIs

### Spikee  
**Repo**: https://github.com/WithSecureLabs/spikee  
A Python-based fuzzing and test automation framework for prompt injection.  
- Allows red team scripting and batch mutation  
- Includes prompt seeds and scenario test modules  
- Designed for use with agent and plugin-based systems

### Damn Vulnerable LLM Agent  
**Repo**: https://github.com/WithSecureLabs/damn-vulnerable-llm-agent  
A LangChain-based demo that highlights real-world flaws in agent orchestration.  
- Supports role hijacks, context pollution, and tool-based injection  
- Actively maintained with documented attack examples

### MyLLM Bank  
**URL**: https://myllmbank.com/  
A simulated online banking chatbot designed to be compromised.  
- Contains scenario-based jailbreak challenges  
- Helps train testers on financial system risks  
- Great for testing guardrails and injection bypasses

### MyLLM Doctor  
**URL**: https://myllmdoc.com/  
A vulnerable healthcare AI designed to simulate patient-AI interactions.  
- Focuses on role hijacks, misinformation, and data extraction  
- Excellent for testing ethical boundaries in model response shaping

---

## A.3 Guided Exercises and Academy Paths

### HTB Academy: AI Red Teamer  
**URL**: https://academy.hackthebox.com/path/preview/ai-red-teamer  
A structured training path from Hack The Box focusing on adversarial AI.  
- Covers prompt injection, bypasses, and output manipulation  
- Requires free HTB account  
- Offers labs and quizzes with solutions

---

## A.4 Prompt Challenge Sites

### Prompt Airlines  
**URL**: https://promptairlines.com/  
A community challenge board offering new prompt injection puzzles each week.  
- Tracks leaderboard scores  
- Includes payload-sharing community  
- Good source of creative inspiration

### GPT Prompt Attack  
**URL**: https://gpa.43z.one/  
A high-signal testing interface for prompt injection and content filtering.  
- Easy to test filters in GPT-4/GPT-3.5  
- Clean interface with output debugging  
- Open-ended sandbox environment

---

## A.5 Recommendations

| Use Case                      | Resource                                     |
|------------------------------|----------------------------------------------|
| Total beginner               | Gandalf, Prompting Labs                      |
| Guided red teaming track     | HTB Academy – AI Red Teamer                  |
| Open-source app exploitation | AI Goat, DVLLM Agent                         |
| Injection fuzzing            | Spikee, FuzzLLM (advanced)                   |
| Healthcare AI simulation     | MyLLM Doctor                                 |
| Financial LLM simulation     | MyLLM Bank                                   |
| Weekly challenge practice    | Prompt Airlines, DoubleSpeak                 |

---

## A.6 Operational Advice

- Always test in **authorized or simulated environments**
- Save and categorize payloads that succeed
- Build a rotation schedule to stay sharp (e.g., 3 prompts/day)
- Contribute to open-source labs if you develop novel attack chains
- Use these challenges to train others—internally or publicly

---

## References

- Lakera Labs. (2023). *Gandalf: Prompt Injection Challenge*  
- Immersive Labs. (2023). *Prompting Labs Platform*  
- WithSecure. (2023). *Damn Vulnerable LLM Agent & Spikee*  
- D. Hammon. (2023). *AI Goat – Vulnerable AI App Demo*  
- Hack The Box. (2024). *AI Red Teamer Path*

