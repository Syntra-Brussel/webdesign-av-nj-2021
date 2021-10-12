---
layout: template
title: Tabel element
url: /html/elementen/tabel_element
collection: [html, elementen]
---

## Tabel element

<img src="{{ '/html/elementen/images/tabel_html.png' | relative_url}}" />

Om inhoud in een tabel weer te geven gebruiken we het <span style="color: red"><code>&lt;table&gt;</code></span> element.

De inhoud die op eenzelfde lijn wordt weergeven wordt opgenomen binnen een <span style="color: blue"><code>&lt;tr&gt;</code></span> element.

Elke kolom binnen een rij wordt weergeven met een <span style="color: green"><code>&lt;td&gt;</code></span> element.

### Tabel hoofding
Als de eerste rij binnen het <code>&lt;table&gt;</code> element de hoofding is vervangen we de <code>&lt;td&gt;</code> door <code>&lt;th&gt;</code>.

<pre data-enlighter-language="html">
&lt;table border=&quot;1&quot; width=&quot;100%&quot;&gt;
  &lt;tr&gt;
    &lt;th&gt;kolom 1&lt;/th&gt; 
    &lt;th&gt;kolom 2&lt;/th&gt; 
    &lt;th&gt;kolom 3&lt;/th&gt; 
  &lt;/tr&gt; 
  &lt;tr&gt;
    &lt;td&gt;cel 1.1&lt;/td&gt; 
    &lt;td&gt;cel 1.2&lt;/td&gt; 
    &lt;td&gt;cel 1.3&lt;/td&gt; 
  &lt;/tr&gt; 
  &lt;tr&gt; 
    &lt;td&gt;Cel 2.1&lt;/td&gt;
    &lt;td&gt;cel 2.2&lt;/td&gt;
    &lt;td&gt;cel 2.3&lt;/td&gt;
  &lt;/tr&gt; 
  &lt;tr&gt; 
    &lt;td&gt;Cel 3.1&lt;/td&gt;
    &lt;td&gt;cel 3.2&lt;/td&gt;
    &lt;td&gt;cel 3.3&lt;/td&gt;
  &lt;/tr&gt; 
&lt;/table&gt;
</pre>

### Kolommen samenvoegen
Je kan ook meerdere kolommen samenvoegen via het attribuut colspan:


<pre data-enlighter-language="html">
&lt;table widh=&quot;100%&quot; border=&quot;1&quot;&gt; 
  &lt;tr&gt; 
    &lt;th&gt;Naam&lt;/th&gt; 
    &lt;th colspan=&quot;2&quot;&gt;Telefoon&lt;/th&gt; 
  &lt;/tr&gt; 
  &lt;tr&gt; 
    &lt;td&gt;Bert Jansen&lt;/td&gt; 
    &lt;td&gt;03/123.12.34&lt;/td&gt; 
    &lt;td&gt;0475/01.23.45&lt;/td&gt; 
  &lt;/tr&gt; 
&lt;/table&gt;
</pre>

<img src="{{ '/html/elementen/images/colspan.png' | relative_url}}" />

### Rijen samenvoegen
Je kan ook meerdere rijen samenvoegen via het attribuut rowspan:

<pre data-enlighter-language="html">
&lt;table width=&quot;100%&quot;&gt;
  &lt;tr&gt; 
    &lt;th&gt;Naam:&lt;/th&gt; 
    &lt;td&gt;Bert Jansen&lt;/td&gt; 
  &lt;/tr&gt; 
  &lt;tr&gt; 
    &lt;th rowspan=&quot;2&quot;&gt;Telefoon:&lt;/th&gt; 
    &lt;td&gt;03/123.12.34&lt;/td&gt; 
  &lt;/tr&gt; 
  &lt;tr&gt; 
    &lt;td&gt;0475/01.23.45&lt;/td&gt;
  &lt;/tr&gt; 
&lt;/table&gt;
</pre>

<img src="{{ '/html/elementen/images/rowspan.png' | relative_url}}" />