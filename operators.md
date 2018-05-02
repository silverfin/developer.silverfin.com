---
layout: home
---

<h1>Operators</h1>

Operators are used to compare data

* <a href="#equals">==</a>
* <a href="#difference">!=</a>
* <a href="#greater">&gt;</a>
* <a href="#lower">&lt;</a>
* <a href="#great-equals">&gt;=</a>
* <a href="#lower-equals">&lt;=</a>
* <a href="#or">or</a>
* <a href="#and">and</a>
* <a href="#contains">contains</a>

* <a href="#blank">blank</a>
* <a href="#empty">empty</a>

<h3 id="equals">==</h3>

<p>The "equals to" operator compares data to see if they are equal.</p>

<div class="topic">

{% capture input %}
{% raw %}
<div class="comment">// {% assign variable1 = 100 %}</div>
<div class="comment">// {% assign variable2 = 100 %}</div>
<br />
<pre>
{% if variabele1 == variabele2 %}
  Deze variabelen zijn gelijk aan elkaar
{% else %}
  Deze variabelen zijn verschillend van elkaar
{% endif %}
</pre>
{% endraw %}
{% endcapture %}

{% capture output %}
{% assign variable1 = 100 %}
{% assign variable2 = 100 %}

{% if variabele1 == variabele2 %}
  Deze variabelen zijn gelijk aan elkaar
{% else %}
  Deze variabelen zijn verschillend van elkaar
{% endif %}
{% endcapture %}

{% include preview.html %}
