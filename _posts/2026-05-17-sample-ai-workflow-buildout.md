---
title: "Sample: AI workflow buildout"
description: A build-log style post for showing the before/after shape of an AI-assisted operational workflow.
categories: build-log ai-systems operations
references:
  - label: Sample workflow diagram for visual testing only
    url: /writing/
---

<p class="sample-note">Sample article format. This is a visual test for build logs, workflow diagrams, and review-load charts.</p>

This is the kind of post I would use when the writing is about building something, not only arguing for it.

The format should make the workflow visible: what the human did before, what the system prepares now, where review still happens, and which error modes remain unacceptable.

## Before and after

<figure class="chart-card">
  <figcaption>
    <strong>Figure 1.</strong> A simple workflow map. The point is not to make the process look automated; it is to show where automation stops.
  </figcaption>
  <div class="flow-chart" role="img" aria-label="Sample AI workflow map">
    <div class="flow-step">Raw export</div>
    <div class="flow-step">Normalize fields</div>
    <div class="flow-step accent">AI draft</div>
    <div class="flow-step review">Human review</div>
    <div class="flow-step">Final report</div>
  </div>
</figure>

The shape of the build matters more than the model choice. If the review step is fake, the system is fragile. If the source boundary is unclear, the output will eventually lie with confidence.

## Review load

<figure class="chart-card">
  <figcaption>
    <strong>Figure 2.</strong> Illustrative review load by task type after the workflow is split into preparation, drafting, and approval.
  </figcaption>
  <div class="stack-chart" role="img" aria-label="Illustrative review load by task type">
    <div class="stack-row">
      <span class="stack-label">Before</span>
      <span class="stack-bar">
        <span class="stack-segment manual" style="--value: 72%;">Manual prep</span>
        <span class="stack-segment review" style="--value: 28%;">Review</span>
      </span>
    </div>
    <div class="stack-row">
      <span class="stack-label">After</span>
      <span class="stack-bar">
        <span class="stack-segment automated" style="--value: 42%;">System prep</span>
        <span class="stack-segment ai" style="--value: 30%;">AI draft</span>
        <span class="stack-segment review" style="--value: 28%;">Review</span>
      </span>
    </div>
  </div>
</figure>

## What I would publish

The article would include the parts that are normally omitted:

- the source files used,
- the handoff from system to reviewer,
- the checks that prevent silent failure,
- the remaining cases that still need manual handling.

The tone can stay personal. Something like: "This worked better after I stopped trying to make the AI sound complete and made the review state explicit."
