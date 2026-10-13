# CrewAI Build Report

## 1. Overview

This project uses CrewAI to build a sequential multi-agent workflow that explains a technical topic in plain language. The workflow contains three agents: Research Analyst, Technical Writer, and Editor.

## 2. Original Implementation

The original program uses three agents in sequence:

1. **Research Analyst:** Collects five key facts and two open questions about the topic.
2. **Technical Writer:** Uses the research brief to write an approximately 250-word explainer.
3. **Editor:** Improves clarity and flags claims that need sources.

The original topic was: "how small teams can use AI agents in data science."

The original terminal output is saved in `run1_original.txt`, and the original explainer is saved in `explainer_run1.md`.

## 3. Code Change

I modified the writing task in `main.py`. The revised instructions require the explainer to include a concrete example of a small data science team using AI agents and a practical, numbered three-step implementation checklist. The instructions also ask the writer to avoid unsupported statistics and clearly mark claims that need verification.

This change makes the expected output more practical and gives the reader actionable steps.

## 4. Changed Implementation

I ran the modified program using the same topic as the original run. This keeps the topic consistent for comparison.

The changed terminal output is saved in `run2_changed.txt`, and the changed explainer is saved in `explainer_run2.md`.

## 5. Comparison

The original version focuses on producing a plain-language explainer based on the research brief. The changed version adds specific requirements for a real-world example and a three-step checklist.

These additional requirements provide a clearer structure and make the explainer more action-oriented. The generated content may vary between runs, so the saved outputs should be used to evaluate whether the new requirements were actually met.

## 6. Limitations

AI-generated facts and statistics may be inaccurate or require verification. Claims flagged by the editor should be checked against reliable sources before being used in academic or professional work.

## 7. Conclusion

This exercise demonstrates how changing a task description can guide a multi-agent workflow toward a more structured and practical result while retaining the original three-agent sequence.