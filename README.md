Iterative Prompting for LAby 5–12 Maze Scoring

This repository accompanies the paper:  
  "Meta Prompting for Clinical AI: Iterative Refinement of GPT-5 in Psychomotor Assessment"    
by Sarah Ayad & Pamela Khattar.

 Overview

We automate scoring of the LAby 5–12 psychomotor test using:
-   MobileNetV2   for Line Crossing (LC)
-   Meta-prompted GPT-5   (especially V5) for Deviation Measure (MD)

Segmentation is performed using the   Segment Anything Model (SAM)  .

 Prompt Versions
We implement an iterative prompting strategy (V1 to V5):
- V1: Minimal Rubric
- V2: Adds Localized Justifications
- V3: Adds Exclusion Rules
- V4: Zero-Error Control
- V5: Few-Shot Anchoring (best performance:   86% MD accuracy  )

 Contents
- `prompts/` — All GPT-5 prompt templates
- `data/` — Sample input images and expert annotations
- `notebooks/` — Training and inference notebooks
- `scripts/` — SAM segmentation, GPT-5 API calls, and evaluation tools
- `results/` — Outputs, plots, and final scores

