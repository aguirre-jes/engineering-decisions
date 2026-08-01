# Engineering Decisions Methodology

Engineering Decisions is more than a collection of cloud-native laboratories.

It is a repeatable methodology for exploring engineering questions through reproducible implementation, controlled experimentation, and evidence-based reasoning.

This document defines the principles followed by every Engineering Decision published in this repository.

---

# Core Philosophy

Engineering Decisions are not intended to prove that one technology is universally better than another.

Instead, they aim to answer practical engineering questions by combining:

- Official documentation
- Hands-on implementation
- Controlled experiments
- Observable evidence
- Engineering reasoning

The objective is not certainty.

The objective is confidence supported by evidence.

---

# Laboratory Design Principles

Every Engineering Decision should follow these principles.

## 1. Start with a Question

Every laboratory begins with a real engineering question.

Examples:

- What engineering responsibilities remain after node management disappears?
- When should Amazon ECS be preferred over Amazon EKS Auto Mode?
- Why do Kubernetes resource requests still matter?

If there is no engineering question, there is no Engineering Decision.

---

## 2. Define a Hypothesis

Every laboratory should propose an initial hypothesis before implementation begins.

The hypothesis should be validated—or disproved—through experimentation rather than assumptions.

---

## 3. Build a Reproducible Environment

Every laboratory must be reproducible from scratch.

Infrastructure should be provisioned using Infrastructure as Code whenever possible.

Manual configuration should be avoided unless it is part of the experiment itself.

---

## 4. Change One Variable at a Time

Each experiment should introduce a single engineering decision while keeping all other variables unchanged.

This makes observations easier to understand and conclusions easier to defend.

---

## 5. Collect Observable Evidence

Engineering conclusions should always be supported by evidence.

Examples include:

- Kubernetes Events
- Pod Status
- Metrics
- Logs
- Deployment behavior
- Resource utilization

Evidence should always be reproducible.

---

## 6. Explain the Trade-offs

Every engineering decision introduces advantages and disadvantages.

Laboratories should document both.

The goal is not to recommend a universal solution but to explain the consequences of each decision.

---

## 7. Keep Production in Mind

Every experiment should reflect production-oriented engineering practices whenever possible.

This includes topics such as:

- Reliability
- Scalability
- Security
- Cost
- Operability
- Maintainability

---

## 8. Consider Cost as a Design Constraint

Laboratories should be intentionally designed to minimize unnecessary cloud costs while remaining fully reproducible.

Cost should never become a barrier to learning.

---

# The Engineering Decision Lifecycle

Every Engineering Decision follows the same workflow.

```text
Engineering Question
        ↓
Hypothesis
        ↓
Implementation
        ↓
Experiment
        ↓
Evidence
        ↓
Observations
        ↓
Trade-offs
        ↓
Engineering Decision
```

---

# Definition of Done

An Engineering Decision is considered complete when:

- The laboratory can be reproduced from scratch.
- Infrastructure is provisioned using Infrastructure as Code.
- Every experiment has documented evidence.
- Trade-offs are clearly explained.
- Conclusions are supported by observable behavior.
- The accompanying technical article has been published.

Until then, the laboratory remains a work in progress.

---

# Continuous Improvement

Engineering Decisions are living documents.

As cloud platforms evolve, laboratories may be updated to reflect new capabilities, revised best practices, or improved engineering understanding while preserving the reasoning behind previous decisions.