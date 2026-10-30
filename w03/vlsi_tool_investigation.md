# VLSI Tool Investigation

## Tool: Verilator

Verilator is an open-source Verilog/SystemVerilog simulator and lint tool. It is relevant to my Design Verification track because it can identify RTL problems and run fast simulation-based checks.

## Problem it solves

It provides linting and cycle-accurate simulation for RTL without requiring a commercial simulator.

## Inputs

- Verilog/SystemVerilog source files
- Include paths and preprocessor defines
- Top-module name
- Testbench or C++/SystemC harness

## Outputs

- Lint diagnostics and warnings
- Generated simulation model
- Executable simulation
- Optional waveform traces

## Basic workflow explored

Select a small RTL module, run lint, identify warnings or errors, build the simulation model, run a testbench and inspect the output or waveform. The supported language subset, testbench setup and tracing options must be understood before relying on results.

## AI/ML opportunity

An AI assistant could explain lint messages, group recurring failures and summarise regression results. It should not change RTL automatically; an engineer must review and test every suggestion.

## Source

[Verilator Documentation](https://verilator.org/guide/latest/)
