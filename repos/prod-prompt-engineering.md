# Prompt Engineering in Production

A hands-on production framework for building, testing, versioning, and securing prompts across multiple LLMs. Not a tutorial — a working system you can deploy.

## What This Repo Covers

- Prompt Registry — versioned prompt files (YAML/JSON) with metadata: version, author, use case, model target
- Prompt Testing Harness — runs the same prompt across GPT-4o, Claude 3.5, Gemini Flash, logs outputs and scores them
- Evaluation Metrics — response length consistency, hallucination flags, latency per model, cost per 1000 calls
- System Prompt Stress Tester — injects adversarial inputs, edge cases, and role-break attempts, logs failure modes
- Prompt Diff Tool — compares v1 vs v2 of a prompt against the same test set, shows output behaviour changes
- Dashboard — CLI and Streamlit output showing eval results across versions and models

## What You Will Learn by Building It

- Why prompts are code and must be versioned, tested, and monitored like code
- How tokenisation silently breaks prompts at scale
- How the same prompt behaves differently across GPT-4o, Claude, and Gemini
- How to defend against prompt injection and system prompt leakage
- How to reduce cost and latency through prompt design without losing quality

## Who It Is For

- AI Engineers building production LLM applications
- Engineers who want to move beyond "vibe prompting" into systematic prompt engineering
- Builders who want a real framework they can fork and extend into their own systems

## Start Here

- Clone the repo and set up your `.env` with API keys for OpenAI, Anthropic, and Google
- Start with `prompts/registry/` — understand the versioning structure before running anything
- Run `tests/harness.py` against the example prompt to see multi-model evaluation in action

**GitHub Repository:**  
[Access the repo here](https://github.com/saiharsha-k/prod-prompt-engineering)
