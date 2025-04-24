# Appendix B – Tooling Index for Red Teamers

Prompt injection, role hijacking, and systemic LLM testing benefit from automation and repeatability. The following tools enable red teamers to:

- Generate mutated payloads
- Automate LLM probing and behavior logging
- Manage multi-turn sessions with context memory
- Evaluate output for filter bypasses or behavioral shifts
- Structure reproducible attack testbeds

This appendix catalogs production-grade tools across categories, with links, primary use cases, and integration notes.

---

## B.1 Fuzzing and Payload Mutation

### Spikee  
**Repo**: https://github.com/WithSecureLabs/spikee  
A full-featured red team fuzzing framework for LLM agent chains.  
- Supports direct, recursive, and indirect injection scenarios  
- Configurable payload mutation strategies  
- Designed for agent-based systems with memory and tools

### LLMFuzzer  
**Repo**: https://github.com/s0md3v/LLMFuzzer  
A lightweight prompt fuzzer designed to evade filters and test payload impact.  
- CLI-based interface  
- Easy to extend with new injection types  
- Includes evasion logic and output validation heuristics

### FuzzLLM  
**Repo**: https://github.com/cyc1ing/FuzzLLM  
Fuzzer with RL-guided mutation strategies for adversarial prompt crafting.  
- Uses scoring feedback to guide payload selection  
- Suitable for batch model evaluation  
- Python-based orchestration

---

## B.2 Prompt Generators and Payload Libraries

### AutoDAN  
**Repo**: https://github.com/mxrch/AutoDAN  
Script to generate variants of the DAN (Do Anything Now) jailbreak prompt.  
- Simple CLI tool for generating DAN payloads at scale  
- Good for training and regression testing

### DAN-Sploit  
**Repo**: https://github.com/Bin-Huang/dan-sploit  
Toolkit to mutate and encode prompt payloads for filter evasion.  
- Supports ROT13, Base64, homoglyph substitution  
- Output payloads suitable for downstream fuzzing

### PromptPerfect (Commercial)  
**URL**: https://promptperfect.jina.ai/  
Web-based interface to test prompt variation and formatting sensitivity.  
- Useful for instructional tone shaping  
- Less suited to offensive research, but good for pre-injection conditioning

---

## B.3 LLM Wrapper and Prompt Debugging Utilities

### LangChain Prompt Inspector  
**URL**: https://smith.langchain.com/  
Web UI for visualizing prompt construction, context splitting, and agent planning logic.  
- Essential for identifying where user-controlled input enters the prompt  
- Supports inspection of internal prompt formatting

### PromptFoo  
**Repo**: https://github.com/promptfoo/promptfoo  
CLI and dashboard for testing prompts across multiple models and conditions.  
- Supports assertions, benchmarks, and A/B testing  
- Useful for comparing jailbreak success rates across targets

### OpenLLMetry  
**Repo**: https://github.com/langfuse/openllmetry  
Monitoring, logging, and evaluation toolkit for LLM apps.  
- Tracks success/failure of jailbreak attempts over time  
- Compatible with OpenAI, Cohere, Anthropic, open-weight models

---

## B.4 Testing Interfaces

### RedTeaming-GPT  
**Repo**: https://github.com/maltron/RedTeaming-GPT  
A CLI wrapper that logs attack attempts and outputs.  
- Lightweight and scriptable  
- Good for payload prototyping and log capture

### PromptBench (Research-grade)  
**Repo**: https://github.com/evalplus/promptbench  
Framework for LLM prompt evaluation with multi-dimensional metrics.  
- Academic focus  
- Supports filter bypass, alignment deviation, and robustness scoring

---

## B.5 Agent and RAG-Specific Testing Tools

### DVLLM Agent  
**Repo**: https://github.com/WithSecureLabs/damn-vulnerable-llm-agent  
A vulnerable LangChain-based chatbot with modular prompt injection surfaces.  
- Ideal for testing chained role hijack, tool command override, recursive memory injection  
- Supports plugin and toolchain testing

### RAGatouille  
**Repo**: https://github.com/hwchase17/ragatouille  
A RAG pipeline testing framework.  
- Simulates document injection into context  
- Useful for testing indirect prompt injection via retrieval layer

---

## B.6 Additional Resources and Utilities

| Tool / Repo                | Use Case                                  |
|---------------------------|--------------------------------------------|
| [`Text-attack`](https://github.com/QData/TextAttack) | NLP adversarial sample generator (useful for obfuscated LLM input) |
| [`AdvPrompt`](https://github.com/thunlp/AdvPrompt)   | Prompt optimization and adversarial mutation research               |
| [`promptinject`](https://github.com/llm-attacks/promptinject) | Python module for basic injection templates                        |
| [`CAPE`](https://github.com/AI-secure/CAPE)          | Evaluation of model robustness via adversarial prompting           |

---

## B.7 Operational Recommendations

- Maintain your own payload testbed and mutation logs  
- Combine CLI tools with centralized logging for analysis  
- Version control successful payloads with metadata  
- Incorporate LLM wrappers into CI for regression testing  
- Build RAG + Agent simulators to test end-to-end pipelines

---

## References

- WithSecure. (2023). *Spikee and DVLLM Agent*  
- S0md3v. (2023). *LLMFuzzer: Prompt Fuzzing Toolkit*  
- LangChain. (2024). *Prompt Inspector and Agent Debugging Tools*  
- EvalPlus. (2023). *PromptBench Benchmarking Framework*  
- OpenAI and Anthropic. (2023). *Best Practices for Prompt Security Audits*

