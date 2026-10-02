---
layout: plugin
title: Hold It
permalink: /plugins/hold-it/
plugin: hold-it
description: Freeze a note or chord beneath whatever you play next.
---
{%- assign plugin          = site.data.plugins[page.plugin] -%}
{%- assign marketplace_url = plugin.marketplace_url | strip -%}

<span class="kicker">Plugin for the Darkglass Anagram</span>


# Hold It

<p class="lede"><strong>Freeze effect for infinite sustain.</strong></p>

{% include plugin-tags.html plugin=plugin %}

{% include plugin-art.html plugin=plugin off="/assets/images/hold-it-off.webp" on="/assets/images/hold-it-on.webp" width=400 height=400 alt="Dust &amp; Coil Hold It plugin bypassed—blue control dimmed" %}


*Freeze a note or chord beneath whatever you play next.* 

Hold It gives you infinite sustain for pads, drones, or harmonic beds. It delivers a smooth, natural hold of any bass note or chord played on electric bass, fretless, or upright. We tuned it for both pizzicato and arco, with smooth captures that avoid turning finger noise, bow scratch, or bright transients into an endless buzz.



## Get it

[Available now in the Anagram Marketplace]({{ marketplace_url }}).
