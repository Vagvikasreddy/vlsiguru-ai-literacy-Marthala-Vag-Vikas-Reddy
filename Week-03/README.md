# Week 03 - Practical AI Tools and Engineering Learning

## AI tools explored

I explored ChatGPT, Gemini, Claude and Perplexity as learning assistants. I used them for beginner-friendly explanations, prompt refinement, code walkthroughs, quizzes, comparison of answers and finding technical sources. I treated every answer as a suggestion and verified important claims using official documentation.

## Prompt improvement

Initial prompt: Explain neural networks.

Improved prompt: Explain a feed-forward neural network to a beginner using a semiconductor defect-inspection example. Define inputs, weights, bias, activation, output and loss. Use a numbered explanation, one limitation and two self-check questions.

Adding context, the audience, constraints and an output format made the response clearer and more useful.

## Verified claim

Claim: Test data should not be repeatedly used to guide training decisions because that can make performance look better than it really is.

Source: [Google Machine Learning Crash Course - Overfitting](https://developers.google.com/machine-learning/crash-course/overfitting)

Conclusion: Validation data helps guide development, while a held-out test set gives a more independent final estimate.

## Open-source VLSI tool: Verilator

Verilator is an open-source Verilog/SystemVerilog simulator and lint tool. It translates synthesizable HDL into a cycle-accurate executable model. Its inputs include HDL files, include paths, defines and a top module. Its outputs include lint diagnostics, a simulation model, executable simulation and optional waveform traces.

Basic workflow: write RTL → lint → select the top module → build → run the testbench → inspect logs or waveforms → fix RTL. AI could help explain lint messages, group recurring failures and summarize regressions, but an engineer must review all suggestions.

Source: [Verilator Documentation](https://verilator.org/guide/latest/)

## Reflection

- ChatGPT was most useful for interactive explanations and debugging questions.
- Adding an engineering scenario and requested format improved prompts the most.
- I learned that Verilator supports fast open-source RTL simulation and linting, but testbench setup and compatibility still matter.
- Questions for the ML masterclass: How should model confidence be calibrated? How can data leakage be detected in engineering datasets?

## Responsible use

I did not upload confidential RTL, netlists, timing constraints or proprietary EDA material. I reviewed AI-generated suggestions and took responsibility for the final technical decisions.
