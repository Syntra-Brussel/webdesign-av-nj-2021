---
layout: template
title: Attributen
url: /html/elementen/formulier_elementen
collection: [html, elementen]
---

## Formulier elementen

Een hoeksteen van webpagina’s zijn formulieren. Ze bestaan al sinds het begin maar sinds de introductie van HTML5 zijn de mogelijkheden grondig uitgebreid.

Formulier elementen worden samen gezet in een <code style="color: blue">&lt;form&gt;</code> element.

Het <code style="color: blue">&lt;form&gt;</code> element heeft enkele belangrijke attributen:

<code style="color: green"><u>action</u></code>: de URL naar waar het formulier gestuurd moet worden voor verwerking

<code style="color: green"><u>method</u></code>: GET (de inhoud van de velden wordt via de URL mee gestuurd), POST (de inhoud van de velden wordt onzichtbaar verstuurd)
Voor de introductie van HTML5 waren er al heel wat formulier elementen.

Alle invoer velden moeten binnen <code style="color: blue">&lt;form&gt;</code> en <code style="color: blue">&lt;/form&gt;</code> staan.

<img src="{{ '/html/elementen/images/form_html.png' | relative_url}}" />

### Elementen die sinds HTML5 bestaan
Er zijn tal van nieuwe elementen geïntroduceerd die veel meer frontend validatie mogelijk maken.

<pre data-enlighter-language="html">
&lt;input type=&quot;email&quot; required placeholder=&quot;Voer een e-mailadres in&quot; /&gt;
</pre>

Het required attribuut zorgt voor een frontend validatie op een geldig e-mail adres formaat voor het formulier wordt verstuurd.

Naast het type email, zijn ook volgende types geïntroduceerd:

<ul>
<li>color</li>
<li>date</li>
<li>datetime</li>
<li>datetime-local</li>
<li>email</li>
<li>month</li>
<li>number</li>
<li>range</li>
<li>search</li>
<li>tel</li>
<li>time</li>
<li>url</li>
<li>week</li>
</ul>

### Elementen die al voor HTML5 bestonden
#### Een tekstveld
<pre data-enlighter-language="html">
&lt;input name=&quot;voornam&quot; type=&quot;text&quot;&gt;
</pre>
Het <code>name</code> attribuut is verplicht bij een <code>&lt;input&gt;</code> element

#### De selectielijst
<pre data-enlighter-language="html">
&lt;select name=&quot;auto&quot;&gt; 
  &lt;option value=&quot;volvo&quot;&gt;Volvo&lt;/option&gt; 
  &lt;option selected value=&quot;saab&quot;&gt;Saab&lt;/option&gt; 
  &lt;option value=&quot;fiat&quot;&gt;Fiat&lt;/option&gt; 
  &lt;option value=&quot;audi&quot;&gt;Audi&lt;/option&gt; 
&lt;/select&gt;
</pre>

<ul>
<li>Waneer meer dan 1 optie geselecteerd mag worden krijgt het <code>&lt;select&gt;</code> element een attribuut <code>multiple</code>.</li>
<li>De optie die geselecteerd wordt krijgt het attribuut <code>selected</code>.</li>
<li>Een <code>name</code> attribuut is verplicht bij een <code>&lt;select&gt;</code> element.</li>
</ul>

#### Selectie rondje (radio)
Er is maar één keuze mogelijk.

<pre data-enlighter-language="html">
&lt;input type=&quot;radio&quot; id=&quot;optie_1&quot; name=&quot;optie&quot; value=&quot;Optie 1&quot;&gt; 
&lt;label for=&quot;optie_1&quot;&gt;Dit is optie 1&lt;/label&gt;&lt;br /&gt; 
&lt;input type=&quot;radio&quot; id=&quot;optie_2&quot; name=&quot;optie&quot; value=&quot;Optie 2&quot;&gt; 
&lt;label for=&quot;optie_2&quot;&gt;Dit is optie 2&lt;/label&gt;&lt;br /&gt; 
&lt;input type=&quot;radio&quot; id=&quot;optie_3&quot; name=&quot;optie&quot; value=&quot;Optie 3&quot;&gt; 
&lt;label for=&quot;optie_3&quot;&gt;Dit is optie 3&lt;/label&gt;
</pre>
<ul>
<li>Elk keuze rondje krijgt dezelfde naam via het <code>name</code> attribuut</li>
<li>De waarde die wordt verstuurd staat in het <code>value</code> attribuut van elk keuze rondje</li>
<li>De <code>id</code> van de optie is belangrijk om het label via het <code>for</code> attribuut te koppelen</li>
<li>De optie die al geselecteerd wordt bij het laden krijgt het attribuut <code>checked</code> mee</li>
</ul>

<pre data-enlighter-language="html">
&lt;input type=&quot;radio&quot; checked /&gt;
</pre>
#### Selectie vakje (checkbox)
Er zijn meerdere opties mogelijk.

<pre data-enlighter-language="html">
&lt;input type=&quot;checkbox&quot; id=&quot;optie_1&quot; name=&quot;optie_1&quot; value=&quot;Optie 1&quot;&gt; 
&lt;label for=&quot;optie_1&quot;&gt;Dit is optie 1&lt;/label&gt;&lt;br /&gt; 
&lt;input type=&quot;checkbox&quot; id=&quot;optie_2&quot; name=&quot;optie_2&quot; value=&quot;Optie 2&quot;&gt; 
&lt;label for=&quot;optie_2&quot;&gt;Dit is optie 2&lt;/label&gt;&lt;br /&gt; 
&lt;input type=&quot;checkbox&quot; id=&quot;optie_3&quot; name=&quot;optie_3&quot; value=&quot;Optie 3&quot;&gt; 
&lt;label for=&quot;optie_3&quot;&gt;Dit is optie 3&lt;/label&gt;
</pre>

<ul>
<li>Elke optie krijgt een aparte naam via het <code>name</code> attribuut</li>
<li>De waarde die wordt verstuurd staat in het <code>value</code> attribuut van elke optie</li>
<li>De <code>id</code> van de optie is belangrijk om het label via het <code>for</code> attribuut te koppelen</li>
<li>De optie die al geselecteerd wordt bij het laden krijgt het attribuut <code>checked</code> mee</li>
</ul>

<pre data-enlighter-language="html">
&lt;input type=&quot;checkbox&quot; checked /&gt;
</pre>

#### Een groot tekstveld
<pre data-enlighter-language="html">
&lt;textarea name=&quot;bericht&quot; rows=&quot;10&quot; cols=&quot;30&quot;&gt;&lt;/textarea&gt;
</pre>
<ul>
<li>Via het attribuut <code>cols</code> geef je de breedte op van het tekstveld</li>
<li>Via het attribuut <code>rows</code> geef je de hoogte op van het tekstveld</li>
<li>Een <code>name</code> attribuut is verplicht bij een textarea element</li>
</ul>
#### Een knop
<pre data-enlighter-language="html">
&lt;button type=&quot;button&quot;&gt;Klik mij!&lt;/button&gt;
</pre>

#### Een verzend knop
<pre data-enlighter-language="html">
&lt;input type=&quot;submit&quot; value=&quot;Verstuur&quot; /&gt;
</pre>
Een verzend knop verzend de inhoud van het formulier naar de de URL die in het <code>action</code> attribuut staat van het <code>&lt;form&gt;</code> element.

#### Bestand opladen
<pre data-enlighter-language="html">
&lt;input type=&quot;file&quot; name=&quot;bestand&quot;&gt;
</pre>
