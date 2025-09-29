# Sentinel Scanner — Payload Mutator & Adaptive Payload Engine

Sentinel Scanner is a next-gen open-source vulnerability scanner that uses adaptive, AI-driven payload mutation to discover vulnerabilities more reliably and reduce false positives.

This repository contains the Payload Mutation Engine (Phase 1 prototype), including:
- deterministic + randomized mutation rules (encodings, junk injection, casing, wrappers)
- a small SQLite store for learning successful payloads
- an LLM integration hook (stub) for AI-driven suggestions
- example CLI/demo

## Quickstart

```bash
# clone
git clone https://github.com/<your-username>/sentinel-scanner.git
cd sentinel-scanner

# create venv
python -m venv .venv
source .venv/bin/activate

# install deps
pip install -r requirements.txt

# run demo
python examples/demo.py
