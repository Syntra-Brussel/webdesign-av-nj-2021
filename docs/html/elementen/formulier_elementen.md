---
layout: template
title: Attributen
url: /html/elementen/formulier_elementen
collection: [html, elementen]
---

## Formulier elementen

Een hoeksteen van webpagina’s zijn formulieren. Ze bestaan al sinds het begin maar sinds de introductie van HTML5 zijn de mogelijkheden grondig uitgebreid.

Formulier elementen worden samen gezet in een <span style="color: blue">&lt;form&gt;</span> element.

Het <span style="color: blue">&lt;form&gt;</span> element heeft enkele belangrijke attributen:

<span style="color: green"><u>action</u></span>: de URL naar waar het formulier gestuurd moet worden voor verwerking
<span style="color: green"><u>method</u></span>: GET (de inhoud van de velden wordt via de URL mee gestuurd), POST (de inhoud van de velden wordt onzichtbaar verstuurd)
Voor de introductie van HTML5 waren er al heel wat formulier elementen.

Alle invoer velden moeten binnen <span style="color: blue">&lt;form&gt;</span> en <span style="color: blue">&lt;form&gt;</span> staan.

<img src="{{ '/html/elementen/images/form_html.png' | relative_url}}" />

### Elementen die sinds HTML5 bestaan
Er zijn tal van nieuwe elementen geïntroduceerd die veel meer frontend validatie mogelijk maken.

<pre data-enlighter-language="html">
&lt;input type=&quot;email&quot; required placeholder=&quot;Voer een e-mailadres in&quot; /&gt;
</pre>

Het required attribuut zorgt voor een frontend validatie op een geldig e-mail adres formaat voor het formulier wordt verstuurd.

Naast het type email, zijn ook volgende types geïntroduceerd:

color
date
datetime
datetime-local
email
month
number
range
search
tel
time
url
week

### Elementen die al voor HTML5 bestonden
#### Een tekstveld
<pre data-enlighter-language="html">
&lt;input name=&quot;voornam&quot; type=&quot;text&quot;&gt;
</pre>
Het name attribuut is verplicht bij een input element

#### De selectielijst
<pre data-enlighter-language="html">
&lt;select name=&quot;auto&quot;&gt; 
  &lt;option value=&quot;volvo&quot;&gt;Volvo&lt;/option&gt; 
  &lt;option selected value=&quot;saab&quot;&gt;Saab&lt;/option&gt; 
  &lt;option value=&quot;fiat&quot;&gt;Fiat&lt;/option&gt; 
  &lt;option value=&quot;audi&quot;&gt;Audi&lt;/option&gt; 
&lt;/select&gt;
</pre>
Waneer meer dan 1 optie geselecteerd mag worden krijgt het <select> element een attribuut multiple.
De optie die geselecteerd wordt krijgt het attribuut selected
Een name attribuut is verplicht bij een select element

#### Selectie rondje (radio)
Er is maar één optie mogelijk.

<pre data-enlighter-language="html">
&lt;input type=&quot;radio&quot; id=&quot;optie_1&quot; name=&quot;optie&quot; value=&quot;Optie 1&quot;&gt; 
&lt;label for=&quot;optie_1&quot;&gt;Dit is optie 1&lt;/label&gt;&lt;br /&gt; 
&lt;input type=&quot;radio&quot; id=&quot;optie_2&quot; name=&quot;optie&quot; value=&quot;Optie 2&quot;&gt; 
&lt;label for=&quot;optie_2&quot;&gt;Dit is optie 2&lt;/label&gt;&lt;br /&gt; 
&lt;input type=&quot;radio&quot; id=&quot;optie_3&quot; name=&quot;optie&quot; value=&quot;Optie 3&quot;&gt; 
&lt;label for=&quot;optie_3&quot;&gt;Dit is optie 3&lt;/label&gt;
</pre>

Elke optie krijgt dezelfde naam via het name attribuut
De waarde die wordt verstuurd staat in het value attribuut van elke optie
De id van de optie is belangrijk om het label via het for attribuut te koppelen
De optie die al geselecteerd wordt bij het laden krijgt het attribuut checked mee
<input type="radio" checked />

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

Elke optie krijgt een aparte naam via het name attribuut
De waarde die wordt verstuurd staat in het value attribuut van elke optie
De id van de optie is belangrijk om het label via het for attribuut te koppelen
De optie die al geselecteerd wordt bij het laden krijgt het attribuut checked mee

<pre data-enlighter-language="html">
&lt;input type=&quot;checkbox&quot; checked /&gt;
</pre>

#### Een groot tekstveld
<pre data-enlighter-language="html">
&lt;textarea name=&quot;bericht&quot; rows=&quot;10&quot; cols=&quot;30&quot;&gt;&lt;/textarea&gt;
</pre>

Via het attribuut cols geef je de breedte op van het tekstveld.
Via het attribuut rows geef je de hoogte op van het tekstveld.
Een name attribuut is verplicht bij een textarea element

#### Een knop
<pre data-enlighter-language="html">
&lt;button type=&quot;button&quot;&gt;Klik mij!&lt;/button&gt;
</pre>

#### Een verzend knop
<pre data-enlighter-language="html">
&lt;input type=&quot;submit&quot; value=&quot;Verstuur&quot; /&gt;
</pre>
Een verzend knop verzend de inhoud van het formulier naar de de URL die in het action attribuut staat van het form element.

#### Bestand opladen
<pre data-enlighter-language="html">
&lt;input type=&quot;file&quot; name=&quot;bestand&quot;&gt;
</pre>
