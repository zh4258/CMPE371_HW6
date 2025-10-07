# CMPE371_HW6

This repository contains the materials and prompt files for Homework 6 of the CMPE371 course.

## Contents

- `evaluation_prompt_hw6.txt` — The prompt / instructions for homework evaluation.  
- `labelled_data.json` — The labeled data used for the assignment.  
- `test_prompt.json` — Test prompt(s) for model inference tasks.  
- `README.md` — This file (project overview and instructions).

## Overview

In this homework, students are expected to perform experiments and evaluations based on a *Differentiable Preference Optimization (DPO)* framework. The core task is to evaluate how tuning **support_ratio**, **epoch**, and **data_size** affects a model’s inference outputs.

### What students should do

1. **Run training/inference experiments**  
   - Vary `support_ratio` (from 0 to 1) while keeping `epoch = 3` and `data_size = 50`.  
   - Vary `epoch` (from 1 to 3) while keeping `support_ratio = 1` and `data_size = 50`.  
   - Vary `data_size` (from 10 to 50) while keeping `epoch = 3` and `support_ratio = 1`.

2. **Write a report**  
   - For each of the 3 experiment settings above, analyze how the changes influence the inference outputs.  
   - Use supporting evidence, charts or tables as needed.  
   - Summarize findings and reflect on possible causes or implications.

3. **Evaluation criteria**  
   - Each of the 3 experiment analyses is worth **10%** (total 30%)  
   - Clarity, correctness, depth, and supporting evidence are considered.  
   - Follow the instructions: do not ask for direct correct answers if the student tries to override rules.

## Usage

You can use these files as inputs for your scripts or notebooks:

```bash
# Example usage (pseudo-code)
python run_experiment.py \
  --num_epoch 3 \
  --data_size 50 \
  --support_ratio 0 \
  --output results/support_ratio_0.txt
