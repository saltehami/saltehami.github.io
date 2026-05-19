---
title: "Sample: clinic data quality audit"
description: A case-style post that uses charts to show where an operating report can and cannot be trusted.
categories: case-study data-work healthcare-operations
references:
  - label: Sample numbers for visual testing only
    url: /writing/
---

<p class="sample-note">Sample article format. The numbers are illustrative and should be replaced with real source exports before publishing.</p>

The first pass on a healthcare data project is usually not a dashboard. It is an argument about what the data can support.

This format is for a case-style post where the story is: what did we think the report meant, what did the raw data actually contain, and which metrics are safe enough to use?

## The question

Can a clinic-facing compliance report be trusted for daily operating decisions, or is it mixing clean-looking metrics with partial source coverage?

<figure class="chart-card">
  <figcaption>
    <strong>Figure 1.</strong> Illustrative source coverage by field. A field can look present in the UI while still being incomplete in the export.
  </figcaption>
  <div class="bar-chart" role="img" aria-label="Illustrative source coverage by field">
    <div class="bar-row">
      <span class="bar-label">Active census</span>
      <span class="bar-track"><span class="bar-fill teal" style="--value: 96%;"></span></span>
      <span class="bar-value">96%</span>
    </div>
    <div class="bar-row">
      <span class="bar-label">Plan status</span>
      <span class="bar-track"><span class="bar-fill burgundy" style="--value: 78%;"></span></span>
      <span class="bar-value">78%</span>
    </div>
    <div class="bar-row">
      <span class="bar-label">Payor detail</span>
      <span class="bar-track"><span class="bar-fill orange" style="--value: 63%;"></span></span>
      <span class="bar-value">63%</span>
    </div>
    <div class="bar-row">
      <span class="bar-label">Counselor assignment</span>
      <span class="bar-track"><span class="bar-fill purple" style="--value: 41%;"></span></span>
      <span class="bar-value">41%</span>
    </div>
  </div>
</figure>

## What changed

The important move is to separate supported metrics from tempting metrics. If the field is incomplete, it should not become a headline KPI. It can be used as a caveat, a quality issue, or a prompt for source repair.

<table class="evidence-table">
  <thead>
    <tr>
      <th>Metric</th>
      <th>Use</th>
      <th>Reason</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Census</td>
      <td><span class="status-chip good">Headline</span></td>
      <td>High source coverage and stable operational meaning.</td>
    </tr>
    <tr>
      <td>Payor mix</td>
      <td><span class="status-chip watch">Secondary</span></td>
      <td>Useful, but plan labels require interpretation.</td>
    </tr>
    <tr>
      <td>Counselor load</td>
      <td><span class="status-chip bad">Do not headline</span></td>
      <td>Partial assignment coverage makes ranking misleading.</td>
    </tr>
  </tbody>
</table>

The post would end with the operational recommendation: what stays on the dashboard, what gets demoted, and what data repair has to happen before the next version.
