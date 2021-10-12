---
layout: template
title: Basis elementen
url: /html/elementen/basis_elementen
collection: [html, elementen]
---

## Basis elementen

### Een paragraaf
<pre data-enlighter-language="html">
&lt;p&gt;Uw paragraaf hier&lt;/p&gt;
</pre>
Weinig opmaak, enkel een marge boven en onder.

### Een link
<pre data-enlighter-language="html">
&lt;a href=&quot;http://www.syntra-brussel.be&quot;&gt;Ga naar de website van Syntra&lt;/a&gt;
</pre>
Het <code>href</code> attribuut is verplicht.

Wanneer de link in een nieuwe browser tab moet openen gebruik je het target attribuut met de waarde “_blank”.

<pre data-enlighter-language="html">
&lt;a target=&quot;_blank&quot; href=&quot;http://www.syntra-brussel.be&quot;&gt;Ga naar de website van Syntra in een nieuwe tab&lt;/a&gt;
</pre>

### Een titel 

Van belangrijk naar minder belangrijk:
<pre data-enlighter-language="html">
&lt;h1&gt;Grote titel&lt;/h1&gt;
&lt;h2&gt;Kleinere titel&lt;/h2&gt;
&lt;h3&gt;Nog kleinere titel&lt;/h3&gt;
&lt;h4&gt;Nog veel kleinere titel&lt;/h4&gt;
&lt;h5&gt;Nog veel veel kleinere titel&lt;/h5&gt;
</pre>
Weinig opmaak, enkele een verschil in grootte.

<img src="{{ '/html/elementen/images/h1-h5.png' | relative_url}}" />

### Vette tekst
<pre data-enlighter-language="html">
&lt;strong&gt;Een vette tekst&lt;/strong&gt;
</pre>

### Cursieve tekst
<pre data-enlighter-language="html">
&lt;em&gt;Een cursieve tekst&lt;/em&gt;
</pre>

### Een onderlijnde tekst
<pre data-enlighter-language="html">
&lt;u&gt;Een onderlijnde tekst&lt;/u&gt;
</pre>

### Een softe enter
<pre data-enlighter-language="html">
&lt;br /&gt;
</pre>

### Een horizontale lijn
<pre data-enlighter-language="html">
&lt;hr /&gt;
</pre>

### Een beeld
<pre data-enlighter-language="html">
&lt;img src=&quot;logo.jpg&quot; alt=&quot;Alternatieve tekst&quot; width=&quot;100&quot; height=&quot;200&quot; /&gt;
</pre>

De belangrijkste attributen:
<ul>
    <li>
        Het <code>src</code> attribuut bevat de URL naar het beeld
        <ul>
        <li>absoluut pad met domeinnaam: https://www.domeinnaam.be/xxx/afbeelding_naam.jpg</li>
        <li>absoluut pad zonder domeinnaam: /xx/afbeelding_naam.jpg</li>
        <li>relatief pad = pad vanaf html bestand: xxx/afbeelding_naam.jpg</li>
        </ul>
    </li>
    <li>Het <code>alt</code> attribuut bevat de alternatieve tekst die belangrijk is voor de zoekmotor</li>
    <li>Het <code>width</code> attribuut geef de breedte aan dat het beeld moet getoond worden (kan afwijken van de eigenlijke breedte van het beeld)
    Zonder <code>width</code> wordt het beeld op volle breedte getoond.</li>
    <li>Het <code>height</code> attribuut geeft de hoogte aan dat het beeld moet getoond worden (kan afwijken van de eigenlijke hoogte van het beeld)
    Zonder <code>height</code> wordt het beeld op volle breedte getoond.</li>
</ul>

### Ongeordende lijst
<pre data-enlighter-language="html">
&lt;ul&gt; 
  &lt;li&gt;Een item&lt;/li&gt; 
  &lt;li&gt;Nog een item&lt;/li&gt; 
  &lt;li&gt;En nog een item&lt;/li&gt; 
&lt;/ul&gt;
</pre>
De ongeordende lijst heef weinig opmaak, standaard staat voor elk item een “•”.


### Geordende lijst
<pre data-enlighter-language="html">
&lt;ol&gt; 
  &lt;li&gt;Een item&lt;/li&gt; 
  &lt;li&gt;Nog een item&lt;/li&gt; 
  &lt;li&gt;En nog een item&lt;/li&gt; 
&lt;/ol&gt;
</pre>

De geordende lijst heeft weinig opmaak, standaard staat voor elk item een oplopend cijfer.

Het attribuut type heeft volgende mogelijke waardes: “1”, “A”, “a”, “I”, “i”
(numeriek, A-Z, a-z, I-II-III…, i-ii-iii)

### Label
Het label element element wordt het vaakst gebruikt in combinatie met formulier elementen (zie verder in dit hoofdstuk).

<pre data-enlighter-language="html">
&lt;label for=&quot;naam&quot;&gt;Naam&lt;/label&gt;
&lt;input type=&quot;text&quot; id=&quot;naam&quot; /&gt;
</pre>

Het <code>for</code> attribuut geeft aan bij welk element het label hoort. Je zal zien dat in dit geval het tekstveld de focus krijgt als je er op klikt.

In het voorbeeld hierboven hoort het label dus bij het tekstveld met het <code>id</code> attribuut met als waarde "naam”.