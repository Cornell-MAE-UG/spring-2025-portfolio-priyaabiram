---
layout: default
title: "Engineering Ethics Case Study: Boeing 737 MAX"
image: /assets/images/ethics-system-map.svg
summary: Ethics case study dissecting MCAS design choices, incentive structures, and preventable safeguards.
---

<section class="project-hero">
  <p class="text-muted mb-2">MAE 4300 · Ethics Portfolio</p>
  <h2>Ethical Review of the Boeing 737 MAX Program</h2>
  <p class="lead">Systems-level analysis of how engineering decisions, incentives, and regulatory gaps culminated in two preventable crashes.</p>
  <div class="metrics-grid">
    <div class="metric-card">
      <span>Flights Lost</span>
      <strong>2</strong>
    </div>
    <div class="metric-card">
      <span>Lives Lost</span>
      <strong>346</strong>
    </div>
    <div class="metric-card">
      <span>Primary Failure</span>
      <strong>MCAS</strong>
    </div>
    <div class="metric-card">
      <span>Key Standard</span>
      <strong>ASME Canon 1</strong>
    </div>
  </div>
</section>

### What Happened
The 737 MAX program introduced the Maneuvering Characteristics Augmentation System (MCAS) to offset pitch-up tendencies caused by larger engines. MCAS was granted authority to push the nose down using input from a single angle-of-attack (AoA) sensor. Both Lion Air Flight 610 (2018) and Ethiopian Airlines Flight 302 (2019) experienced erroneous AoA data, repeated MCAS activations, and catastrophic dives that pilots could not diagnose because MCAS was undocumented in the flight manual.

These events exposed deeper systemic failures: Boeing’s push to minimize pilot retraining, aggressive production schedules driven by competition with Airbus, and an FAA delegation structure that limited independent scrutiny. The result was a safety-critical system shipped with a single point of failure, limited authority boundaries, and minimal pilot awareness.

### Design and Organizational Drivers
- **Technical gaps:** Single-sensor dependency, unlimited MCAS authority compared with earlier 737 logic, and no immediate pilot annunciation violated core redundancy guidelines for flight-critical software.
- **Organizational pressure:** Management prioritized certification speed and marketing claims (“no simulator time required”), filtering and deferring safety concerns raised by engineers.
- **Regulatory capture:** The Organization Designation Authorization (ODA) process left crucial MCAS reviews in Boeing’s hands, diluting the FAA’s ability to challenge hazardous assumptions.

### Ethical Issues
Applying ASME Canon 1 (public welfare first) and Canon 3 (issue public statements only in an objective manner), the MAX case shows how incentives can override professional duties:
- Approving MCAS with known single-point failures contradicted the obligation to prioritize life over cost and schedule.
- Withholding MCAS documentation from pilots and monetizing optional safety alerts undermined transparency and informed decision-making.
- Continuing operations after the first crash ignored conservative safety precedent and risked additional lives—an ethical breach at both corporate and regulatory levels.

### How It Could Have Been Prevented
1. **Design discipline:** Enforce redundant sensor validation, limited MCAS authority, and explicit cockpit annunciations before certification.
2. **Training honesty:** Provide simulator scenarios and manual documentation describing MCAS behavior; empower pilots to override automation confidently.
3. **Regulatory independence:** Require third-party review for single-point safety systems and remove commercial incentives from certification schedules.
4. **Post-incident humility:** Ground the fleet after Lion Air 610 while investigations matured; a precautionary stand-down would likely have prevented the second crash.

### Quick Takeaways
This case illustrates that ethics is not a postscript to engineering—it is embedded in every trade-off between time, money, and human life. I learned to:
- Question “business-as-usual” pressure when safety margins shrink.
- Elevate concerns even when organizational incentives discourage escalation.
- Treat transparency as a design requirement: if pilots, operators, or the public cannot understand a system, it is not truly safe.

### Full Essay & Reference
- [Read the full Ethics Analysis (PDF)]({{ '/assets/ethics/Ethics_737_MAX_Essay.pdf' | relative_url }})
- GitHub Pages permalink: `{{ page.url | absolute_url }}`
