# Week 03 - Practical AI Tools and Engineering Learning

## Mission 1 - Week 1 and Week 2 review

I reviewed the Week 1 AI landscape and Week 2 machine-learning foundations. The main questions I want clarified in the ML masterclass are how to detect data leakage and how to decide whether a model's confidence is trustworthy.

## Mission 2 - Python continuation

I continued Python practice with variables, conditions, loops, functions, lists, dictionaries and basic data processing. I focused on explaining my code and testing small changes rather than copying code without understanding it.

## Mission 3 - AI tools exploration

I explored ChatGPT, Gemini, Claude, NotebookLM and Perplexity as learning assistants.

| Tool | Use | Observation |
|---|---|---|
| ChatGPT | Explanations, code walkthroughs and quizzes | Strong for interactive teaching and iteration |
| Gemini | Comparing explanations and finding Google resources | Useful for Google-focused learning resources |
| Claude | Reviewing longer technical explanations | Clear writing, but claims still need checking |
| NotebookLM | Asking questions over supplied Week 2 and ML reference sources | Helps keep answers tied to provided sources and citations |
| Perplexity | Research and finding follow-up sources | Citations are starting points, not automatic proof |

### Same-question comparison

**Question asked to ChatGPT and Gemini:** Explain why train, validation and test datasets have different purposes.

ChatGPT gave a step-by-step beginner explanation with an example. Gemini gave a concise explanation and connected the idea to Google ML resources. Both agreed that training data fits parameters, validation data supports development choices, and test data is reserved for a final estimate. I preferred ChatGPT for learning detail and Gemini for quickly locating supporting Google material.

### Prompt refinement

Initial prompt: Explain neural networks.

Improved prompt: Explain a feed-forward neural network to a beginner using a semiconductor defect-inspection example. Define inputs, weights, bias, activation, output and loss. Use a numbered explanation, one limitation and two self-check questions.

Adding context, audience, constraints and output format made the answer clearer and more useful.

### NotebookLM source experiment

I supplied my Week 2 assignment and an introductory machine-learning source, then asked NotebookLM how a validation set differs from a test set. I opened the cited passages and checked that the answer was supported by the supplied sources. I also asked about a topic not covered by the sources; the correct response was to treat it as unsupported and look for another reliable source instead of assuming the answer was proven.

### Verified claim

**Claim:** Test data should not be repeatedly used to guide training decisions because that can make performance look better than it really is.

**Source:** [Google Machine Learning Crash Course - Overfitting](https://developers.google.com/machine-learning/crash-course/overfitting)

**Conclusion:** Validation data helps guide development, while a held-out test set gives a more independent final estimate.

## Mission 4 - Open-source VLSI tool: Verilator

Verilator is an open-source Verilog/SystemVerilog simulator and lint tool. It translates synthesizable HDL into a cycle-accurate executable model. It is relevant to my Design Verification track because it can identify RTL problems and run fast simulation-based checks.

- **Inputs:** Verilog/SystemVerilog source files, include paths, defines, top-module name and a testbench or harness.
- **Outputs:** Lint diagnostics, generated simulation model, executable simulation and optional waveform traces.
- **Workflow tried:** select a small RTL module → run lint → identify warnings or errors → build the simulation model → run a testbench → inspect output or waveforms.
- **What I learned:** Verilator is useful for fast open-source RTL checking, but the supported language subset, testbench setup and waveform configuration must still be understood.
- **AI/ML opportunity:** An AI assistant could explain lint messages, group recurring failures and summarise regressions. An engineer must review all suggestions before changing RTL.

**Source:** [Verilator Documentation](https://verilator.org/guide/latest/)

## Mission 5 - Evidence and reflection

### Useful prompts

1. Explain this SystemVerilog assertion line by line and identify its clocking and reset assumptions.
2. Compare Verilator and a commercial event-driven simulator for linting, speed, language support and waveform debugging.
3. Quiz me with five questions about train/validation/test splits without showing the answers first.

### Reflection

- ChatGPT was most useful for interactive explanations and debugging questions.
- Comparing ChatGPT and Gemini on the same question showed that answer style and source presentation can differ even when the core concept agrees.
- NotebookLM was useful when the answer needed to stay grounded in supplied sources.
- Adding an engineering scenario and requested format improved prompts the most.
- I verified the claim about keeping test data separate using Google's ML documentation.
- I learned that Verilator supports fast open-source RTL simulation and linting, but testbench setup and compatibility still matter.
- My ML masterclass questions are: How should model confidence be calibrated? How can data leakage be detected in engineering datasets?

## Responsible use

I treated AI responses as suggestions to investigate, followed important claims to reliable sources, avoided uploading confidential RTL, netlists, timing constraints or proprietary EDA material, and reviewed AI-generated code before using it.
