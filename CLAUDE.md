# CLAUDE.md

## Project
Course repository for COSC 650: Applied LLM Systems (Maryville University).
8-week graduate course covering tokenization, transformer architecture,
prompt engineering, function calling, retrieval-augmented generation,
fine-tuning, and evaluation.

## Structure
- week-01/ through week-08/ : weekly assignments and notebooks
- notes/: research notes and reading annotations
- project/: final project code and documentation
- CLAUDE.md: this file
- README.md: human-facing project description

## Conventions

- All code is Python 3.11+
- Commits use descriptive messages, not "update" or "fix"

## Do Not
- Delete files or directories without confirming first
- Push to main without checking what is staged
- Commit API keys or any file in .env
- 
## Week-1 Assignment

- OpenAI is used to test Amharic/English supplied passages
- Notebooks are saved from Google Colab via Save in GitHub
- tiktoken is used for the tokenization experiment

- ## Week-2 Assignment

- ## Purpose of the assignment

•	Creating a forward pass that turns a given prompt into a probability distribution.

•	Building a sampling step that turns that distribution into a choice. 

•	To see the effect of temperature, top-k, and top-p on the token distribution of a model.

## Technologies used:

•	DistilGPT2

•	OpenAI

•	Jupyter/Python on Google Colab

# Week-3: Prompt Engineering Artifact Project

This week's notebook evaluates two versioned security-triage prompts across 12 test cases, using exact-match severity accuracy and semantic similarity for rationales.

# Technologies Used
Google Colab environment

OPENAI/GPT-4o

GEMINE/API

# Week-4 Multi_Tool Assistant

The Multi -Tool Assistant  notebook uses Gemini Flash through Google's OpenAI-compatible endpoint. It defines three constrained tools, implements a complete request-and-response loop, provides a guarded arithmetic evaluator, records every tool call, evaluates the tools, and demonstrates structured recovery from a real invalid-date failure.

# Technologies used:

Gemini Flash 3.8.

OpenAI/gpg-4o

Google collab

# Week-5
- RAG Pipeline with Retrieval Evaluation

- This week's notebook builds a complete pipeline and compares retrieval choices with real precision and recall.

- Used Python
  
- Sentence Transformers
  
- FAISS
  
- pandas
  
- Gemini-flash 3.8

# Week 7: Healthcare Administrative Intent Classification

## Objective
Classify healthcare administrative requests into exactly one of five labels: billing_question, find_clinic, get_lab_results', refill_medication, or schedule_appointment. 

## Dataset and reproducibility
Synthetic, template-generated text with random seed 7; no real patient records. The source notebook generates 907 raw records, removes 7 invalid and 593 duplicate records, leaving 307 unique valid records. Stratified balanced splits contain 200 training examples (40 per intent) and 50 evaluation examples (10 per intent); 57 cleaned records are unused in the split. Files: clean_dataset.csv, train.csv, evaluation.csv. 

## Retrieval and evaluation
Embed training text with sentence-transformers/all-MiniLM-L6-v2, L2-normalize, and search a FAISS `IndexFlatIP` index for the top 4 examples. Normalized inner product equals cosine similarity. Compare zero-shot against dynamically retrieved few-shot prompts on the same held-out 50 examples using Gemini, temperature 0. 

## Technologies used

Google colab

Gemini with API

Sentence transformers/all-miniLM-L6-V2

Oepnai

 # Week 8: Healthcare Administrative Assistant
- Purpose
  
This week's assignment contains a Jupyter capstone prototype for healthcare administrative assistance. It classifies requests, retrieves relevant administrative policy, optionally logs a simulated workflow route, and produces a policy-grounded response. The primary notebook is Week_8_capstone.ipynb.

# Architecture
User request → semantic few-shot intent classification → intent-conditioned query expansion → FAISS policy retrieval → optional constrained workflow routing → grounded prompt → optional Gemini response → logging/evaluation.

# Technologies used
- Python 3 and Jupyter Notebook: 
- NumPy and pandas: 
- Sentence Transformers (all-MiniLM-L6-v2): 
- FAISS (faiss-cpu==1.12.0, IndexFlatIP): 
- scikit-learn: 
- OpenAI Python SDK with a Google Gemini-compatible endpoint: 
- Python standard library (os, re, json, ast, operator, pathlib, hashlib, unittest. mock, etc.): 
- GEMINI_API_KEY: 



