# Vibe Coding + Vibe Research for LLM Research: Tutorial Resources

> **Tutorial by Zhaochen Su, HKUST CSE | February 2026**
>
> A curated list of papers, blogs, and tools for the tutorial on AI-augmented coding and research workflows in LLM research.

---

## Table of Contents

- [1. Vibe Coding: Origin & Overview](#1-vibe-coding-origin--overview)
- [2. AI Coding Tools](#2-ai-coding-tools)
- [3. Vibe Research & Automated Scientific Discovery](#3-vibe-research--automated-scientific-discovery)
- [4. Key Academic Papers](#4-key-academic-papers)
- [5. Benchmarks & Evaluation](#5-benchmarks--evaluation)
- [6. Deep Research Tools](#6-deep-research-tools)
- [7. Practical Guides & Best Practices](#7-practical-guides--best-practices)
- [8. Further Reading](#8-further-reading)

---

## 1. Vibe Coding: Origin & Overview

### The Origin

- **Andrej Karpathy's Tweet (Feb 3, 2025)** — The tweet that coined "vibe coding" (6.7M+ views): *"There's a new kind of coding I call 'vibe coding', where you fully give in to the vibes, embrace exponentials, and forget that the code even exists."*
  - [Original Tweet](https://x.com/karpathy/status/1886192184808149383)

- **Karpathy's 2025 LLM Year in Review** — Reflection on how vibe coding became a cultural phenomenon, how it empowers both beginners and professionals, and the shift toward "agentic engineering."
  - [Blog Post](https://karpathy.bearblog.dev/year-in-review-2025/)

- **"Vibe coding" named Collins Dictionary Word of the Year 2025**

### Survey & Analysis

- **"A Survey of Vibe Coding with Large Language Models"** (Ge et al., Oct 2025) — The first comprehensive survey of vibe coding, analyzing 1000+ papers. Formalizes vibe coding as a Constrained MDP and proposes a taxonomy of five development models (Unconstrained Automation, Iterative Conversational, Planning-Driven, Test-Driven, Context-Enhanced).
  - [arXiv:2510.12399](https://arxiv.org/abs/2510.12399)

- **Vibe Coding — Wikipedia** — Community-maintained overview with history and criticisms.
  - [Wikipedia](https://en.wikipedia.org/wiki/Vibe_coding)

### From Vibe Coding to Agentic Engineering

- **"Vibe Coding is Passe"** (The New Stack, 2026) — Karpathy moves on from "vibe coding" to "agentic engineering", emphasizing that developers now orchestrate agents rather than write code directly.
  - [The New Stack](https://thenewstack.io/vibe-coding-is-passe/)

---

## 2. AI Coding Tools

### Cursor

| | |
|---|---|
| **Website** | [cursor.com](https://cursor.com) |
| **Type** | AI-native IDE (VS Code fork) |
| **Key Feature** | Composer (multi-file editing), Agent mode, @-mentions |

- **Cursor 2.0 Ultimate Guide** — Covers multi-agent workflow, Composer, aggregated diffs. [Skywork AI Blog](https://skywork.ai/blog/vibecoding/cursor-2-0-ultimate-guide-2025-ai-code-editing/)
- **Cursor AI Complete Guide: MCPs, Rules & Context Engineering** — Practical tips on `.cursor/rules/`, MCP setup, context management. [Medium](https://medium.com/@hilalkara.dev/cursor-ai-complete-guide-2025-real-experiences-pro-tips-mcps-rules-context-engineering-6de1a776a8af)
- **"How I Use Cursor (+ My Best Tips)"** — Test-driven AI dev, Command K shortcuts, agent babysitting. [Builder.io](https://www.builder.io/blog/cursor-tips)
- **Cursor AI Deep Dive: Architecture & Best Practices** — Technical architecture, security, enterprise features. [Collabnix](https://collabnix.com/cursor-ai-deep-dive-technical-architecture-advanced-features-best-practices-2025/)

### Claude Code

| | |
|---|---|
| **Website** | [docs.anthropic.com/en/docs/claude-code](https://docs.anthropic.com/en/docs/claude-code) |
| **GitHub** | [github.com/anthropics/claude-code](https://github.com/anthropics/claude-code) |
| **Type** | Agentic CLI tool |
| **Key Feature** | Autonomous multi-step execution, bash/edit/search tools, sub-agents |

- **Introduction to Agentic Coding** (Anthropic official) — Moving from fragmented AI snippets to integrated agentic development. [Blog](https://claude.com/blog/introduction-to-agentic-coding)
- **Claude Code Tutorial** — Step-by-step walkthrough. [Medium](https://medium.com/aimonks/claude-code-tutorial-80037240aaab)
- **Claude Code 2.0 Experience & Tips** — Practical advice on getting better at using coding agents. [Sankalp's Blog](https://sankalp.bearblog.dev/my-experience-with-claude-code-20-and-how-to-get-better-at-using-coding-agents/)
- **Claude Code Beginner to Pro Guide (2026)** — Installation, CLAUDE.md, Plan Mode, comparison with other tools. [codewithmukesh](https://codewithmukesh.com/blog/claude-code-for-beginners/)
- **Building Agents with Claude Agent SDK** — How to build custom agents on top of Claude Code's capabilities. [Anthropic Engineering](https://www.anthropic.com/engineering/building-agents-with-the-claude-agent-sdk)

### GitHub Copilot

| | |
|---|---|
| **Website** | [github.com/features/copilot](https://github.com/features/copilot) |
| **Type** | IDE plugin (inline completion + agent mode) |

### Windsurf

| | |
|---|---|
| **Website** | [windsurf.com](https://windsurf.com) |
| **Type** | Agentic IDE (VS Code fork, formerly Codeium) |
| **Key Feature** | Cascade agent for deep codebase understanding |

- **Windsurf Review (2026)** — Detailed review of features and use cases. [vibecoding.app](https://vibecoding.app/blog/windsurf-review)
- **Windsurf vs Cursor Comparison** — Head-to-head comparison. [Builder.io](https://www.builder.io/blog/windsurf-vs-cursor)

### Aider

| | |
|---|---|
| **Website** | [aider.chat](https://aider.chat) |
| **GitHub** | [github.com/paul-gauthier/aider](https://github.com/paul-gauthier/aider) |
| **Type** | CLI, git-aware, model-agnostic |

### Cline

| | |
|---|---|
| **Website** | [cline.bot](https://cline.bot) |
| **Type** | Open-source VS Code extension, plan-then-act |

- **Top 6 Claude Code Alternatives** — Comparison of CLI/agent coding tools. [Cline Blog](https://cline.bot/blog/top-6-claude-code-alternatives-for-agentic-coding-workflows-in-2025)

### Devin

| | |
|---|---|
| **Website** | [devin.ai](https://devin.ai) |
| **Type** | Fully autonomous cloud agent |

### Tool Comparisons

- **AI Coding Agent Showdown: 10 Top Tools Compared** — Comprehensive benchmark of Cursor, Claude Code, Cline, Aider, Devin, and more. [Patrick Hulce](https://blog.patrickhulce.com/blog/2025/ai-code-comparison)
- **Best AI Coding IDE 2025: Cursor vs Claude Code vs Windsurf** — Feature-by-feature comparison. [HumAI](https://www.humai.blog/best-ai-coding-ide-2025-cursor-vs-antigravity-vs-claude-code-vs-windsurf-the-complete-comparison/)
- **10 Things Developers Want from Agentic IDEs in 2025** — Industry analysis from RedMonk. [RedMonk](https://redmonk.com/kholterhoff/2025/12/22/10-things-developers-want-from-their-agentic-ides-in-2025/)
- **Agentic Coding Tools Setup Guide** — Claude Code, Aider, and CLI-based AI development. [iKangai](https://www.ikangai.com/agentic-coding-tools-explained-complete-setup-guide-for-claude-code-aider-and-cli-based-ai-development/)

---

## 3. Vibe Research & Automated Scientific Discovery

### The AI Scientist

End-to-end automated research: idea generation → code → experiments → paper writing.

- **The AI Scientist v1** (Lu et al., Aug 2024) — First comprehensive framework for fully automated scientific discovery. Uses frontier LLMs to perform research independently.
  - [arXiv:2408.06292](https://arxiv.org/abs/2408.06292) | [Blog](https://sakana.ai/ai-scientist/) | [GitHub](https://github.com/SakanaAI/AI-Scientist)

- **The AI Scientist v2** (Yamada et al., Apr 2025) — Workshop-level automated discovery via agentic tree search. Produced the **first AI-generated peer-review-accepted paper** at an ICLR workshop. Eliminates human-provided code templates.
  - [arXiv:2504.08066](https://arxiv.org/abs/2504.08066)

### Agent Laboratory

- **Agent Laboratory** (Schmidgall et al., Jan 2025) — Autonomous LLM-based framework that completes the entire research process: literature review → experimentation → report writing. Supports autonomous and co-pilot modes. 84% cost reduction vs. previous methods.
  - [arXiv:2501.04227](https://arxiv.org/abs/2501.04227) | [GitHub](https://github.com/SamuelSchmidgall/AgentLaboratory) | [Project Page](https://agentlaboratory.github.io/)

### AIDE (Weco AI)

- **AIDE: AI-Driven Exploration in the Space of Code** (Schmidt, Srikanth et al., Feb 2025) — Frames ML engineering as code optimization via tree search. State-of-the-art on Kaggle, MLE-Bench, and RE-Bench. Adopted by researchers at Meta, DeepMind, Sakana AI.
  - [arXiv:2502.13138](https://arxiv.org/abs/2502.13138) | [GitHub](https://github.com/WecoAI/aideml)

### Vibe Research Concept

- **"Vibe-Research instead of Deep-Research"** — AI agents proactively drive the research process (literature mining, ideation, multi-agent coordination) rather than just responding to prompts.
  - [Medium](https://medium.com/@abertina/vibe-research-instead-of-deep-research-ai-agents-and-the-future-of-scientific-discovery-4d561248f3e2)

---

## 4. Key Academic Papers

### Vibe Coding & AI-Assisted Development

| Paper | Authors | Year | Link |
|-------|---------|------|------|
| A Survey of Vibe Coding with Large Language Models | Ge et al. | 2025 | [arXiv:2510.12399](https://arxiv.org/abs/2510.12399) |
| SWE-bench: Can Language Models Resolve Real-World GitHub Issues? | Jimenez et al. | 2024 | [arXiv:2310.06770](https://arxiv.org/abs/2310.06770) (ICLR 2024 Oral) |

### Automated Scientific Discovery

| Paper | Authors | Year | Link |
|-------|---------|------|------|
| The AI Scientist: Towards Fully Automated Open-Ended Scientific Discovery | Lu, Lu, Lange et al. | 2024 | [arXiv:2408.06292](https://arxiv.org/abs/2408.06292) |
| The AI Scientist-v2: Workshop-Level Automated Scientific Discovery via Agentic Tree Search | Yamada et al. | 2025 | [arXiv:2504.08066](https://arxiv.org/abs/2504.08066) |
| Agent Laboratory: Using LLM Agents as Research Assistants | Schmidgall et al. | 2025 | [arXiv:2501.04227](https://arxiv.org/abs/2501.04227) |
| AIDE: AI-Driven Exploration in the Space of Code | Schmidt, Srikanth et al. | 2025 | [arXiv:2502.13138](https://arxiv.org/abs/2502.13138) |

### LLMs for Research Ideation

| Paper | Authors | Year | Link |
|-------|---------|------|------|
| Can LLMs Generate Novel Research Ideas? A Large-Scale Human Study with 100+ NLP Researchers | Si, Yang, Hashimoto | 2024 | [arXiv:2409.04109](https://arxiv.org/abs/2409.04109) (ICLR 2025) |

### Surveys on AI for Science

| Paper | Authors | Year | Link |
|-------|---------|------|------|
| Agentic AI for Scientific Discovery: A Survey of Progress, Challenges, and Future Directions | — | 2025 | [arXiv:2503.08979](https://arxiv.org/abs/2503.08979) |
| From AI for Science to Agentic Science: A Survey on Autonomous Scientific Discovery | — | 2025 | [arXiv:2508.14111](https://arxiv.org/abs/2508.14111) |

---

## 5. Benchmarks & Evaluation

| Benchmark | What It Measures | Link |
|-----------|-----------------|------|
| **SWE-bench** | Can LLMs resolve real GitHub issues? | [swebench.com](https://www.swebench.com) |
| **SWE-bench Verified** | Human-validated subset (500 tasks) | [OpenAI Blog](https://openai.com/index/introducing-swe-bench-verified/) |
| **MLE-bench** (OpenAI) | ML engineering on Kaggle competitions | [OpenAI](https://openai.com/index/mle-bench/) |
| **RE-Bench** (METR) | Research engineering tasks | [METR](https://metr.org/) |

---

## 6. Deep Research Tools

Tools for AI-augmented literature review and research synthesis.

| Tool | Provider | Key Strength |
|------|----------|-------------|
| **Deep Research** | Google (Gemini) | Web search + synthesis, good source accuracy |
| **Deep Research** | OpenAI (ChatGPT Pro) | Detailed long-form reports |
| **Perplexity** | Perplexity AI | Real-time web search with citations |
| **Elicit** | Elicit | Academic paper search & extraction |
| **Semantic Scholar** | Allen AI | Academic search API, citation graphs |
| **NotebookLM** | Google | Upload papers, ask questions, generate summaries |

### Deep Research Evaluation

- **"Deep Research for Scientific Literature Review"** — Compares Gemini vs OpenAI for academic literature review; Gemini finds more recent papers, OpenAI provides more detail but can hallucinate references. [Blog](https://xiangyu-yin.com/content/post_deep_research.html)
- **"Deep Research and Open Access"** — OpenAI largely hallucinated references; Gemini and Perplexity did not. [Andrew Wheeler](https://andrewpwheeler.com/2025/08/28/deep-research-and-open-access/)
- **Evaluation Sheet for Deep Research** (arXiv, Sep 2025) — Formal evaluation framework for AI-generated research reports. [arXiv:2510.01283](https://arxiv.org/abs/2510.01283)

---

## 7. Practical Guides & Best Practices

### For Vibe Coding

1. **Be specific in prompts** — "Add LoRA rank=16 to attention layers" >> "Add LoRA"
2. **Set up project context** — Use `CLAUDE.md`, `.cursorrules`, or `.github/copilot-instructions.md`
3. **Write tests first** — Let AI implement against your test spec
4. **Commit frequently** — AI makes big changes; small commits help rollback
5. **Paste errors directly** — AI is excellent at debugging from stack traces
6. **Match vibe level to risk** — Careful review for training code; full vibe for plotting scripts

### For Vibe Research

1. **Always verify citations** — LLMs can hallucinate paper titles, authors, and results
2. **Use AI for breadth, yourself for depth** — AI surveys widely, you analyze deeply
3. **Cross-check across models** — Compare Claude, GPT, Gemini outputs on important claims
4. **AI writes the first draft, you write the final draft** — Keep your unique insight
5. **Be transparent** — Disclose AI assistance in papers

### Recommended Blog Posts

- **"How I Use Cursor (+ My Best Tips)"** — [Builder.io](https://www.builder.io/blog/cursor-tips)
- **"Getting Started with Cursor AI"** — [emgoto.com](https://www.emgoto.com/cursor/)
- **Claude Code Tutorial** — [Medium](https://medium.com/aimonks/claude-code-tutorial-80037240aaab)
- **Agentic Coding Tools Setup Guide** — [iKangai](https://www.ikangai.com/agentic-coding-tools-explained-complete-setup-guide-for-claude-code-aider-and-cli-based-ai-development/)

---

## 8. Further Reading

- **Karpathy's 2025 LLM Year in Review** — [Blog](https://karpathy.bearblog.dev/year-in-review-2025/)
- **Sebastian Raschka's LLM Research Papers List (2024)** — [Newsletter](https://magazine.sebastianraschka.com/p/llm-research-papers-the-2024-list)
- **Sebastian Raschka's LLM Research Papers List (2025 H1)** — [Newsletter](https://magazine.sebastianraschka.com/p/llm-research-papers-2025-list-one)
- **Sebastian Raschka's LLM Research Papers List (2025 H2)** — [Newsletter](https://magazine.sebastianraschka.com/p/llm-research-papers-2025-part2)
- **"Is Vibe Coding the Future?"** — Balanced developer perspective. [joeattardi.dev](https://joeattardi.dev/is-vibe-coding-the-future)
- **"Vibe Reading: Is Research Writing Ready for the LLM Era?"** — [CSPaper Forum](https://forum.cspaper.org/topic/101/from-pdf-is-dead-to-ai-vibe-reading-is-research-writing-ready-for-the-llm-era)

---

*Last updated: February 2026*
