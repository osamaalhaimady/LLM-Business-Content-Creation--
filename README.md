# Enhancing Central Bank Communications with AI

## Project Overview

This project explores the use of a lightweight Large Language Model (LLM) to simplify complex financial and regulatory communications from the Bank of Russia.

The goal is to improve text clarity, transparency, and readability while preserving the original meaning and essential numerical information.

## Model

- Model: Vikhr-Llama-3.2-1B-instruct
- Domain: Financial and regulatory communication
- Language: Russian
- Main technique: Unsupervised Style Transfer
- Training approach: Style-tuning followed by prompt-based inference

## Methodology

The project initially considered Supervised Fine-Tuning (SFT), which requires paired examples of complex and simplified texts.

Because the available datasets were unpaired and computational resources were limited, the team adopted an Unsupervised Style Transfer approach.

The workflow consisted of:

1. Preparing separate collections of complex and simple financial texts.
2. Fine-tuning the model on simple financial texts to learn their writing style.
3. Using instruction prompts to guide the model in simplifying complex texts.
4. Evaluating the generated outputs using transparency and readability metrics.
5. Reviewing the outputs for preservation of important information.

## Evaluation

The project used two evaluation metrics:

- **AlinaEstimator:** Evaluates transparency in financial communication.
- **ARIEstimator:** Evaluates text readability.

The project report describes an example in which the transparency score increased from 3 to 6, while the readability score decreased from 6.4 to 6.1.

These results relate to the reported evaluation example and should not be interpreted as a universal performance guarantee.

## My Contribution

According to the project presentation, my contributions included:

- Fine-tuning the Vikhr-Llama-3.2-1B-instruct model using Unsupervised Style Transfer.
- Implementing style-tuning and prompt-based inference.
- Helping resolve data integrity issues during model training.

## Team

This was a collaborative project involving students from:

- Harbin Institute of Technology
- Yangzhou University
- Hohai University

## Project Materials

- [Research Paper](Research_Paper.pdf)
- [Project Presentation](Project_Presentation.pptx)
- [Presentation Script](Presentation_Script.docx)

## Limitations

The project focused on Russian financial texts and a specific communication domain.

The current approach may require additional training and evaluation before being applied to other languages or domains.

Further work could include larger evaluation studies, human feedback, and additional safeguards to verify factual accuracy.

## Acknowledgment

This project was developed as part of the SMILE(s) Summer School 2025 project activities.

The work was completed collaboratively by the project team.
