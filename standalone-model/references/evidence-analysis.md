---
name: evidence-analysis
description: Assess source coverage, analytics integrity, and apparent qualitative-quantitative conflicts without overstating what the evidence proves.
---

# Evidence Analysis

## Purpose

Use this reference when several sources or participants are supplied, when product analytics are part of the evidence, or when measured behaviour and reported experience appear to disagree. Context Reader uses it to assess evidence quality and classify conflicts without explaining causes. Research Guide may continue into hypotheses or a resolving study.

## Preserve source coverage

Assign each source or participant a short identifier before combining material. Process every readable source and retain its identifier on material observations.

- Do not let the first, longest, most vivid, or most recent source dominate the result.
- Confirm that every supplied source contributed to the analysis or state why it did not.
- Mark a pattern supported by only one source as single-source rather than discarding or generalising it.
- Separate recurrence from consequence. A rare issue may still matter when the harm is high.

This is a coverage check, not a rule that every participant must appear in the final answer when they add no relevant evidence.

## Before trusting product data

Check the integrity of the measure before treating its shape as a design signal:

1. **Event meaning:** verify what action or system condition actually fires the event rather than trusting its label.
2. **Denominator:** check whether audience or acquisition changes explain a rate movement.
3. **Path model:** determine whether the funnel assumes an order that the product does not enforce.
4. **Time boundary:** align changes with releases, instrumentation changes, campaigns, seasonality, or operational events.
5. **Segments:** inspect whether platform, market, user type, or entry point behaves differently from the aggregate.
6. **Missing boundary:** identify behaviour occurring before instrumentation begins or after it ends.

Context Reader reports whether these checks strengthen or weaken the evidence. It does not name the UX cause.

## From analytics to research hypotheses

Research Guide may interpret trustworthy patterns as hypotheses. For each hypothesis, state:

- the observed shape and affected segment;
- the proposed mechanism, explicitly labelled as a hypothesis;
- what observation would disprove it;
- whether existing data, a recording, direct observation, or a conversation can answer it;
- the cheapest responsible way to kill or retain it.

Rank hypotheses by decision value and how cheaply they can be discriminated, not by narrative plausibility.

Useful shapes include a single-step cliff, gradual multi-step attrition, retention that stabilises, retention that continues falling, or two distinct time-on-task groups. Treat these as prompts for investigation, never automatic diagnoses.

## When qualitative and quantitative evidence disagree

First determine whether the conflict is real:

- Do both sources describe the same population, moment, and task?
- Does instrumentation cover the behaviour discussed in research?
- Is one source answering a frequency question while the other answers an intent question?
- Is the apparent conflict caused by aggregation hiding a small but affected segment?

Give questions to the evidence capable of answering them:

| Question | Stronger source |
| --- | --- |
| What happened, where, and how often? | Behavioural or operational evidence |
| Why did it happen, and what was the person trying to accomplish? | Direct research or observation |
| Is the proposed work worth doing? | A design and product judgment informed by both, not a finding from either alone |

When a material conflict remains, define one narrow resolving study. Before it runs, state the disputed claim, the result that would overturn the qualitative account, and the result that would overturn the quantitative account. If no possible result would change the decision, the activity is advocacy rather than resolution.

## Ground rules

- Do not infer causation from a funnel or retention curve.
- Do not ask a dashboard to explain intent.
- Do not use a small qualitative sample to estimate prevalence.
- Do not average conflicting sources into a compromise neither supports.
- State confidence and evidence limitations alongside every material conclusion.
