---
layout: page
title: TunnelSense
description: Low-power, non-contact sensing using tunnel diode oscillators
img: assets/img/projects/tunnelsense_setup.png
importance: 4
category: research
related_publications: true
---

Many sensing scenarios — tracking occupancy, monitoring vital signs, diagnosing machine faults — need to observe motion without touching the object at all. TunnelSense rethinks non-contact sensing using tunnel diode oscillators, which are highly sensitive to changes in their surrounding electromagnetic environment: an object moving nearby shifts the oscillator's resonant frequency, and therefore the radio waves it generates.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/tunnelsense_setup.png" title="TunnelSense setup" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/tunnelsense_sensor.png" title="TunnelSense sensor" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The TunnelSense receiver and reference device setup (left) and sensor tag (right).
</div>

Tags built on this principle run on under 100 μW with a bias voltage starting at just 70 mV, enabling long operation on a small battery or harvested energy. In this work we demonstrate breathing detection at distances up to 30 cm between subject and tag.

{% cite thaddeus2024tunnelsense %}
