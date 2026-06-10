# Contribution 1: Quantized Training

**Contribution Number:** 1  
**Student:** Kaung Myat Naing  
**Issue:** https://github.com/pytorch/ao/issues/554  
**Status:** Phase I In Progress  

---

## Why I Chose This Issue

I chose this issue because it is directly related to my interests in machine learning systems, efficient AI, and model optimization. Quantized training is important because it can reduce memory usage during training and potentially make larger model training more accessible. Since TorchAO focuses on PyTorch-native optimization workflows, this issue gives me a chance to learn how real-world ML infrastructure supports lower-precision training techniques such as INT8, FP8, and quantization-aware workflows.

This issue also matches my learning goals because I want to go deeper than application-level AI work and understand how model training can be optimized at the framework level. I hope to learn how TorchAO organizes quantized training code, how benchmark or recipe scripts are structured, and how to compare a baseline training path against a quantized training path using metrics like loss, memory usage, and runtime.

---

## Understanding the Issue

### Problem Description

TorchAO currently has strong support for quantization and model optimization, but this issue asks for more practical quantized training recipes or examples. In my own words, what is missing is a clear, runnable starting point that shows how to train a small model using a quantized training approach and compare it against a normal BF16/FP16 baseline.

### Expected Behavior

There should be a small, understandable example or recipe that demonstrates quantized training in TorchAO. Ideally, the example should make it easy to compare a normal training baseline with a quantized training path and report basic results such as loss behavior, memory usage, and runtime. This would help new contributors and users understand how quantized training works in TorchAO.

### Current Behavior

The issue describes quantized training as an important direction, but the full scope is broad. It discusses different possible precision choices for weights, activations, and optimizer states, but there is not yet a simple beginner-friendly recipe attached to the issue that clearly demonstrates one complete small-scale quantized training workflow.

### Affected Components

The main parts of the codebase likely involved are:

- `torchao/prototype/quantized_training`
- Existing quantized training examples or benchmark scripts
- Benchmark or recipe structure used for comparing baseline training against quantized training
- TorchAO tensor or quantization utilities used by the quantized training path

For my first contribution, I plan to start by reading the existing quantized training prototype code and identifying the smallest realistic place to add a runnable example or benchmark.

---

## Reproduction Process

### Environment Setup

[Notes on setting up your local development environment - challenges you faced, how you solved them]

### Steps to Reproduce

1. [Step 1]
2. [Step 2]
3. [Observed result]

### Reproduction Evidence

- **Commit showing reproduction:** [Link to commit in your fork]
- **Screenshots/logs:** [If applicable]
- **My findings:** [What you discovered during reproduction]

---

## Solution Approach

### Analysis

[Your analysis of the root cause - what's causing the issue?]

### Proposed Solution

[High-level description of your fix approach]

### Implementation Plan

Using UMPIRE framework (adapted):

**Understand:** [Restate the problem]

**Match:** [What similar patterns/solutions exist in the codebase?]

**Plan:** [Step-by-step implementation plan]
1. [Modify file X to do Y]
2. [Add function Z]
3. [Update tests]

**Implement:** [Link to your branch/commits as you work]

**Review:** [Self-review checklist - does it follow the project's contribution guidelines?]

**Evaluate:** [How will you verify it works?]

---

## Testing Strategy

### Unit Tests

- [ ] Test case 1: [Description]
- [ ] Test case 2: [Description]
- [ ] Test case 3: [Description]

### Integration Tests

- [ ] Integration scenario 1
- [ ] Integration scenario 2

### Manual Testing

[What you tested manually and results]

---

## Implementation Notes

### Week [X] Progress

[What you built this week, challenges faced, decisions made]

### Week [Y] Progress

[Continue documenting as you work]

### Code Changes

- **Files modified:** [List]
- **Key commits:** [Links to important commits]
- **Approach decisions:** [Why you chose certain approaches]

---

## Pull Request

**PR Link:** [GitHub PR URL when submitted]

**PR Description:** [Draft or final PR description - much of the content above can be adapted]

**Maintainer Feedback:**
- [Date]: [Summary of feedback received]
- [Date]: [How you addressed it]

**Status:** [Awaiting review / Iterating / Approved / Merged]

---

## Learnings & Reflections

### Technical Skills Gained

[What you learned technically]

### Challenges Overcome

[What was hard and how you solved it]

### What I'd Do Differently Next Time

[Reflection on your process]

---

## Resources Used

- [Link to helpful documentation]
- [Tutorial or Stack Overflow post that helped]
- [GitHub issues or discussions that helped]
