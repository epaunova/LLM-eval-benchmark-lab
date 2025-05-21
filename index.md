---

# 🧪 LLM Eval Benchmark Lab

A modular evaluation system for GenAI teams who need structured model comparison across reasoning, safety, and latency tradeoffs.

> Built by Eva Paunova – [GitHub](https://github.com/epaunova) | [LinkedIn](https://www.linkedin.com/in/eva-hristova-paunova-a194b3210/)

---

## 🧩 Why I Built This

At Deci.ai, Meta, and Microsoft I worked on building AI products under real constraints:  
- Cost budgets  
- Latency SLAs  
- Alignment and safety  
- Noisy user data

This project brings structure and strategy to LLM evaluation, bridging the gap between infra and product.

---

## 🚀 What It Does

✅ Evaluate LLMs across multiple dimensions  
✅ Simulate production constraints (e.g. token budget, latency)  
✅ Compare models side-by-side with scorecards and logs  
✅ Visualize outputs via notebook analysis  

---

## 📂 Folder Structure

llm-eval-benchmark-lab/
├── runner.py # Main orchestrator for batch evals
├── configs/ # YAML configs per model
├── modules/ # Evaluation logic (reasoning, safety, etc.)
├── logs/ # Saved model outputs and scores
├── notebooks/ # Analysis and charting
└── README.md

yaml
Copy
Edit

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
