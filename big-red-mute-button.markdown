---
layout: default
title: Big Red Mute Button
permalink: /big-red-mute-button/
description: A free dedicated-mute plugin for the Darkglass Anagram. Press once for silence. Press again for signal.
---

<span class="kicker">Plugin for the Darkglass Anagram</span>

# Big Red Mute Button

<p class="lede"><strong>STOP YOUR SOUND. NOW.</strong></p>

<span class="tag tag--red">Free</span>
<span class="tag">Anagram</span>
<span class="tag">Mono &amp; stereo</span>

<figure class="product-state">
  <span class="state-swap">
    <img class="state-swap__off" src="{{ '/assets/images/brmb-off.png' | relative_url }}" alt="Big Red Mute Button bypassed—dimmed with signal live">
    <img class="state-swap__on" src="{{ '/assets/images/brmb-on.png' | relative_url }}" alt="" aria-hidden="true">
  </span>
  <figcaption>Hover to engage</figcaption>
</figure>

Big Red Mute Button gives Anagram an immediate, dedicated mute. Assign it to the
control you already use: a stomp footswitch, MIDI controller, or anything else
available.

No long press. No hidden gesture performed correctly under stage lighting while
everyone waits.

Press the big red button: your signal mutes. Press it again: your signal returns.

## Why it exists

I got the idea by listening to Anagram owners. Several people in the Facebook
group said they wished the pedal had a mute. Strictly speaking, it does: long-press
a footswitch to open the tuner, which mutes by default.

That answers the literal feature request while missing the UX problem. The same
footswitch normally controls something else in the preset. A long press is a
different interaction from a stomp. And on stage, “enter another mode which also
happens to mute” is not equivalent to “stop my signal now.”

Some of those users were told that triggering the tuner is not difficult. It
isn't. That was never the point.

## The one control

**Fade** sets the transition time, from an immediate cutoff to a smooth fade out
and back in. At longer settings, the mute behaves more like an automatic volume
pedal. Fade is also the block's quick-pot: turn the encoder to adjust it, or press
the encoder to toggle the mute.

Why fade at all? Because changing a nonzero digital sample directly to zero
creates a step discontinuity—the kind of mathematically correct event that a PA
helpfully renders as a click. Big Red Mute Button ramps to zero over the selected
time, then stays at exactly zero.

Muted is a binary specification.

<div class="panel panel--red">
<span class="kicker">Silence, re-engineered</span>
At Dust &amp; Coil Audio Laboratories, we refuse to treat silence as the mere absence
of sound.

Big Red Mute Button features our proprietary Vacuum Tube Silence™ technology,
producing a warm nothingness suitable for stage or studio. Every mute is digitally
hand-calibrated to deliver zero-latency silence and audiophile-approved nothingness.

Independent testing confirms that when Big Red Mute Button is engaged, it is
extremely difficult to hear.
</div>

## What it does to your tone

Nothing. Bypassed audio is bit-for-bit identical to the input. No gain, EQ,
compression, saturation, warmth, air, punch, heft, sparkle, or other substance
normally sold by the ounce.

The DSP itself is mono; Anagram creates one instance per channel in a stereo
chain. The audio thread performs no allocation, locking, or file access. Roughly
ten lines of arithmetic do the actual work. The rest is research.

## A first experiment

I have decades of software-engineering experience, but I am new to audio DSP.
Big Red Mute Button was the ideal first plugin: genuinely useful, narrowly scoped,
and just complicated enough to exercise the entire Anagram vendor pipeline—DSP,
controls, artwork, metadata, on-device testing, packaging, submission, and
updates.

Better to learn those things on a plugin with one knob than on a physical model
of an upright bass.

<figure class="lab-photo">
  <img src="{{ '/assets/images/mute-laboratory.webp' | relative_url }}" alt="Big Red Mute Button under development on the Dust & Coil laboratory bench">
  <figcaption>Development apparatus. Coffee not pictured due to operational requirements.</figcaption>
</figure>

## Price

Free. No license key, account, activation, or trial period.

## Get it

Available now in the Utilities section of the Anagram Marketplace. Add it to your
library and install it on the pedal.

[Big Red Mute Button on the Anagram Marketplace →](https://marketplace.anagram.shop/learn-more?id=gid://shopify/Product/16160722026874)
