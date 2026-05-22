---
layout: archive
title: "Moving Lens Effect"
permalink: /movinglenseffect/
author_profile: true
use_math: true
---

{% include base_path %}

<div class="hero-section hero-section--page-intro">
  <p class="hero-eyebrow"><a href="https://arxiv.org/abs/2605.18938">arXiv:2605.18938 (2026)</a></p>
  <p class="hero-tagline">A purely gravitational signature of cosmic transverse motion.</p>
  <p class="hero-position">First measurement, at signal-to-noise <span class="placeholder-inline">[S/N]</span> from <span class="placeholder-inline">[CMB experiment]</span> &times; <span class="placeholder-inline">[galaxy survey]</span>.</p>
</div>

<div class="figure-placeholder">
  <div class="figure-placeholder__label">Hero figure</div>
  <div class="figure-placeholder__detail">Result plot from arXiv:2605.18938 to be inserted here.<br>Suggested filename: <code>/images/movinglens_detection.png</code> (.img-wide class)</div>
</div>
<p class="research-block__caption">Caption to be added: one-sentence statement of the headline result.</p>

<div class="research-nav">
  <a href="#physics">The Physics</a>
  <a href="#detection">The Detection</a>
  <a href="#watch">Watch</a>
  <a href="#lineage">Lineage</a>
  <a href="#resources">Resources</a>
</div>


<div id="physics" class="research-section research-section--flush" markdown="1">

## What is the moving lens effect?

<p class="research-intro">As a massive structure moves transverse to our line of sight, its gravitational potential drags CMB photons across the sky, producing a small-scale dipolar temperature pattern aligned with the motion. Unlike the kinetic Sunyaev-Zel'dovich effect — which depends on bulk gas motion and ionization — the moving-lens signal is purely gravitational, making it a clean probe of the transverse velocity field and the growth rate of structure.</p>

The induced temperature contrast is small — of order $10^{-9}$ at the location of a typical massive halo — but its dipolar geometry, set by the direction of transverse motion, is highly distinctive. A matched filter stacked across many objects recovers it above the larger but unstructured background of primary CMB fluctuations. Two ingredients are essential: high-resolution CMB maps, and an accurate estimate of the transverse velocity field reconstructed from galaxy positions.

Because the effect arises from photon deflection rather than scattering, it carries no astrophysical bias from gas thermodynamics or feedback. This makes it complementary to the kSZ effect, which depends on the radial gas-weighted velocity. Together, they access orthogonal components of the same large-scale velocity field.

</div>


<div id="detection" class="research-section" markdown="1">

## The detection

<p class="research-intro">In <a href="https://arxiv.org/abs/2605.18938">Hotinli et al. (2605.18938)</a>, we report the first measurement of the moving-lens effect, applying an optimal matched-filter estimator to <span class="placeholder-inline">[CMB experiment]</span> temperature maps cross-correlated with the transverse-velocity field reconstructed from <span class="placeholder-inline">[galaxy survey]</span>.</p>

<span class="placeholder-inline">[Methodology paragraph — to be filled in: pipeline, transverse-velocity reconstruction, filter design, null-test framework, foreground handling.]</span>

<div class="figure-placeholder">
  <div class="figure-placeholder__label">Result figure</div>
  <div class="figure-placeholder__detail">Measured stacked signal vs. LCDM prediction, from arXiv:2605.18938.</div>
</div>
<p class="research-block__caption">Placeholder for result figure caption.</p>

The measurement is consistent with the LCDM expectation at the <span class="placeholder-inline">[X]</span>% level and provides a direct, gas-independent handle on the cosmic transverse-velocity field. Combined with kSZ-based reconstructions of the radial component, the moving lens provides a route to mapping the full three-dimensional velocity field from CMB observations.

</div>


<div id="watch" class="research-section" markdown="1">

## Watch

<p class="research-intro">A short visual summary of the result.</p>

<div class="video-responsive">
<iframe src="https://www.youtube.com/embed/QiViSKMSv2A" title="Moving lens effect — first detection" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>

</div>


<div id="lineage" class="research-section" markdown="1">

## Lineage

<p class="research-intro">From prediction to detection — a nine-year arc.</p>

<div class="cv-entry">
  <div class="cv-entry__date">2017</div>
  <div class="cv-entry__content">
    <strong>Prediction and detection method</strong><br>
    <a href="https://arxiv.org/abs/1710.08913">Hotinli et al. (1710.08913)</a>
    <span class="cv-entry__detail">Derived the dipolar temperature pattern induced by transverse halo motion and proposed matched-filter estimators for future CMB experiments.</span>
  </div>
</div>

<div class="cv-entry">
  <div class="cv-entry__date">2020</div>
  <div class="cv-entry__content">
    <strong>Optimal estimator and forecasts</strong><br>
    <a href="https://arxiv.org/abs/2006.03060">Hotinli, Johnson &amp; Meyers (2006.03060)</a>
    <span class="cv-entry__detail">Constructed the optimal quadratic estimator combining CMB temperature maps with galaxy positions, forecasting signal-to-noise ~20 for next-generation CMB experiments combined with the Rubin Observatory.</span>
  </div>
</div>

<div class="cv-entry cv-entry--current">
  <div class="cv-entry__date">2026</div>
  <div class="cv-entry__content">
    <strong>First detection</strong><br>
    <a href="https://arxiv.org/abs/2605.18938">Hotinli et al. (2605.18938)</a>
    <span class="cv-entry__detail">First measurement of the moving-lens effect, using <span class="placeholder-inline">[experiment × survey]</span>.</span>
  </div>
</div>

</div>


<div id="resources" class="research-section" markdown="1">

## Resources

- <a href="https://arxiv.org/abs/2605.18938">arXiv:2605.18938</a> — main paper (2026)
- <a href="https://arxiv.org/abs/2006.03060">arXiv:2006.03060</a> — optimal estimator and forecasts (2020)
- <a href="https://arxiv.org/abs/1710.08913">arXiv:1710.08913</a> — original prediction (2017)
- <a href="https://www.youtube.com/watch?v=QiViSKMSv2A">Video summary</a> — YouTube
- <a href="/research/#beyond-ksz">Context</a> — Beyond kSZ section on the Research page

</div>
