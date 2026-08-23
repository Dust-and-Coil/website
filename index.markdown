---
layout: default
---

<span class="kicker">Dust &amp; Coil Audio Laboratories · Colorado</span>

# Useful effects. Unnecessary amounts of research.

<p class="lede">Dust &amp; Coil makes plugins for the
<a href="https://www.darkglass.com/products/anagram">Darkglass Anagram</a>. We build
small, opinionated tools for bass players—usually because somebody has noticed a
problem, and the existing answer is some variation of “just work around it.”</p>

We are a three-person joint venture: a double-bass luthier, a professional jazz
bassist, and me—a career software engineer who also plays bass. I am the sole
developer. After decades of ordinary software, audio DSP is the newer part. So I
began with a controlled experiment: Could I make an effect that reliably produces
no sound at all?

The results have been encouraging.

---

## Available now

<a class="feature" href="{{ '/big-red-mute-button/' | relative_url }}">
  <span class="state-swap">
    <img class="state-swap__off" src="{{ '/assets/images/brmb-off.png' | relative_url }}" alt="Big Red Mute Button bypassed—dimmed with signal live">
    <img class="state-swap__on" src="{{ '/assets/images/brmb-on.png' | relative_url }}" alt="" aria-hidden="true">
  </span>
  <span class="feature__copy">
    <span class="kicker">Free · Anagram</span>
    <strong>Big Red Mute Button</strong>
    <span>Press the big red button: your signal mutes. Press it again: your signal returns.</span>
    <span class="feature__more">Inspect the research →</span>
  </span>
</a>

---

## Currently under investigation

<div class="feature feature--static">
  <span class="state-swap">
    <img class="state-swap__off" src="{{ '/assets/images/hold-it-off.webp' | relative_url }}" alt="Dust & Coil Hold It plugin bypassed—blue control dimmed">
    <img class="state-swap__on" src="{{ '/assets/images/hold-it-on.webp' | relative_url }}" alt="" aria-hidden="true">
  </span>
  <span class="feature__copy">
    <span class="kicker">Coming soon</span>
    <strong>Hold It</strong>
    <span>Natural decay has been identified as incompatible with project requirements.</span>
  </span>
</div>

---

## Get in touch

<span class="kicker">Ideas · bug reports · questions</span>

Big Red Mute Button began with Anagram owners saying they wanted a dedicated
mute. We are listening. If there is a small problem in your signal chain that
everyone else has told you to work around, we would especially like to hear
about it.

<form class="form" action="https://formspree.io/f/{{ site.formspree_id }}" method="POST">
  <label for="name">Name</label>
  <input id="name" type="text" name="name" required>

  <label for="email">Email</label>
  <input id="email" type="email" name="email" required>

  <label for="message">Message</label>
  <textarea id="message" name="message" rows="6" required></textarea>

  <button type="submit">Send</button>
</form>

<p style="margin-top: 1rem">
  Or email <a href="mailto:{{ site.email }}">{{ site.email }}</a> directly.
</p>
