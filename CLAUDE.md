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







