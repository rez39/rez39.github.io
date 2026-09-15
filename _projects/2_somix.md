---
layout: page
title: SoMix
description: An autodyning receiver architecture using tunnel diode oscillators for long-range, low-power reception
img: assets/img/projects/somix_frontend.png
importance: 2
category: research
related_publications: true
---

Low-power transmission has advanced a great deal, but low-power *reception* over similarly useful ranges has lagged behind — most low-power receivers rely on Schottky diode envelope detectors, which are limited in sensitivity and can't support complex modulation. SoMix (Single Oscillator Mixer) uses the autodyning property of tunnel diode oscillators to generate a carrier signal and perform signal downconversion in the same circuit, merging two traditionally power-hungry analog tasks into one energy-efficient step.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/somix_frontend.png" title="SoMix RF front-end" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/somix_demo.png" title="SoMix demo setup" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The SoMix front-end (left) consumes under 100 μW while supporting high-sensitivity reception; the demo setup (right) shows range testing in the field.
</div>

Through injection-locking, SoMix stabilizes its tunnel diode oscillator using even a weak external carrier, receiving FM transmissions from over 100 m in line-of-sight. It outperforms state-of-the-art low-power receivers on power, range, and functionality.

{% cite medaranga2025unraveling %}
