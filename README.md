# Retrieval-Centric Multimodal Question Answering Benchmark

Sample benchmark accompanying the paper:

**See It, Search It: Evaluating Retrieval Decision-Making in Web-Enabled Multimodal LLMs**

## Overview

This repository contains sample data from a benchmark designed to evaluate how modern multimodal large language models (MLLMs) combine **visual understanding** with **integrated web retrieval**.

Unlike traditional visual question answering benchmarks, this benchmark distinguishes between:

* **Static questions**, where answers are available from visual understanding and existing model knowledge.
* **Dynamic questions**, where answering correctly requires identifying visual content and retrieving up-to-date information from the web.

The benchmark is intended for evaluating retrieval-aware multimodal reasoning, including retrieval triggering, query generation, retrieval effectiveness, and failure analysis.

---

## Repository Structure

```
dataset/
├── visual_static_dataset/
│   └── sample images and annotations
└── visual_dynamic_dataset/
    └── sample images and annotations
```

### Static Split

The static split contains examples whose answers are expected to be obtainable without external retrieval. It is designed to evaluate:

* visual understanding
* factual visual question answering
* retrieval calibration
* unnecessary web search behaviour

### Dynamic Split

The dynamic split contains examples requiring retrieval of information beyond the model's knowledge cutoff. These examples evaluate:

* retrieval triggering
* visually grounded search query generation
* retrieval-assisted multimodal reasoning
* integration of retrieved evidence

---

## Usage

Each sample consists of:

* an image
* a natural language question
* a reference answer

The benchmark is model-agnostic and can be evaluated using any multimodal system supporting image understanding, with or without integrated web search.

---

## Full Benchmark

This repository currently contains representative sample data.

The complete benchmark, evaluation scripts, and annotations will be released upon acceptance of the accompanying paper.
