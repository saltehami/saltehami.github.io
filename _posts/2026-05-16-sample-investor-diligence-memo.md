---
title: "Sample: investor diligence memo"
description: A memo format for testing a company's AI workflow claims against source evidence and operational risk.
categories: strategy diligence ai-systems
references:
  - label: Sample scoring rubric for visual testing only
    url: /writing/
---

<p class="sample-note">Sample article format. This is a mock diligence memo structure, not a real company assessment.</p>

This format is for writing that is closer to investor diligence: a company claims its AI product changes a workflow, and the question is whether that claim survives contact with the actual operation.

## The claim

The company says its system reduces administrative work by preparing the first draft of a recurring clinical operations report.

That claim is not enough. The diligence question is where the work moved.

<figure class="chart-card">
  <figcaption>
    <strong>Figure 1.</strong> Mock evidence score. A good AI workflow claim needs more than product screenshots.
  </figcaption>
  <div class="score-grid" role="img" aria-label="Mock diligence evidence score">
    <div class="score-cell strong">
      <span>Workflow specificity</span>
      <strong>High</strong>
    </div>
    <div class="score-cell medium">
      <span>Source traceability</span>
      <strong>Medium</strong>
    </div>
    <div class="score-cell weak">
      <span>Review path</span>
      <strong>Weak</strong>
    </div>
    <div class="score-cell medium">
      <span>Deployment proof</span>
      <strong>Medium</strong>
    </div>
  </div>
</figure>

## The evidence test

The useful memo separates three questions:

1. What work did the product actually remove?
2. What work did it move to another person or queue?
3. What failure modes become harder to see?

<figure class="chart-card">
  <figcaption>
    <strong>Figure 2.</strong> Mock work transfer. Time saved in one role can reappear as review, exception handling, or data cleanup elsewhere.
  </figcaption>
  <div class="bar-chart compact" role="img" aria-label="Mock work transfer by workflow stage">
    <div class="bar-row">
      <span class="bar-label">Original manual work</span>
      <span class="bar-track"><span class="bar-fill burgundy" style="--value: 86%;"></span></span>
      <span class="bar-value">86</span>
    </div>
    <div class="bar-row">
      <span class="bar-label">System-prepared work</span>
      <span class="bar-track"><span class="bar-fill teal" style="--value: 58%;"></span></span>
      <span class="bar-value">58</span>
    </div>
    <div class="bar-row">
      <span class="bar-label">Human review</span>
      <span class="bar-track"><span class="bar-fill orange" style="--value: 31%;"></span></span>
      <span class="bar-value">31</span>
    </div>
    <div class="bar-row">
      <span class="bar-label">Exception cleanup</span>
      <span class="bar-track"><span class="bar-fill purple" style="--value: 18%;"></span></span>
      <span class="bar-value">18</span>
    </div>
  </div>
</figure>

## The memo answer

The article would end with a short answer, not a vibe:

> The product appears credible as workflow infrastructure if the buyer already has clean exports and a real review owner. It is weaker as a standalone automation claim because the exception queue is still underspecified.

That is the kind of conclusion this format is meant to support.
