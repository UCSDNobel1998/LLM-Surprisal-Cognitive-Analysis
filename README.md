# LLM Sensitivity to World Knowledge Violations: A Surprisal Analysis

## Overview
This project investigates the alignment between Large Language Model (GPT-2) probability distributions and human cognitive processing. Specifically, we analyze whether **Surprisal metrics** ($-\log_2 p$) in Transformer models correlate with the **N400 ERP (Event-Related Potential)** observed in human neuroscience when processing semantic violations.

## Methodology
- **Model:** GPT-2 (via Hugging Face Transformers)
- **Metric:** Token-level Surprisal calculated from output logits.
- **Stimuli:** 20 "minimal pair" sentences contrasting plausible vs. implausible contexts (e.g., "Winter turns water into *ice*" vs. "*fire*").
- **Analysis:** Statistical comparison of entropy and probability distributions between conditions.

## Key Findings
- The model exhibits significantly higher surprisal for "world knowledge violations" (M ≈ 11.1) compared to plausible completions (M ≈ 4.1).
- These results suggest that Transformer architectures implicitly encode functional maps of physical reality, mirroring human N400 neural signatures.

## Tech Stack
- **Core:** Python 3.9, PyTorch
- **NLP:** Hugging Face Transformers
- **Data/Viz:** Pandas, NumPy, Seaborn, Matplotlib

---
*Project completed for UCSD COGS 150 (Spring 2025).*
