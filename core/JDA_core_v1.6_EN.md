# JDA Core v1.6 — Judgement-Driven Architecture

## 1. What is JDA?

Judgement-Driven Architecture (JDA) is an architecture that treats judgement as a first-class design target.

Traditional business systems primarily model:

- workflows
- procedures
- transactions
- tasks
- events

However, real organizational operations do not proceed only through procedures.

Organizations continuously change direction through judgement.

Examples:

- Should we proceed?
- Should we prioritize this?
- Should we contact this company?
- Should we allow this exception?
- Should we escalate this issue?
- Should we postpone this action?

JDA focuses on these organizational judgements.

---

# 2. Why Judgement Matters

Organizations already accumulate large amounts of data.

Examples:

## Fact Data

- Sales
- Orders
- Customer information
- Billing records

## Behavioral Data

- Clicks
- Views
- Purchase history
- Contact history

However, organizations also generate another critical type of data:

> Judgement Data

Judgement data includes:

- why decisions were made
- what was considered
- which state existed at the time
- what alternatives existed
- which assumptions were held
- what outcome occurred afterward

Most organizations lose this information.

As a result:

- judgement becomes person-dependent
- organizational learning stagnates
- AI cannot reproduce judgement patterns
- mistakes repeat
- successful patterns cannot scale

JDA treats judgement itself as an organizational learning asset.

---

# 3. Definition of Judgement

In JDA, judgement is defined as:

> An act that changes organizational state.

Judgement is not merely a conditional branch.

Judgement changes future organizational behavior.

```text
State A
↓
Judgement
↓
State B
```

A judgement:

- changes state
- determines future actions
- influences future judgement
- affects organizational learning

---

# 4. Four Perspectives of Judgement

JDA treats judgement through four perspectives.

## Proceed

Should the organization proceed?

Example:

- proceed
- reject
- hold
- retry
- escalate

---

## Validity

Was the judgement appropriate?

Example:

- Was the judgement material sufficient?
- Was the reasoning appropriate?
- Was the outcome acceptable?

---

## Accountability

Who owns responsibility for the judgement?

JDA separates:

- judgement actor
- judgement responsibility

AI may support judgement,
but accountability may remain human or organizational.

---

## Exploration

Judgement is not always optimization.

Organizations sometimes explore uncertainty.

Examples:

- testing new markets
- trying experimental proposals
- acting under incomplete information

JDA treats exploratory judgement as a valid organizational behavior.

---

# 5. Judgement as State Transition

JDA models judgement primarily as state transition.

```text
before_state
↓
Judgement
↓
after_state
```

This differs from traditional workflow-centric systems.

JDA focuses on:

- state
- transition
- judgement
- learning

rather than purely procedural sequence.

Therefore:

- exceptions
- retries
- holds
- re-judgements

are also treated as explicit states.

---

# 6. Business Journey (BJ)

Business Journey (BJ) is a meaningful business scope that contains judgement.

BJ is not simply a workflow.

BJ is used as a discovery scope for identifying Judgement Points.

Examples:

- New Client Acquisition
- Proposal Management
- Production Management
- Billing Process
- Payment Collection

BJ exists primarily during discovery phases.

---

# 7. Judgement Point (JP)

Judgement Point (JP) is the core unit of JDA.

A JP is an actual judgement occurring within business operations.

JP is generally expressed as:

```text
Should we ~ ?
```

Examples:

- Should we target this company?
- Should we classify this as a strong lead?
- Should we prioritize this case?
- Should we hold this proposal?
- Should we escalate this issue?

JP is not merely a task.

A JP changes future state and future organizational behavior.

---

# 8. Judgement ROI and JULIA

JDA designs around:

> Which judgements deserve investment

---

## 8.1 Judgement Investment

JDA prioritizes:

> Which judgements to invest in

JULIA determines investment priority for judgement improvement, implementation, and learning.

---

## 8.2 JULIA

JULIA (Judgement Scorecard) evaluates JP importance and determines which judgements should be prioritized for improvement, implementation, and learning.

The name JULIA comes from the initials of its five evaluation dimensions.

JDA does not treat the following as equivalent:

- discovered JP
- JP selected for design
- JP selected for implementation

Evaluation dimensions:

- J = Judgement Financial Impact
- U = Urgency & Frequency
- L = Latency
- I = Influence Scope
- A = Adaptive / Learning Value

---

## 8.3 Evaluation Unit and Implementation Unit

```text
Evaluation unit: JP
Implementation unit: BJ
```

---

# 9. Judgement Journey (JJ)

Judgement Journey (JJ) is an executed chain of JP.

JP is initially discovered within BJ.

However, after discovery, JP becomes a reusable judgement asset.

JJ emerges during implementation and operation when JP executions update:

- states
- attributes
- judgement materials
- organizational learning

Therefore:

```text
BJ = Discovery scope
JP = Judgement unit
JJ = Executed judgement chain
```

---

# 10. JSC — Judgement State Chart

JSC models judgement-driven state transitions.

JSC focuses on:

- states
- transitions
- judgement execution

rather than procedural sequence.

Example:

```text
Lead Identified
↓
JP: Should we contact?
↓
Contacted
```

JSC may also include:

- hold states
- retry states
- exception states
- re-evaluation states

---

# 11. JDC — Judgement Design Canvas

JDC structures judgement itself.

JDC organizes:

- judgement target
- judgement materials
- judgement conditions
- judgement perspectives
- judgement actor
- judgement accountability
- outputs
- validity criteria

JDC makes judgement:

- implementable
- observable
- recordable
- learnable

---

# 12. JLog / VLog

JDA records judgement through two primary logs.

## JLog

Records judgement at execution time.

Examples:

- who judged
- what was judged
- which state existed
- which materials were used
- why judgement occurred
- which transition occurred

---

## VLog

Records post-judgement validity evaluation.

Examples:

- Was the judgement correct?
- Was the reasoning appropriate?
- Was the outcome successful?
- What should improve next time?

Together, JLog and VLog enable organizational judgement learning.

---

# 13. Judgement Injection

Judgement Injection is a central implementation concept in JDA.

Traditional systems often embed judgement directly into code.

JDA instead separates:

- judgement definition
- execution infrastructure

```text
JP Definition
↓
execute_jp
↓
State Transition
↓
JLog Recording
```

This allows judgement to become:

- configurable
- reusable
- observable
- improvable

rather than hardcoded logic.

---

# 14. Learning Cycle

JDA learning proceeds in stages.

```text
Judgement Material Learning
↓
Judgement Reproduction Learning
↓
Judgement Delegation
```

---

## Stage1 — Judgement Material Learning

AI initially supports judgement materials.

Examples:

- summarizing information
- presenting similar cases
- suggesting missing information
- organizing judgement inputs

---

## Stage2 — Judgement Reproduction Learning

As JLog and VLog accumulate,
AI may support judgement reproduction.

```text
AI → Suggested Judgement
Human → Confirm
```

---

## Stage3 — Judgement Delegation

When sufficient validity and learning accumulate,
specific judgements may eventually be delegated to AI.

However, accountability design remains essential.

---

# 15. Relationship with AI

JDA is not primarily an AI adoption framework.

JDA designs structures that AI can support and eventually learn from.

Initially:

```text
AI = Judgement material support
Human = Judgement actor
JLog / VLog = Learning assets
```

AI does not initially replace human judgement.

Instead, AI supports:

- judgement materials
- observations
- hypotheses
- missing information
- previous cases

JDA prioritizes organizational judgement learning over simple automation.

---

# 16. Enterprise World Model

The long-term vision of JDA is the construction of an Enterprise World Model.

Organizations can accumulate:

- organization-specific judgement history
- organization-specific judgement materials
- organization-specific judgement criteria
- organization-specific judgement patterns

As organizational judgement accumulates,
AI may eventually support increasingly sophisticated organizational reasoning.

---

# 17. Current Direction of JDA v1.6

JDA v1.6 is currently organized around:

- judgement as state transition
- BJ as JP discovery scope
- JP as reusable judgement asset
- JSC / JDC
- JLog / VLog
- Judgement Injection
- Learning Cycle
- Judgement Slice Implementation
