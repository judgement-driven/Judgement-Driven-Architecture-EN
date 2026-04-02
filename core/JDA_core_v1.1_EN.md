# JDA Core v1.1

## Judgement-Driven Architecture

---

## 1. Introduction

In recent years, the rapid advancement of AI has begun to fundamentally transform how decisions are made within organizations.  
However, many AI initiatives suffer from the following issues:

- Uncertainty about where AI should be applied  
- Proliferation of PoCs (Proofs of Concept) without production deployment  
- Unclear ROI, making investment decisions difficult  
- AI adoption becoming an end in itself  

The root cause of these problems lies in the unit of application.

Most AI initiatives are designed around business processes:

```text
Process → Automation
```

However, actual enterprise activity follows a different structure:

```text
Information → Judgement → Action → Result
```

While outcomes are produced by actions,  
those actions are determined by judgements.

Therefore, the fundamental unit of enterprise activity is not the process, but the judgement.

---

Furthermore, in the AI era, AI models themselves are becoming commoditized.  
Competitive advantage no longer depends on:

- Which AI is used  

but rather on:

- What is taught to the AI  

---

However, a critical problem remains:

Organizations have not defined what should be learned.

While the importance of proprietary data is widely recognized,  
the following remain unclear:

- What data should be collected  
- How it should be structured  
- How it should be used for learning  

---

This work proposes the following hypothesis:

> Proprietary data in the AI era is judgement data.

Judgement-Driven Architecture (JDA) is an architecture that extracts, structures, logs, and enables learning from organizational judgements for both humans and AI.

---

## 2. Core Hypotheses

JDA is based on the following hypotheses.

---

### Hypothesis 1: Enterprises operate on judgements, not data

Enterprise activities are described by data,  
but what actually changes the state of the enterprise is judgement.

Data is merely input to judgement.  
The control unit of the enterprise is judgement.

---

### Hypothesis 2: Organizational performance is determined by the quality of judgement

Actions are selected through judgement.

Therefore, organizational performance depends not on actions themselves,  
but on the quality of the underlying judgements.

---

### Hypothesis 3: Organizational culture is the accumulation of judgements

Organizational culture is not defined by explicit rules,  
but by the accumulation of daily decision patterns.

Repeated judgements shape behavioral norms.

---

### Hypothesis 4: Judgement logs enable learning for both organizations and AI

Traditional enterprise systems record:

- Data (what happened)  
- Actions (what was done)  

But they do not record:

- Why a judgement was made  
- What alternatives existed  

As a result:

> Actions can be reproduced, but decision-making cannot be learned

By logging judgements:

- Organizations can reflect and improve decisions  
- AI can learn decision-making itself  

---

## 3. Definition of Judgement

Judgement is defined as:

> The act of selecting and fixing one state from multiple possible futures

---

### Characteristics

- Determines state transitions  
- Constrains actions  
- Has an accountable actor  

---

### Judgement Dimensions

- Proceed  
- Validity  
- Accountability  
- Venture  

Venture is not a type of judgement, but a continuous axis of exploration.

---

## 4. Architecture

```text
Discovery → Investment → Learning
```

- Discovery: Identifying judgement structures  
- Investment: Evaluating judgement value  
- Learning: Designing, logging, and improving  

---

## 5. Judgement Structure

```text
Judgement Chain  
└ Judgement Journey  
   └ Judgement Point  
```

Enterprise activity is not a process, but a structure of judgements.

---

## 6. Investment Theory

### Judgement ROI

```text
ROI = Frequency × Impact × Improvement Rate − Cost
```

---

### JULIA

JULIA is a framework for evaluating judgement investment.

It extends traditional ROI-based evaluation by incorporating multiple dimensions.  
This structure is inspired by the Balanced Scorecard (BSC).

---

### JULIA Dimensions

- ROI (Financial)  
- Business Impact (Customer / Business)  
- Automation Potential (Internal Process)  
- Learning Value (Learning)  

JULIA evaluates judgement value in a multi-dimensional manner while incorporating ROI.

---

## 7. Learning System

### JSC

Judgement State Chart

### JDC

Judgement Design Canvas

### JLog

Judgement Log

### VLog

Validation Log

---

### Lifecycle

```text
Before → During → After
```

---

### Learning Loop

```text
Data → AI → Options → Human → JLog → Action → Result → VLog → Learning
```

---

## 8. AI Implementation

### 8.1 Problem of AI Adoption

Failures in AI adoption are caused by incorrect units of application.

```text
Process → Automation (Incorrect)
Judgement → Improvement (Correct)
```

AI can reproduce actions, but cannot learn decision-making.

---

### 8.2 Role of JDA

JDA resolves this problem through the following structure:

```text
Judgement Extraction → JULIA → Design → Logging → Learning
```

---

### 8.3 AI Agent Role Classification

In JDA, AI agents are classified into two types.

---

#### Process AI Agents

**Role:**

- Automate the progression of workflows  
- Execute and orchestrate tasks  
- Proceed to the next step based on judgement results  

**Target:**

- Execution of routine operations  
- Data collection and organization  
- Notification and integration processes  

---

#### Judgement AI Agents

**Role:**

- Collect and structure decision inputs  
- Generate and present options  
- Retrieve similar past judgements from JLog  
- Analyze judgement logs  

**Target:**

- Decision support  
- Option generation  
- Pattern analysis  

---

### 8.4 Relationship

Process agents and judgement agents interact as follows:

```text
Process AI Agent (What to do)
↓
Judgement AI Agent (How to decide)
↓
Human Judgement (Final decision)
↓
JLog (Recording)
↓
Learning (Why it was decided)
```

---

### 8.5 Connection to Enterprise World Model

Through continuous cycles of this structure,  
an enterprise-specific decision model (Enterprise World Model) is formed.

Through accumulation of judgement logs:

- Process agents learn workflow optimization  
- Judgement agents improve decision accuracy  

---

## 9. Positioning

- BI: Data  
- BPM: Process  
- DDD: Model  
- KM: Knowledge  

JDA treats decision-making as a first-class architectural concern.

---

## 10. Venture Judgement

Venture is an axis of exploration,  
and all judgements exist on a continuous spectrum.

---

## 11. Long-term Vision

Construction of the Enterprise World Model

---

## Final Definition

JDA is an architecture that:

- Extracts judgements  
- Evaluates judgements  
- Logs judgements  
- Learns from judgements  

to evolve the decision-making capability of organizations.

---

## License & Citation

Copyright (c) 2026 Shun Takeda (B-AS)  
CC BY 4.0 — <https://creativecommons.org/licenses/by/4.0/>

Citation:  
Takeda, Shun. *Judgement-Driven Architecture*. B-AS, 2026.  
<https://github.com/judgement-driven/Judgement-Driven-Architecture>
