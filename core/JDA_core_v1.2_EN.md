# JDA Core v1.2

## Judgement-Driven Architecture

---

## 1. Introduction

In recent years, the rapid advancement of AI has begun to transform decision-making within enterprises.  
However, many AI initiatives face the following issues:

- Uncertainty about where AI should be applied  
- Proliferation of PoCs that never reach production  
- Lack of clarity in ROI, making investment decisions difficult  
- AI adoption becoming an end in itself  

The root cause of these problems lies in the unit of AI implementation.

Most AI initiatives are designed around tasks or processes.

Task → Automation

However, enterprise activity fundamentally follows this structure:

Information → Judgement → Action → Result

While actions determine outcomes,  
those actions are determined by judgements.

Therefore, the fundamental unit of enterprise activity is not “tasks” but “judgements.”

Furthermore, in the AI era, AI models themselves are becoming commoditized.  
Competitive advantage will be determined not by:

- Which AI is used  
but by  
- What is learned by AI  

This leads to a critical problem:

Enterprises do not have a clear definition of what should be learned.

While the importance of proprietary data is widely recognized,  
there is no systematic framework for:

- What data should be collected  
- How it should be structured  
- How it should be used for learning  

This work proposes the following hypothesis:

Proprietary data in the AI era is “judgement data.”

Judgement-Driven Architecture (JDA) is an architecture that extracts, structures, and logs enterprise judgements,  
enabling both humans and AI to learn from them.

---

## 2. Core Hypotheses

JDA is based on the following hypotheses.

### Hypothesis 1: Enterprises operate on judgement, not data

Enterprise activity can be described by data,  
but what actually changes the state of the enterprise is judgement.

Data is the input for judgement,  
but judgement is the unit of control.

---

### Hypothesis 2: Enterprise outcomes are determined by judgement quality

Actions are selected based on judgement.

Therefore, enterprise outcomes depend not on actions themselves,  
but on the quality of the judgements behind them.

---

### Hypothesis 3: Organizational culture is an accumulation of judgements

Culture is not defined by rules,  
but by patterns of repeated decision-making.

The way judgements are made shapes organizational behavior.

---

### Hypothesis 4: Judgement logs enable learning for both organizations and AI

Traditional enterprise systems record:

- Data (what happened)  
- Actions (what was done)  

But they do not record:

- Why a decision was made  
- What alternatives existed  

As a result:

Actions can be reproduced, but decisions cannot be learned.

By logging judgements:

- Organizations can reflect and learn from decisions  
- AI can learn decision-making itself  

---

## 3. Definition of Judgement

Judgement is:

The act of selecting and fixing one state from multiple possible futures.

### Characteristics

- Determines state transitions  
- Constrains actions  
- Has an accountable owner  

---

### Judgement Dimensions

- Proceed  
- Validity  
- Accountability  
- Venture  

Venture represents the degree of exploration, not a type of judgement.

---

## 4. Architecture

Discovery → Investment → Learning

- Discovery: Discovering judgement structures  
- Investment: Evaluating judgement investment  
- Learning: Design, logging, and learning  

---

## 5. Judgement Structure

Enterprise activity is organized using the following concepts.

---

### Business Journey（BJ）

A unit of business activity.  
Used in Phase0 Foundation.

Examples:
- BJ01 New Client Acquisition  
- BJ07 Payment Confirmation & Reconciliation  

---

### Judgement Journey（JJ）

A chain of judgements toward a specific purpose.  
Used from Phase1 Discovery onward.  
A reinterpretation of BJ from a judgement perspective.

Example:  
JJ01 Lead Qualification Chain:  
"Should we target this company?"  
→ "Should we make contact now?"  
→ "Is this a qualified lead?"  
→ "Should we add them to the list?"

---

### Judgement Point（JP）

The smallest unit of judgement.

Expressed in the form: "Should we...?"

Judgements occur at the intersection of:  
Customer State × Enterprise Action

Examples:
- Should we approach this company?  
- Is this a qualified lead?  
- Which invoice does this payment correspond to?  

---

### Judgement Chain

A chain of enterprise-wide judgements that emerges  
from the sequence of Business Journeys.

It is not explicitly designed,  
but becomes visible once BJ and JJ are defined.

```text
BJ01 → BJ02 → BJ03 → ...
↓
Judgement Chain (emerges as a result)
```

---

### Relationship

```text
BJ (Business unit) ← Foundation
↓ Reinterpreted from a judgement perspective
JJ (Judgement unit) ← Discovery onward
└ JP (Atomic judgement)

BJ01 → BJ02 → BJ03 → ...
↓
Judgement Chain (emerges as a result)
```

Enterprise activity should be understood not as processes,  
but as a structure of judgements.

---

## 6. Investment Theory

### Judgement ROI

ROI = Frequency × Impact × Improvement Rate − Cost

---

### JULIA

JULIA is a framework for evaluating judgement investment.

It extends traditional ROI-based evaluation  
by incorporating multiple perspectives.

This structure is inspired by the Balanced Scorecard (BSC).

---

### JULIA Dimensions

- ROI  
- Business Impact  
- Automation Potential  
- Learning Value  

---

## 7. Learning System

### JSC

Judgement State Chart  

### JDC

Judgement Design Canvas  

### JLog

Judgement Log  

### VLog

Validity Log  

---

### Lifecycle

Before → During → After

---

### Learning Loop

Data → AI → Options → Human → JLog → Action → Result → VLog → Learning

---

## 8. AI Implementation

### 8.1 Problem of AI Adoption

Failures in AI adoption stem from incorrect units.

Task → Automation (incorrect)  
Judgement → Improvement (correct)  

AI can reproduce actions, but cannot learn decisions.

---

### 8.2 Role of JDA

JDA resolves this through:

Judgement Extraction → JULIA → Design → Logging → Learning

---

### 8.3 AI Agent Roles

JDA defines two types of AI agents.

---

#### Process AI Agent

Role:
- Automates workflows  
- Executes tasks  
- Advances processes based on decisions  

---

#### Judgement AI Agent

Role:
- Collects and structures decision inputs  
- Generates options  
- References past judgement logs  
- Supports decision-making  

---

### 8.4 Relationship

```text
Process AI Agent (What to do)
↓
Judgement AI Agent (How to decide)
↓
Human Judgement
↓
JLog
↓
Learning
```

---

### 8.5 Enterprise World Model

Continuous operation of this loop leads to the formation of an Enterprise World Model.

---

## 9. Positioning

- BI: Data  
- BPM: Process  
- DDD: Model  
- KM: Knowledge  

JDA treats decision-making as a first-class concern.

---

## 10. Venture Judgement

All judgements exist on a spectrum of exploration.

---

## 11. Long-term Vision

Construction of the Enterprise World Model

---

## Final Definition

JDA:

Extracts judgement  
Evaluates judgement  
Logs judgement  
Learns from judgement  

To evolve enterprise decision-making capability.

---

## License & Citation

Copyright (c) 2026 Shun Takeda (B-AS)
CC BY 4.0 — <https://creativecommons.org/licenses/by/4.0/>

Citation:
Takeda, Shun. Judgement-Driven Architecture. B-AS, 2026.
<https://github.com/judgement-driven/Judgement-Driven-Architecture>
