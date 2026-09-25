---
layout: default
title: Hold It
permalink: /plugins/hold-it/
plugin: hold-it
description: A coming-soon plugin for the Darkglass Anagram. When the note should keep going and the instrument has other plans.
---
{%- assign plugin = site.data.plugins[page.plugin] -%}
{%- assign marketplace_url = plugin.marketplace_url | strip -%}

<span class="kicker">Plugin for the Darkglass Anagram</span>


# Hold It

<p class="lede"><strong>Natural decay has been identified as incompatible with project requirements.</strong></p>

{% include plugin-tags.html plugin=plugin %}

{% include plugin-art.html plugin=plugin off="/assets/images/hold-it-off.webp" on="/assets/images/hold-it-on.webp" width=364 height=427 alt="Dust &amp; Coil Hold It plugin bypassed—blue control dimmed" %}


## Why this exists

Bass notes end. That is usually correct. Sometimes it is not.

The workarounds are familiar: ride the volume pedal, ride the compressor, re-attack the string and pretend it is the same note, or accept a gap where the arrangement wanted a line. None of those is difficult. That was never the point.

Hold It is for the moment when the note should keep going and the instrument has other plans.


{% if marketplace_url != "" %}
{% comment %}
  TODO(launch): add a "## The controls" section here, like the BRMB page's
  "The one control". Copy to come from the plugin team — not rendered until written.
{% endcomment %}

## Price

{% include plugin-price.html plugin=plugin %}

{% include plugin-price.html plugin=plugin part="note" %}

## Get it

[Available now in the Anagram Marketplace]({{ marketplace_url }}). Add it to your
library and install it on the pedal.

{% else %}
## Status

Coming soon. Controls, pricing, and the Anagram Marketplace listing will land here when the plugin does.


## Meanwhile

Ideas, bug reports from the field, and “please make it do X” notes are welcome on the
[contact page]({{ '/contact/' | relative_url }}).

{% endif %}
