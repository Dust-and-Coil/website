---
layout: default
title: Big Red Mute Button
permalink: /big-red-mute-button/
description: A free instant-mute plugin for the Darkglass Anagram. One footswitch, click-free silence.
---

<span class="kicker">Plugin for the Darkglass Anagram</span>

# Big Red Mute Button

<p class="lede">One footswitch. Instant, click-free silence. That is the whole
feature.</p>

<span class="tag tag--red">Free</span>
<span class="tag">Anagram</span>
<span class="tag">Mono &amp; stereo</span>
<span class="tag">Open source</span>

<figure class="artpair">
  <div>
    <img src="{{ '/assets/images/brmb-on.png' | relative_url }}" alt="Big Red Mute Button engaged — lit red, muted">
    <figcaption>Engaged — muted</figcaption>
  </div>
  <div>
    <img src="{{ '/assets/images/brmb-off.png' | relative_url }}" alt="Big Red Mute Button bypassed — dimmed, signal live">
    <figcaption>Bypassed — live</figcaption>
  </div>
</figure>

## What it does

Drop it anywhere in a chain and bind it to any footswitch. Stomp: silence. Stomp
again: your signal, untouched.

It is deliberately backwards from every other block on the pedal. A normal effect
does something when you turn it *on*; this one goes quiet when you turn it on, and
gets out of the way when you turn it off. Engaged means muted.

Useful for tuning in silence, swapping instruments mid-set, killing a hum before
you find it, or simply stopping — cleanly, on the beat, without a thump through
the PA.

## What it doesn't do

Nothing. Bypassed, the audio it passes is bit-for-bit identical to what came in.
No tone, no makeup gain, no character. When it isn't muting, it isn't there.

## The one control

**Fade** — 1 to 250 ms, how long the mute takes.

Turned all the way down, it is a hard cut. Turned up, the signal swells in and out
like a volume pedal you don't have to hold. It is also the block's quick-pot, so
the rotary knob over the block adjusts it directly, and a press toggles the mute.

## Why a fade at all

Snapping a signal to zero between one sample and the next is a step
discontinuity — a vertical cliff in the waveform. A cliff like that contains
energy at every frequency, and what you hear is a click or a pop, sometimes loud
enough to be a problem at stage volume. Ramping the level down over a few
milliseconds removes the cliff, and the ear hears nothing but the note ending.

The ramp is a straight line rather than a curve, for a specific reason: a straight
line arrives at its destination exactly, so once the fade completes the output is
exactly zero. The obvious alternative — an exponential glide — only ever
*approaches* zero, and would leave a faint ghost of the signal underneath. Muted
should mean muted.

<div class="panel">
<span class="kicker">Under the hood</span>
Mono in, mono out; the Anagram instances it per channel for stereo chains. No
allocation, no locking, and no file access on the audio thread, so it is safe at
any buffer size. Roughly ten lines of arithmetic do the actual work.
</div>

## Price

Free, and free of any license gate — install it and it runs.

It exists partly because a good mute is genuinely worth having, and partly as an
honest first pass through the whole Anagram vendor pipeline: build, on-device
testing, artwork, metadata, submission, updates. Better to learn that on a plugin
with one knob.

## Availability

Built, installed, and running on real hardware. It is finishing device testing and
the Marketplace submission now — this page will link the download the day it is
listed.

Source is published under the ISC license at
[github.com/{{ site.github_username }}/big-red-button](https://github.com/{{ site.github_username }}/big-red-button).

[Ask to be told when it ships →]({{ '/#get-in-touch' | relative_url }})
