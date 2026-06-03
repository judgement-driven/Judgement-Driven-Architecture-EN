# Judgement-Driven Architecture (JDA)

> This repository contains the original Japanese version of the  
> Judgement-Driven Architecture (JDA) theory and method.
>
> English repository:  
> https://github.com/judgement-driven/Judgement-Driven-Architecture-EN
>
> Judgements are organizational assets.  
> Organizations do not operate only on data — they operate on judgement.

---

# One-line Definition

Judgement-Driven Architecture (JDA) is an architecture for discovering, designing, executing, recording, evaluating, and learning organizational judgements in order to continuously improve decision-making capability.

---

# Why JDA Exists

Most business systems are designed around workflows.

However, real business operations rarely follow workflows cleanly.

In practice, work changes direction continuously based on judgement.

Examples:

- Should we proceed with this opportunity?
- Should we target this company?
- Should we allow this exception?
- Which case should we prioritize?
- Should we postpone this action?
- Who should confirm this issue?

Organizations operate through accumulated judgements.

However, in many organizations:

- Judgements are highly person-dependent
- Judgement reasons are not recorded
- Judgement materials are not shared
- Validity is not evaluated
- AI cannot learn organizational judgement patterns

Organizations already store large amounts of data.

Examples of factual data:

- Sales
- Orders
- Customer information
- Billing information

Examples of behavioral data:

- Clicks
- Views
- Purchases
- Contact history

But organizations also contain another important type of data:

> Judgement data

In the AI era, foundation models themselves will increasingly become commoditized.

Competitive advantage will shift toward:

- What organizations learn
- What judgements they record
- What judgement materials they improve
- How organizational judgement evolves

JDA is an architecture for turning judgement into organizational learning assets.

---

# What is Judgement?

In JDA, judgement is defined as:

> An act that changes organizational state.

Judgement is not a simple if-branch.

Judgement changes business state and determines future actions and future judgements.

```text
State A
↓
Judgement
↓
State B
```

JDA treats judgement through four perspectives:

- Proceed
- Validity
- Accountability
- Exploration

---

# What JDA Focuses On

JDA treats judgement as a first-class architectural concern.

JDA does not treat business as merely a collection of tasks or workflows.

Instead, JDA focuses on discovering and improving the judgements embedded inside business operations.

```text
Discover
↓
Evaluate
↓
Design
↓
Record
↓
Execute
↓
Learn
```

The goal of JDA is not to immediately delegate judgement to AI.

The first goal is to make human judgement visible.

Then:

- organize judgement materials
- record judgement reasons
- record state transitions
- evaluate validity
- accumulate learning assets

AI initially supports judgement materials rather than replacing human judgement.

As JLog and VLog accumulate, AI may eventually support judgement reproduction and partial judgement delegation under controlled conditions.

---

# Core Structure of JDA v1.6

JDA v1.6 discovers Judgement Points (JP) within Business Journeys (BJ), and treats JP as the central unit of design, execution, logging, and learning.

```text
BJ (Discovery Scope)
↓
JP (Judgement Point)

JP → JSC / JDC (Design)
JP → JLog / VLog (Logging)
JP → Learning Cycle (Learning)
```

JDA does not optimize workflows themselves.

JDA continuously improves the judgements embedded within business operations.

---

# Business Journey (BJ)

Business Journey (BJ) is a meaningful business scope that contains judgement.

BJ is not simply a workflow.

BJ is a discovery scope used to identify Judgement Points during Phase1 Discovery.

Examples:

- BJ01 New Client Acquisition
- BJ02 Proposal Creation
- BJ03 Production Management
- BJ04 Billing Process
- BJ05 Payment Confirmation and Collection

---

# Judgement Point (JP)

Judgement Point (JP) is an actual judgement occurring within business operations.

JP is generally expressed in the following form:

```text
Should we ~ ?
```

Examples:

- Should we target this company?
- Should we prioritize this case?
- Should we contact this company?
- Should we classify this as a strong lead?
- Which invoice does this payment belong to?
- Should we postpone this?

JP is not merely a task.

A JP changes future states, actions, and subsequent judgements.

---

# Case / Proposal

JDA treats judgement targets as Cases.

```text
Case = Entity × Context
```

In implementation, Proposal may be used as a concrete executable unit of Case.

Example: BJ01 New Client Acquisition

```text
Entity = Company
Context = Campaign
Proposal = Company × Campaign
```

Proposal becomes the central unit for:

- State management
- JP execution
- JLog recording
- VLog evaluation
- Learning

---

# Judgement Journey (JJ)

Judgement Journey (JJ) is a chain of JP executions.

JP is discovered within BJ during Phase1 Discovery.

However, once discovered, JP becomes a reusable judgement asset rather than remaining permanently tied to BJ.

JJ emerges and becomes observable during Phase5 Implementation and later phases, as JP executions update Proposal / Case states, attributes, and judgement materials.

In summary:

```text
BJ = Discovery scope for JP
JP = Judgement point
JJ = Executed chain of judgements
```

---

# JSC

JSC (Judgement State Chart) is a design artifact for modelling state transitions caused by judgement.

JSC focuses on state rather than procedural sequence.

```text
before_state
↓
JP
↓
after_state
```

JDA treats judgement as state transition.

Therefore, hold states, exceptions, retries, and re-judgements are also treated as states.

---

# JDC

JDC (Judgement Design Canvas) is a design artifact for structuring judgement itself.

JDC organizes:

- Judgement definition
- Judgement target
- Judgement materials
- Judgement conditions
- Judgement perspectives
- Judgement results
- Judgement actor
- Judgement accountability
- Judgement finalization method
- Outputs

JDC makes judgement implementable, recordable, and learnable.

---

# JLog / VLog

JDA records judgement through two types of logs.

```text
JLog = Judgement-time log
VLog = Post-judgement validity log
```

JLog records:

- Who made the judgement
- What was judged
- Which state the judgement occurred in
- Which judgement materials were used
- Which conditions and perspectives were used
- Why the judgement was made
- Which state transition occurred afterward

VLog records:

- Whether the judgement result was valid
- Whether judgement materials were appropriate
- Whether judgement reasoning was valid
- What the actual outcome was
- How future judgement should improve

Together, JLog and VLog make judgement learnable.

---

# Judgement Injection

Judgement Injection is a key implementation concept in JDA v1.6.

Traditional business systems often embed judgement logic directly into code or UI.

JDA instead treats JP as a managed definition injected into an execution harness.

```text
JP Definition
↓
execute_jp
↓
State Transition
↓
JLog Recording
```

This separates judgement definitions from execution infrastructure.

Judgement becomes:

- a design target
- an operational target
- a learning target

rather than hardcoded business logic.

---

# Learning Cycle

The JDA Learning Cycle enables staged organizational judgement learning.

```text
Judgement Material Learning
↓
Judgement Reproduction Learning
↓
Judgement Delegation
```

---

## Stage1: Judgement Material Learning

Initially, AI supports judgement materials rather than judgement itself.

Examples:

- showing similar cases
- summarizing judgement materials
- assisting judgement reason input
- identifying missing information
- presenting previous judgements

---

## Stage2: Judgement Reproduction Learning

As JLog and VLog accumulate, AI can begin supporting judgement reproduction.

```text
AI → Suggested Judgement
Human → Confirm
```

---

## Stage3: Judgement Delegation

When sufficient logs and validity evaluations accumulate, certain judgements may eventually be delegated to AI under controlled conditions.

However, judgement delegation always requires accountability design.

---

# JDA Method v1.6

JDA Method v1.6 consists of the following phases:

```text
Phase0 Foundation
↓
Phase1 Discovery
↓
Phase2 JULIA
↓
Phase3 Design
↓
Phase4 Log
↓
Phase5 Implementation
↓
Phase6 Learning
```

---

# Phase0 Foundation

Understand the judgement domain and define the Business Journeys (BJ) that become the scope for Phase1 Discovery.

Main outputs:

- JDA-BMC
- Business Journey list
- Target BJ

---

# Phase1 Discovery

Extract actual Judgement Points (JP) within the target BJ scope.

Phase1 does not design JJ.

Main outputs:

- JP list
- JP refinement records
- JP merge/exclusion notes

---

# Phase2 JULIA

JULIA (Judgement Log Impact Assessment) evaluates extracted JP and determines which judgements should be prioritized.

Evaluation dimensions:

- ROI
- Business Impact
- Automation Potential
- Learning Value

Phase2 determines:

```text
Which judgements deserve investment
```

---

# Phase3 Design

Design judgement structure, state transitions, judgement materials, accountability, and execution units for selected JP.

Main outputs:

- JSC
- JDC
- Case / Proposal definitions
- Judgement material definitions
- Accountability definitions

---

# Phase4 Log

Make designed judgements recordable as JLog and VLog.

Main outputs:

- JLog definitions
- VLog definitions
- Logging timing definitions
- Validity evaluation methods

---

# Phase5 Implementation

Design and implement the JDA execution infrastructure.

Key elements:

- Harness
- execute_jp
- State management
- Proposal / Case
- JLog / VLog
- Operational Bridge

---

# Phase6 Learning

Improve judgement materials, conditions, perspectives, and thresholds using accumulated JLog and VLog.

```text
Judgement Material Learning
↓
Judgement Reproduction Learning
↓
Judgement Delegation
```

---

# Implementation Pattern

JDA v1.6 defines Judgement Slice Implementation as its primary implementation strategy.

Judgement Slice Implementation means:

> Implementing judgement materials, judgement input, state transitions, and JLog/VLog collection first around high-priority JP selected through JULIA, while supplementing surrounding processes through Operational Bridge.

JDA implementation does not attempt to fully automate everything from the beginning.

Instead:

```text
Deploy the smallest structure capable of recording judgement logs first
```

JJ emerges later through actual JP execution during operation.

---

# Relationship with AI

JDA is not primarily an AI adoption framework.

JDA is an architecture for designing structures that AI can support and eventually learn from.

Initially:

```text
AI = Judgement material support
Human = Judgement actor
JLog / VLog = Learning assets
```

AI does not initially replace human judgement.

AI supports:

- judgement materials
- observations
- hypotheses
- missing information
- previous cases

Judgement delegation only becomes possible after sufficient logging and validity confirmation.

---

# Long-term Vision

The long-term vision of JDA is the construction of an Enterprise World Model.

Organizations can accumulate not only business data, but also judgement data.

As judgement data accumulates, organizations can develop:

- organization-specific judgement history
- organization-specific judgement materials
- organization-specific judgement criteria
- organization-specific judgement models

JDA is an architecture for organizational judgement learning.

---

# Repository Structure

```text
.
├── core/
│   └── JDA_core_v1.6.md
│
├── method/
│   ├── 00_overview.md
│   ├── 01_phase0_foundation.md
│   ├── 02_phase1_discovery.md
│   ├── 03_phase2_julia.md
│   ├── 04_phase3_design.md
│   ├── 05_phase4_log.md
│   ├── 06_phase5_implementation.md
│   ├── 06a_judgement_slice_implementation.md
│   ├── 07_phase6_learning.md
│   └── JDA_BMC_definition.md
│
├── implementation/
│   └── BJ01/
│
└── tools/
    └── jda_phase_template.html
```

---

# Current Status

JDA Core v1.6 and JDA Method v1.6 are currently organized around:

- Judgement as state transition
- Business Journey as JP discovery scope
- JP as reusable judgement asset
- Judgement Injection
- JLog / VLog
- Judgement Slice Implementation
- Learning Cycle

---

# License

Copyright (c) 2026 Shun Takeda (B-AS)

Licensed under the Creative Commons Attribution 4.0 International License (CC BY 4.0).

https://creativecommons.org/licenses/by/4.0/

---

# Citation

If you use this theory in research, articles, presentations, or other materials, please cite:

Judgement-Driven Architecture (JDA)  
Author: Shun Takeda (B-AS)  
GitHub Repository  
https://github.com/judgement-driven/Judgement-Driven-Architecture

## BibTeX

```bibtex
@misc{JDA2026,
  title={Judgement-Driven Architecture},
  author={Takeda, Shun},
  year={2026},
  howpublished={GitHub Repository},
  organization={B-AS},
  url={https://github.com/judgement-driven/Judgement-Driven-Architecture}
}
```
