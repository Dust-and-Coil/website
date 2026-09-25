---
layout: default
---

{%- comment -%} A plugin is live iff its marketplace_url is filled in (see _data/plugins.yml). {%- endcomment -%}
{%- assign live_plugins = "" | split: "" -%}
{%- assign soon_plugins = "" | split: "" -%}
{%- for entry in site.data.plugins -%}
  {%- assign url = entry[1].marketplace_url | strip -%}
  {%- if url == "" -%}
    {%- assign soon_plugins = soon_plugins | push: entry[1] -%}
  {%- else -%}
    {%- assign live_plugins = live_plugins | push: entry[1] -%}
  {%- endif -%}
{%- endfor -%}
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
