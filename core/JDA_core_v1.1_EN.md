# JDA Core v1.1

## Judgement-Driven Architecture

---

## 1. Introduction

In recent years, advances in AI have significantly changed how organizations approach decision-making.  
However, many AI initiatives face common problems:

- Unclear where AI should be applied  
- Proofs of concept (PoCs) do not reach production  
- ROI is difficult to explain  
- AI adoption becomes an end in itself  

The root cause of these issues lies in the unit of application.

Most AI initiatives are designed around business processes:

Business → Automation

However, real organizational activity follows a different structure:

Information → Judgement → Action → Result

Actions determine outcomes, but actions themselves are determined by judgements.

Therefore, the fundamental unit of an organization is not “business process” but “judgement”.

Furthermore, in the AI era, AI models themselves are becoming commoditized.  
Competitive advantage will shift from:

- Which AI you use  

to:

- What you make AI learn  

This leads to a critical problem:

Organizations do not know what data they should collect and learn from.

While proprietary data is widely discussed, the following are not clearly defined:

- What data should be collected  
- How it should be structured  
- How it should be used for learning  

This research proposes the following hypothesis:

> Proprietary data in the AI era is “judgement data”.

Judgement-Driven Architecture (JDA) is an architecture that extracts, structures, and logs judgements, enabling both humans and AI to learn from them.

---

## 2. Core Hypothesis

JDA is based on the following hypotheses.

### Hypothesis 1: Organizations are driven by judgements, not data

While data describes organizational activity,  
it is judgement that actually changes the state of the organization.

Data is only input; judgement is the control unit.

---

### Hypothesis 2: Organizational outcomes depend on judgement quality

Actions are selected through judgement.  
Therefore, outcomes depend not on actions themselves but on the quality of the underlying judgements.

---

### Hypothesis 3: Organizational culture is the accumulation of judgements

Organizational culture is not defined by formal rules,  
but by the accumulation of daily decision patterns.

Repeated judgements shape how an organization behaves.

---

### Hypothesis 4: Judgement logs enable learning for both organizations and AI

Traditional systems record:

- What happened (data)  
- What was done (actions)  

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

Judgement is:

The act of selecting and fixing one state among multiple possible futures.

### Properties

- Determines state transitions  
- Constrains subsequent actions  
- Has a responsible actor  

---

### Judgement Dimensions

- Proceed  
- Validity  
- Accountability  
- Venture  

Venture is not a type of judgement, but a dimension representing exploration.

---

## 4. Architecture

Discovery → Investment → Learning

- Discovery: Identify judgement structures  
- Investment: Evaluate judgement value  
- Learning: Design, log, and learn  

---

## 5. Judgement Structure

Judgement Chain  
└ Judgement Journey  
   └ Judgement Point  

Organizations should be understood as structures of judgements rather than processes.

---

## 6. Investment Theory

### Judgement ROI

ROI = Frequency × Impact × Improvement Rate − Cost

---

### JULIA

JULIA is a judgement investment evaluation framework.

It extends traditional ROI-based evaluation by incorporating multiple dimensions.

This structure is inspired by the Balanced Scorecard (BSC).

---

### JULIA Dimensions

- ROI (Financial)  
- Business Impact (Customer / Business)  
- Automation Potential (Internal Process)  
- Learning Value (Learning)  

JULIA incorporates ROI while enabling multi-dimensional evaluation.

---

## 7. Learning System

### JSC (Judgement State Chart)

State transition model driven by judgements.

---

### JDC (Judgement Design Canvas)

Framework for designing judgements.

---

### JLog

Judgement log (decision, context, reasoning).

---

### VLog

Validity log (post-evaluation of judgement).

---

### Lifecycle

Before → During → After

---

### Learning Loop

Data → AI → Options → Human → JLog → Action → Result → VLog → Learning

---

## 8. AI Implementation

Failures in AI adoption stem from incorrect unit selection.

Business → Automation (incorrect)  
Judgement → Improvement (correct)  

AI can reproduce actions but cannot learn decision-making.

JDA resolves this through:

Judgement Extraction → JULIA → Design → Logging → Learning

---

## 9. Positioning

- BI: Data  
- BPM: Process  
- DDD: Model  
- KM: Knowledge  

JDA treats decision-making as a first-class system.

---

## 10. Venture Judgement

Venture represents the exploration dimension of judgement.  
All judgements exist on a continuous spectrum of exploration.

---

## 11. Long-term Vision

Construction of an Enterprise World Model.

---

## Final Definition

JDA is an architecture that:

Extracts judgements  
Evaluates judgements  
Logs judgements  
Learns from judgements  

to continuously improve organizational decision-making capability.

## License & Citation

Copyright (c) 2026 Shun Takeda（B-AS）  
CC BY 4.0 — <https://creativecommons.org/licenses/by/4.0/>

Citation : Takeda, Shun. Judgement-Driven Architecture. B-AS, 2026.  
<https://github.com/judgement-driven/Judgement-Driven-Architecture>
