# Judgement-Driven Architecture

🌐 **Languages**

-   English
-   Japanese (Original):
    https://github.com/judgement-driven/Judgement-Driven-Architecture

> **Preserve decisions. Organizations become smarter.**\
> **Companies are driven not by data, but by decisions.**

**One-line definition**

Judgement-Driven Architecture (JDA) is a theory for designing **a
decision infrastructure where organizational judgements are structured
as logs and continuously learned from by both humans and AI.**

------------------------------------------------------------------------

# Why This Theory Was Created

Many business activities are described as flows.

Business processes, process diagrams, workflows, and many other formats
are used to organize work.

However, real work does not flow cleanly according to those diagrams.

**In reality, work constantly changes direction based on decisions.**

For example:

-   Should we proceed with this deal?
-   Should we allow this exception?
-   Which option should we prioritize?

Business operations advance through the accumulation of such decisions.

However, these decisions usually have the following problems:

-   They become dependent on individuals
-   The reasoning behind them is not recorded
-   Their validity is not evaluated later
-   AI cannot use them

Companies already possess large amounts of data.

### Fact Data

-   Sales
-   Orders
-   Product information

### Behavioral Data

-   Clicks
-   Views
-   Purchases

However, there is another critical type of data in organizations:

> **Decision Data**

For example, in sales:

-   Prioritized Company A
-   Dropped this deal
-   Proceeded with this proposal

Such decisions occur every day.

But usually the following are not recorded:

-   Why the decision was made
-   What information was considered
-   Whether the decision was correct

Judgement-Driven Architecture (JDA) is a theory that designs a structure
where

> **decisions are treated as states, stored as logs, and made
> learnable.**

------------------------------------------------------------------------

# What is JDA

Judgement-Driven Architecture (JDA) is

> **a design theory that structures decisions as units of learning.**

JDA is not:

-   A simple business process improvement method
-   An AI implementation framework
-   An organizational transformation theory

Instead, JDA is

> **a theory for designing systems where humans and AI continuously
> learn from decisions.**

------------------------------------------------------------------------

# Terms and Abbreviations

  Abbreviation   Meaning
  -------------- ---------------------------------
  JDA            Judgement-Driven Architecture
  JP             Judgement Point
  JSC            Judgement State Chart
  JULIA          Judgement Log Impact Assessment
  JDC            Judgement Design Canvas
  JLog           Judgement Log
  VLog           Validity Log

------------------------------------------------------------------------

# Definition of Judgement

## What is a Judgement

A judgement is

**an act that fixes a state.**

Every judgement has four aspects:

-   Proceed
-   Validity
-   Accountability
-   Venture

------------------------------------------------------------------------

## What is Fixing a State

Fixing a state means that a responsible actor locks a state and
constrains the next transition.

In other words,

> **A judgement is the act of narrowing future possibilities to one
> path.**

------------------------------------------------------------------------

## What is a Log

A log is the record of that fixation.

It records:

-   Who made the decision
-   What decision was made
-   Why the decision was made

------------------------------------------------------------------------

## What is Learning

Learning means evaluating the validity of those past decisions and
reflecting them into future decision criteria.

------------------------------------------------------------------------

# Venture Judgement

Proceed / Validity / Accountability provide a structure for safe
decision cycles.

However, organizations also need

> **decisions that select outside the existing distribution.**

A Venture Judgement is

> **a decision that intentionally accepts risk because the potential
> upside is discontinuously large.**

Prerequisites:

-   Defined acceptable loss
-   Defined exit criteria
-   Designed number of trials
-   Clear responsibility
-   Logged reasoning

------------------------------------------------------------------------

## Examples of Venture Judgements

### Executive Level

-   Nintendo: Famicom (NES)
-   Sony: Walkman

### Operational Level

-   Experimental proposal to a new client
-   Creative approach that breaks the standard playbook
-   Small-scale experimental project

------------------------------------------------------------------------

# JDA Design Principles

1.  Do not change the existing flow
2.  Treat decisions as units of learning
3.  AI presents decision materials
4.  Allow venture judgements
5.  Decision logs create learning cycles

------------------------------------------------------------------------

# Overall Structure of JDA

``` mermaid
flowchart LR
    Domain[Domain Definition]
    Extract[Judgement Extraction]
    Prioritize[Prioritization]
    Design[Judgement Design]
    Log[Log Design]
    Implement[Implementation]
    Learn[Learning]

    Domain --> Extract --> Prioritize --> Design --> Log --> Implement --> Learn
    Learn --> Design
```

------------------------------------------------------------------------

# Phase Overview

JDA is implemented through the following phases.

## Phase 0 --- Establish the Decision Foundation

-   Define decision domain boundaries
-   Extract business journeys
-   Do not optimize yet
-   Do not design a "ToBe" process

------------------------------------------------------------------------

## Phase 1 --- Judgement Extraction

-   Decompose business journeys
-   Enumerate Judgement Points (JP)
-   Define Judgement State Charts (JSC)

------------------------------------------------------------------------

## Phase 2 --- Prioritization (JULIA)

Evaluation axes:

-   Impact
-   Frequency
-   Individual dependency
-   Learning value

------------------------------------------------------------------------

## Phase 3 --- Judgement Design (JDC)

Define:

-   Human decision
-   AI-supported decision
-   AI-substituted decision
-   Venture judgement
-   Responsible actor
-   Escalation rules

------------------------------------------------------------------------

## Phase 4 --- Log Design

Define logs for:

-   Decision materials
-   Decision options
-   Decision results
-   Decision reasoning
-   Validity evaluation

------------------------------------------------------------------------

## Phase 5 --- Implementation

-   DB / JSON schema design
-   UI design
-   Workflow integration
-   AI integration (LLM / RAG / SLM)

------------------------------------------------------------------------

## Phase 6 --- Learning

-   Validity review
-   Decision trend analysis
-   Venture review
-   Criteria updates

------------------------------------------------------------------------

# Decision Log Loop (JDA Learning Loop)

``` mermaid
flowchart LR
    DATA[Data]
    AI[AI organizes materials]
    OPTION[Decision options]
    HUMAN[Human decision]
    JLOG[Judgement Log]
    ACTION[Action]
    RESULT[Result]
    VLOG[Validity Log]
    LEARN[Learning]

    DATA --> AI
    AI --> OPTION
    OPTION --> HUMAN
    HUMAN --> JLOG
    JLOG --> ACTION
    ACTION --> RESULT
    RESULT --> VLOG
    VLOG --> LEARN
    LEARN --> AI
```

------------------------------------------------------------------------

# Minimal Implementation Example

``` python
options = AI.propose_options(context)

decision = human.select(options)

JLog.save(
    context=context,
    decision=decision,
    options=options
)

result = observe_result()

VLog.save(
    decision=decision,
    result=result
)

AI.learn(JLog, VLog)
```

------------------------------------------------------------------------

# Positioning of JDA

  Field                 Focus                     What is Stored
  --------------------- ------------------------- -------------------
  BI                    Fact Data                 Sales / Logs
  Process Improvement   Business Flow             Procedures
  AI                    Prediction / Generation   Models
  **JDA**               **Decision Making**       **Decision Logs**

JDA operates in

> **the domain of decisions.**

------------------------------------------------------------------------

# Relationship with AI

JDA is not an AI adoption framework.

Instead, it is

> **a theory for designing a structure where AI can naturally
> integrate.**

AI roles:

-   Collect decision materials
-   Organize information
-   Generate options
-   Optimize

Human roles:

-   Final judgement
-   Venture judgement
-   Responsibility judgement

------------------------------------------------------------------------

# Long-Term Vision

The long-term goal of JDA is to accumulate organizational decision logs
and allow them to be shared by both organizations and AI.

This leads to the creation of a

> **Corporate World Model**

This enables:

-   Accelerated organizational learning
-   AI decision support
-   Preservation of corporate culture

------------------------------------------------------------------------

# License

Copyright (c) 2026 Shun Takeda (B-AS)

This project is released under the\
**Creative Commons Attribution 4.0 International License (CC BY 4.0).**

Full license text:\
https://creativecommons.org/licenses/by/4.0/

------------------------------------------------------------------------

# Citation

If you use this theory in research, articles, or publications, please
cite:

Judgement-Driven Architecture\
Author: Shun Takeda (B-AS)\
GitHub Repository\
https://github.com/judgement-driven/Judgement-Driven-Architecture

------------------------------------------------------------------------

## BibTeX

``` bibtex
@misc{JDA2026,
  title={Judgement-Driven Architecture},
  author={Takeda, Shun},
  year={2026},
  howpublished={GitHub Repository},
  organization={B-AS},
  url={https://github.com/judgement-driven/Judgement-Driven-Architecture}
}
```
