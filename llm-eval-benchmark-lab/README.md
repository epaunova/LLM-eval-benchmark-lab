# LLM Eval Benchmark Lab

A modular benchmarking framework for evaluating large language models across reasoning, factuality, safety, and other critical dimensions. Designed for GenAI product managers and research teams who need systematic, repeatable evaluation pipelines.

## Key Components

- **Modular Eval Tasks**: Plug-and-play modules for different tasks (e.g., reasoning, factuality, safety)
- **Constraint-Aware Configs**: Evaluate models under conditions like latency, context length, and token limits
- **Scoring Framework**: Supports GPT-graded, rule-based, and human-loop evaluations
- **Dashboarding**: Notebook-based analytics for model comparison and tradeoff visualization

## Folder Structure

- `modules/`: task-specific eval logic
- `configs/`: per-model eval configuration
- `logs/`: raw outputs, token counts, latency
- `notebooks/`: analysis and visualization

## Example Use Case

Compare GPT-4, Claude 3, and Mistral across:
- Multi-step reasoning under 200-token limit
- Politeness + refusal behavior
- Latency-to-score ratio in summarization

## Quick Start

```bash
python runner.py --config configs/gpt4_config.yaml
```

---
> Created by Eva Paunova | GitHub: [epaunova](https://github.com/epaunova)
