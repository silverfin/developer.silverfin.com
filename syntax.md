---
layout: home
---

<h1>Syntax</h1>

The silverfin templating languages uses 3 kinds of tags:

* <a href="#print-tags">Print tags</a>
* <a href="#logic-tags">Logic tags</a>
* <a href="#layout-tags">Layout tags</a>

Each has its own purpose as explained below.

<h3 id="print-tags">Print tags</h3>

<p>Print tags <code class="highlighter-rouge">{% raw %}{{ }}{% endraw %}</code> are used to print variables on the screen.</p>

<div class="topic">

{% capture input %}
  {% raw %}
    <div class="comment">// {% assign variable = 100 %}</div>
    {{ variable }}
  {% endraw %}
{% endcapture %}
{% capture output %}
  100
{% endcapture %}
{% include preview.html %}

</div>

<div class="topic">

<h3 id="logic-tags">Logic tags</h3>

<p>Logic tags <code class="highlighter-rouge">{% raw %}{% %}{% endraw %}</code> are used for logic and control flows.</p>

{% capture input %}
<pre>{% raw %}
{% assign variable = 100 %}

{% if variable > 0 %}
    Hello world
{% else %}
    Bye World
{% endif %}
{% endraw %}</pre>
{% endcapture %}
{% capture output %}
  Hello world
{% endcapture %}
{% include preview.html %}

</div>

<div class="topic">

<h3 id="layout-tags">Layout tags</h3>

<p>The Layout tags <code class="highlighter-rouge">{% raw %}{:: }{% endraw %}</code> and <code class="highlighter-rouge">{% raw %}{:/ }{% endraw %}</code> are used to adjust the layout within silverfin.</p>

{% capture input %}
<pre>{% raw %}
{::infotext}
  Some info about a subject
{:/infotext}
{% endraw %}</pre>
{% endcapture %}
{% capture output %}
  <img src="img/infotext.png" />
{% endcapture %}
{% include preview.html %}

</div>
