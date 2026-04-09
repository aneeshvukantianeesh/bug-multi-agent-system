# bug-multi-agent-system
# Multi-Agent Bug Debugging System

## Overview

This project implements a multi-agent system that analyzes a bug report and logs, reproduces the issue, and proposes a root cause and fix plan.

---

## Features

* Multi-agent orchestration (Triage, Log Analysis, Hypothesis, Reproduction, Fix, Critic)
* Automated bug reproduction using pytest
* Structured JSON output
* Evidence-based debugging
* Minimal reproducible test case

---

## Project Structure

```
bug-multi-agent-system/
├── notebook.ipynb
├── inputs/
├── sample_repo/
├── outputs/
```

---

## Setup Instructions

1. Install dependencies:

```
pip install pytest
```

2. Run the notebook:

* Open `notebook.ipynb`
* Run all cells

---

## How It Works

1. Parses bug report and logs
2. Identifies failure patterns
3. Generates hypotheses
4. Reproduces bug using pytest
5. Proposes root cause and fix
6. Outputs structured JSON

---

## Reproduction

Run:

```
pytest sample_repo
```

Expected:

* Test fails due to `ZeroDivisionError`

---

## Output

Generated file:

```
outputs/result.json
```

Contains:

* Bug summary
* Evidence
* Reproduction steps
* Root cause
* Patch plan
* Validation plan

---

## Traceability

Console logs show:

* Agent execution steps
* Tool usage (pytest execution)

---

## Notes

* No external APIs used
* Fully reproducible system
* Designed with modular multi-agent architecture
