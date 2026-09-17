---
layout: page
title: AudioCast
description: Ubiquitous connectivity for embedded systems via FM audio-broadcasting, beyond-backscatter tags
img: assets/img/projects/audiocast_system.png
importance: 1
category: research
related_publications: true
---

AudioCast rethinks radio transmitter design to solve two problems at once: spectrum contention and the high power cost of transmission. It uses a tunnel diode oscillator to generate a carrier signal and self-modulate it with a baseband signal directly, producing frequency-modulated transmissions at under 200 μW — without an externally generated or ambient carrier, unlike backscatter systems. We call this a **Beyond-Backscatter** transmitter.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/audiocast_system.png" title="AudioCast system overview" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/audiocast_comparison.png" title="AudioCast comparison" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    AudioCast's transmitter architecture (left) and comparison against related low-power transmission approaches (right).
</div>

The transmissions are decodable by ordinary commodity FM receivers already deployed everywhere — cars, phones, home radios — reaching up to 130 m line-of-sight. Full details, evaluation, and applications (including low-power voice and gesture communication) are in the paper below {% cite reddy2025audiocast %}.
