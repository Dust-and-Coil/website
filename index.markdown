---
layout: default
---

{%- assign live_plugins = site.data.plugins | where: "status", "live" -%}
{%- assign soon_plugins = site.data.plugins | where: "status", "coming-soon" -%}
<div class="feature-row{% if live_plugins.size == 0 or soon_plugins.size == 0 %} feature-row--single{% endif %}">
{%- if live_plugins.size > 0 %}
  <div class="feature-row__col">
    <p class="section-label">Available now</p>
    <div class="feature-list">
    {%- for plugin in live_plugins %}
    {% include plugin-card.html plugin=plugin %}
    {%- endfor %}
    </div>
  </div>
{%- endif %}
{%- if soon_plugins.size > 0 %}

  <div class="feature-row__col">
    <p class="section-label">Coming soon</p>
    <div class="feature-list">
    {%- for plugin in soon_plugins %}
    {% include plugin-card.html plugin=plugin %}
    {%- endfor %}
    </div>
  </div>
{%- endif %}
</div>


<p class="lede">Dust &amp; Coil makes plugins for the
<a href="https://www.darkglass.com/products/anagram">Darkglass Anagram</a>. We build
small, opinionated tools for bass players—usually because somebody has noticed a
problem, and the existing answer is some variation of “just work around it.”</p>

We are a three-person joint venture: a double-bass luthier, a professional jazz
bassist, a career software engineer who also plays bass. 


---

<p class="section-label">On Instagram</p>

{% include instagram-embed.html %}

---

## Get in touch

<span class="kicker">Ideas · bug reports · questions</span>

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
