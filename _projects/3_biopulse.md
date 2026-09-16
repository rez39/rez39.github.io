---
layout: page
title: BioPulse
description: A battery-free, perpetual vital-signs monitoring patch (internship project, Nokia Bell Labs)
img: assets/img/projects/biopulse_patch.png
importance: 5
category: research
related_publications: true
---

Wearables like smartwatches, earbuds, and rings are becoming central to health monitoring, but battery life limits long-term use, and many older adults — who stand to benefit most — face barriers to using digital devices at all. BioPulse is a perpetual, patch form-factor device built to address both: it estimates heart rate, heart rate variability, and blood pressure using a sparse sampling algorithm combined with NFC-based energy transfer and communication, operating entirely without a battery.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/biopulse_patch.png" title="BioPulse patch" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/biopulse_arch.png" title="BioPulse architecture" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The BioPulse patch (left) and its sparse-sampling, NFC-powered architecture (right), which cuts power consumption by 57.9%.
</div>

In evaluation against a ground-truth device, BioPulse achieves a mean absolute error of 5.6 mmHg for systolic and 4.5 mmHg for diastolic blood pressure — a sustainable, accessible approach to continuous vital-signs monitoring. Built during an internship with the Pervasive Systems group at Nokia Bell Labs, Cambridge.

{% cite reddy2025biopulse %}
