---
layout: default
title: Big Red Mute Button
permalink: /big-red-mute-button/
plugin: big-red-mute-button
description: A free dedicated-mute plugin for the Darkglass Anagram. Adjustable fade in and out.
---
{%- assign plugin = site.data.plugins[page.plugin] -%}

<span class="kicker">Plugin for the Darkglass Anagram</span>


# Big Red Mute Button

<p class="lede"><strong>Audiophile-approved nothingness</strong></p>

{% include plugin-tags.html plugin=plugin %}

{% include plugin-art.html plugin=plugin off="/assets/images/brmb-off.webp" on="/assets/images/brmb-on.webp" width=364 height=364 alt="Big Red Mute Button bypassed—dimmed with signal live" %}


## Why this exists

Several people in the Anagram Facebook group said they wished it had a mute. 
Strictly speaking, it does: long-press the left footswitch to open the tuner, 
which mutes by default.

That answers the literal feature request while missing the UX problem. The same
footswitch normally controls something else in the preset. A long press is a
different interaction from a stomp. And on stage, “enter another mode which also
happens to mute” is not equivalent to “stop my signal now.”

Some of those users were told that triggering the tuner is not difficult. It
isn't. That was never the point.


## The one control

**Fade** sets the transition time, from an immediate cutoff to a smooth fade out
and back in. 


## Price

{% include plugin-price.html plugin=plugin %}.


## Get it

[Available now in the Utilities section]({{ plugin.marketplace_url }}) of the Anagram Marketplace. Add it to your
library and install it on the pedal.
