---
title: "Flip It!! — Simulation Tool (Coin & Dice)"
one_liner: "Designed a small but disciplined simulation tool emphasizing predictable control flow, validation-first design, and testability."
featured: true
order: 2
repo_url: "https://github.com/ReginaOfTech/CoinFlipProgram"
tags: ["Python", "Testing", "State Machines"]
highlights:
  - "Implemented object-oriented abstractions to support fair and weighted coins and dice without modifying core logic."
  - "Used explicit state transitions to keep user interaction predictable and easy to test."
  - "Backed core behavior with PyTest-based unit tests to validate correctness and edge cases"
---

### Tech
Python • Object-Oriented Design • State Machines • PyTest

### Overview
Flip It!! is a command-line simulation tool for coin flips and dice rolls designed to demonstrate clean control flow, extensibility, and testability in a small codebase.

### Context
Even simple interactive programs can become fragile when input handling, branching logic, and validation are interwoven. This project focuses on keeping behavior explicit and predictable, even in a lightweight application.

### Approach
- Modeled coins and dice as interchangeable objects using clear interfaces.
- Structured user interaction as a state-driven workflow to avoid deeply nested conditionals.
- Applied validation-first input handling to prevent invalid states.
- Wrote targeted unit tests to verify both expected behavior and edge cases.

### Why This Matters
This project demonstrates disciplined software design at a small scale—prioritizing clarity, correctness, and maintainability, which directly translates to larger production systems.

### Links
- GitHub: [Regina Baker/CoinFlipProgram](https://github.com/ReginaOfTech/CoinFlipProgram)
