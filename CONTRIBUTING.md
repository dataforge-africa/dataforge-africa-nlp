# Contributing to DataForge Africa NLP

Thank you for your interest in contributing to **DataForge Africa NLP**.

This project is not just a codebase — it is **language infrastructure**.  
Every contribution is expected to uphold the principles defined in the  
[DataForge Africa NLP Manifesto](./MANIFESTO.md).

If you have not read the manifesto, please do so before contributing.

---

## Our Core Philosophy

All contributions **must** align with the following non-negotiable principles:

- African languages are first-class citizens
- Algorithm-first before AI-first
- Determinism before probabilistic behavior
- Education, trust, and explainability over novelty
- Open, reusable, and sovereign design

Contributions that violate these principles will not be accepted, even if they are technically correct.

---

## What We Welcome

We actively welcome contributions that:

### 1. Improve Language Foundations
- Text normalization (diacritics, variants, spelling tolerance)
- Tokenization strategies suitable for African languages
- Rule-based intent detection
- Synonym and variant mapping tables

### 2. Extend Language Coverage
- Support for additional African languages
- Language-specific normalization functions
- Clear linguistic documentation per language

### 3. Improve Explainability & Evaluation
- Deterministic evaluation tools
- Error analysis notebooks
- Coverage and failure mode documentation

### 4. Improve Education & Accessibility
- Clear docstrings and inline comments
- Teaching-friendly examples
- Notebooks or scripts suitable for learners

---

## What We Do NOT Accept

The following will **not** be accepted:

- Black-box models without explainability
- LLM-first features without algorithmic grounding
- Over-engineered abstractions
- Hard dependencies on paid or proprietary APIs
- Language-agnostic shortcuts that erase linguistic nuance
- Contributions that assume perfect spelling or keyboards

If a feature cannot be explained to a student, it does not belong here.

---

## Contribution Workflow

### 1. Start With an Issue

Before submitting code:
- Open an issue describing the problem or improvement
- Explain **why** it aligns with the manifesto
- Describe expected behavior and edge cases

This avoids wasted effort and ensures alignment.

---

### 2. Keep Changes Small and Focused

Each pull request should:
- Address a single concern
- Be easy to review
- Include examples or tests
- Avoid refactoring unrelated code

Infrastructure grows best in small, stable increments.

---

### 3. Coding Standards

All code must:

- Be deterministic where possible
- Use clear, descriptive names
- Include type hints
- Include docstrings explaining **why**, not just **what**
- Avoid unnecessary dependencies

Example:

```python
def normalize_sepedi(text: str) -> str:
    """
    Normalize Sepedi text to handle common keyboard and spelling variations.

    Design intent:
    - User-first, not keyboard-first
    - Deterministic behavior
    - Inclusive of informal typing
    """
