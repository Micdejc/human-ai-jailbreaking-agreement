# Multi-Turn Cybersecurity Jailbreak Evaluation for Large Language Models

This repository provides code, datasets, and analysis scripts for systematically assessing the alignment between automated LLM evaluators and human judgments under multi-turn conversational scenarios in cybersecurity.

This study builds upon **[Grammatical Mirage Attack](https://github.com/Micdejc/llm_multiturn_attacks/)** for perform the multi-turn attacks against targeted models.

---

## 📄 Overview

Automated evaluation of LLM safety and jailbreak resilience is increasingly common, yet its agreement with human judgment remains uncertain, especially for **multi-turn dialogues** and **temporal variations** in prompts.

This study evaluates **four automated evaluators**:

- **GPT-4.1**  
- **GPT-5.2**  
- **Llama Guard 3**  
- **Rule-based classifier (GCG)**  

against **human annotators** across:

- Two target models: **Llama 2-7B** and **Qwen 2-7B**  
- Multi-turn dialogues of varying depths  
- Temporal prompt variations (**present vs past tense**)  
- Cybersecurity-related topics  

Performance metrics include:

- **Cohen’s κ** for inter-annotator agreement  
- **F1-score** as a complementary measure  

---

## 🔑 Key Findings

- **Weak human–machine alignment**: Automated evaluators have κ values **below 0.36** across all multi-turn conditions.  
- **Temporal prompt impact**: Past-tense prompts significantly reduce agreement (κ drops by 0.11–0.48).
- **Malware-related prompts are the most challenging**: Across cybersecurity topics, malware discussions show the **lowest evaluator reliability**, highlighting domain-specific challenges.  

**Conclusion:** Current automated evaluators are insufficiently aligned with human judgment, highlighting the need for **human-centered evaluation** in multi-turn jailbreak benchmarking.

---

## Ethical Consideration

This project is intended solely for research purposes and must not be used for malicious, harmful, or unethical activities.
