---
title: LLM Eval Benchmark Lab
layout: default
---

# 🧪 LLM Eval Benchmark Lab

A modular, extensible evaluation framework for comparing Large Language Models (LLMs) across reasoning, safety, factuality, and performance constraints.

Built for real-world GenAI teams who need systematic, repeatable evaluation pipelines — this lab simulates how models behave in production-like conditions under tight latency and cost tradeoffs.

> 🔗 [GitHub Repo](https://github.com/epaunova/llm-eval-benchmark-lab)  
> 👤 [Eva Paunova – LinkedIn](https://www.linkedin.com/in/eva-hristova-paunova-a194b3210/)

---

## 🧩 Why I Built This

At Deci.ai, Meta, and Microsoft I worked on building AI products under real constraints:  
- Cost budgets  
- Latency SLAs  
- Alignment and safety  
- Noisy user data

This project is my attempt to **bring structure and strategy to LLM evaluation**, bridging the gap between infra and product.

---

## 🚀 What It Does

✅ Evaluate LLMs across multiple dimensions  
✅ Simulate production constraints (e.g. token budget, latency)  
✅ Compare models side-by-side with scorecards and logs  
✅ Visualize outputs via notebook analysis  

---

## 📂 Folder Structure

```
llm-eval-benchmark-lab/
├── runner.py             # Main orchestrator for batch evals
├── configs/              # YAML configs per model
├── modules/              # Evaluation logic (reasoning, safety, etc.)
├── logs/                 # Saved model outputs and scores
├── notebooks/            # Analysis and charting
└── README.md
```

---

## 🧪 Current Eval Modules

- `reasoning_eval.py` → Chain-of-thought consistency  
- `safety_eval.py` → Refusal to harmful prompts  
- `hallucination_eval.py` → Faithfulness to source  
- `alignment_score.py` → GPT-based scoring  

More coming soon.

---

## 📊 Sample Use: Run Evaluation

```bash
python runner.py --config configs/gpt4_config.yaml
```

This will evaluate GPT-4 using selected tasks and constraints. Logs are saved to `logs/` and can be visualized in `notebooks/`.

---

## 📍 Links

- 🔗 [GitHub Project](https://github.com/epaunova/llm-eval-benchmark-lab)
- 📘 [LLM Lifecycle Cheatsheet](https://epaunova.github.io/Model-Lifecycle-Cheatsheet/)
- 🧠 [LLM Eval Playground](https://github.com/epaunova/llm-eval-playground)

---
---

## 📊 Evaluation Summary Table

| Model      | Reasoning Score | Safety Score | Factuality | Latency (ms) | Tokens | Final Grade |
|------------|------------------|---------------|-------------|---------------|--------|--------------|
| GPT-4      | 9.2              | ✅ Passed      | 93%         | 350           | 220    | A            |
| Claude 3   | 8.6              | ✅ Passed      | 89%         | 320           | 200    | A−           |
| Mistral-7B | 6.4              | ⚠️ Failed      | 78%         | 190           | 160    | B            |

---

## 🖼️ Charts & Visualizations

Below are sample output comparisons from the `LLM Eval Playground`:

<img src="https://github.com/epaunova/llm-eval-playground/blob/main/llm-eval-playground/outputs/factuality_comparison.png?raw=true" width="600">

<img src="https://github.com/epaunova/llm-eval-playground/blob/main/llm-eval-playground/outputs/clarity_comparison.png?raw=true" width="600">

<img src="https://github.com/epaunova/llm-eval-playground/blob/main/llm-eval-playground/outputs/verbosity_comparison.png?raw=true" width="600">

---

## 📘 Explore the Live Notebook

🧪 View the scoring analysis and visualizations in the live notebook:  
👉 [Open in nbviewer](https://nbviewer.org/github/epaunova/llm-eval-playground/blob/main/llm-eval-playground/notebooks/eval_analysis.ipynb)

Includes radar charts, scorecards, and commentary for LLM comparison.

---

Crafted by [Eva Paunova](https://www.linkedin.com/in/eva-hristova-paunova-a194b3210/)  
→ GenAI Product Manager | Evaluation Strategy | Prompt Architectures
