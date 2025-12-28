# Deep Reinforcement Learning for De Novo TNKS2 Inhibitor Design

This repository presents an AI-driven pipeline for **de novo drug discovery**, focused on identifying novel **TNKS2 inhibitors** using **deep generative models**, **transfer learning**, and **reinforcement learning**.

## Overview
The project implements and benchmarks multiple molecular generative paradigms under a unified framework:
- SMILES-based LSTM
- Transformer-based autoregressive models
- SELFIES-based GPT (MolGPT)
- Graph-based Variational Autoencoders (GraphVAE)

Models are pretrained on large chemical datasets and fine-tuned toward TNKS2-specific chemical space using **transfer learning** and **reinforcement learning (PPO)**.

## Key Features
- Modular end-to-end pipeline: data curation → training → sampling → evaluation
- Multi-representation molecular generation (SMILES, SELFIES, graphs)
- Transfer learning for low-data target specialization
- Reinforcement learning with multi-objective rewards:
  - Drug-likeness (QED)
  - Synthetic accessibility
  - TNKS2 similarity
- Benchmarking across validity, novelty, diversity, and scaffold diversity
- ADMET and drug-likeness validation using SwissADME

## Methodology
1. Pretraining generative models on large chemical datasets  
2. Fine-tuning models toward drug-like chemical space  
3. Reinforcement learning optimization using PPO  
4. Post-generation evaluation and filtering  

## Results
- SELFIES-based models achieve high validity and novelty
- Transformer models balance exploration and chemical correctness
- GraphVAE enables scaffold-level innovation
- Reinforcement learning significantly improves drug-likeness and feasibility

## Tech Stack
- Python
- PyTorch
- RDKit
- SELFIES
- PPO (Reinforcement Learning)
- SwissADME (external validation)

## Use Cases
- AI-driven drug discovery research
- Generative chemistry benchmarking
- Reinforcement learning for molecular optimization

## Disclaimer
This project is for research and educational purposes only. Generated molecules are computational predictions and require experimental validation.
