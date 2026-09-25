---
layout: default
title: Contact
permalink: /contact/
description: Get in touch with Dust & Coil. Ideas, bug reports, and questions about our Darkglass Anagram plugins.
# Linked from the footer; keep out of the header nav.
nav_exclude: true
---

<span class="kicker">Ideas · bug reports · questions</span>


# Get in touch

Big Red Mute Button began with Anagram owners saying they wanted a dedicated
mute. We are listening. If there is a small problem in your signal chain that
everyone else has told you to work around, we would especially like to hear
about it.

<form class="form" action="https://formspree.io/f/{{ site.formspree_id }}" method="POST">
  <input type="hidden" name="_next" value="{{ '/thanks/' | absolute_url }}">
  <label for="name">Name</label>
  <input id="name" type="text" name="name" required>

  <label for="email">Email</label>
  <input id="email" type="email" name="email" required>

  <label for="message">Message</label>
  <textarea id="message" name="message" rows="6" required></textarea>

  <button type="submit">Send</button>
</form>
