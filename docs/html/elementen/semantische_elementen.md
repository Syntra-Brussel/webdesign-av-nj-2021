---
layout: template
title: Semantische elementen
url: /html/elementen/semantische_elementen
collection: [html, elementen]
---
## {{ page.title }}

### Structurele elementen

Het <code><section></code> element definieert een sectie in een webpagina. De inhoud van en sectie hoort thematisch samen.

De inhoud van het <code><article></code> moet zin hebben op zichzelf. Je moet de inhoud op zichzelf kunnen legen.
Bijvoorbeeld: forum post, blog post, nieuws artikel

Het <code><header></code> element slaat op de inhoud in de hoofding.

Het <code><aside></code> element heeft inhoud die los staat van de hoofd elementen maar er wel aan gerelateerd is.

Het <code><footer></code> element bevat de inhoud onderaan een pagina. 
Bijvoorbeeld:  auteur van het document, copyright informatie, privacy informatie, contact informatie

### Semantische elementen combineren
<pre data-enlighter-language="html">
&lt;article&gt; 
  &lt;h1&gt;Weersvoorspelling voor Antwerpen&lt;/h1&gt; 
  &lt;article&gt; 
    &lt;h2&gt;1 maart 2020&lt;/h2&gt; 
    &lt;p&gt;Regen&lt;/p&gt; 
  &lt;/article&gt; 
  &lt;article&gt; 
    &lt;h2&gt;4 maart 2020&lt;/h2&gt; 
    &lt;p&gt;Periodes met regen&lt;/p&gt; 
  &lt;/article&gt; 
  &lt;article&gt; 
    &lt;h2&gt;5 maart 2020&lt;/h2&gt; 
    &lt;p&gt;Hevige regen&lt;/p&gt; 
  &lt;/article&gt;
&lt;/article&gt;
</pre>

### Andere semantische elementen

#### <code>&lt;figure&gt;</code> en <code>&lt;figcaption&gt;</code> elementen
<pre data-enlighter-language="html">
&lt;figure&gt; 
  &lt;img src=&quot;storm_ciara_zorgt_voor_veel_schade.jpg&quot; alt=&quot;Storm Ciara zorgt voor veel schade&quot;&gt; 
  &lt;figcaption&gt;Storm Ciara zorgt voor veel schade in Antwerpen&lt;/figcaption&gt; 
&lt;/figure&gt;
</pre>
 
Gebruik <code>&lt;figure&gt;</code> als inhoud element (bijvoorbeeld in een <code>&lt;p&gt;</code> element) en niet als layout element.

#### <code><nav></code> element
<pre data-enlighter-language="html">
&lt;nav&gt; 
  &lt;a href=&quot;/html/&quot;&gt;HTML&lt;/a&gt; | 
  &lt;a href=&quot;/css/&quot;&gt;CSS&lt;/a&gt; | 
  &lt;a href=&quot;/js/&quot;&gt;JavaScript&lt;/a&gt; | 
&lt;/nav&gt;
</pre>

#### <code>srcset</code> attribuut bij een <code>&lt;img&gt;</code> element
Een attribuut dat beelden met een verschillend formaat voorziet voor verschillende scherm breedtes.

De browser bepaalt zelf welk beeld het gaat inladen.

<pre data-enlighter-language="html">
&lt;img srcset=&quot;beeld_w300.jpg w300, beeld_w1000.jpg w1000, beeld_w2000.jpg w2000&quot; src=&quot;beeld.jpg&quot;&gt;
</pre>

Wanneer <code>srcset</code> niet wordt ondersteund door de browser wordt het beeld uit het <code>src</code> attribuut geladen.

#### <code>&lt;fieldset&gt;</code> element
Nog een voorbeeld van een element zonder veel basis opmaak maar met een duidelijk doel is het <code>&lt;fieldset&gt;</code> element. Zoals de naam het zegt staat het rond een aantal velden (doorgaans in een formulier).

Binnen een <code>&lt;fieldset&gt;</code> element komt bovenaan vaak een <code>&lt;legend&gt;</code> element dat een omschrijving bevat van de velden of van het formulier.

<pre data-enlighter-language="html">
&lt;form&gt; 
  &lt;fieldset&gt; 
    &lt;legend&gt;Inschrijven op de nieuwsbrief&lt;/legend&gt; 
    &lt;input type=&quot;text&quot; id=&quot;naam&quot; name=&quot;naam&quot;&gt; 
    &lt;label for=&quot;naam&quot;&gt;Naam&lt;/label&gt;&lt;br/&gt; 
    &lt;input type=&quot;email&quot; id=&quot;email&quot; name=&quot;email&quot;&gt; 
    &lt;label for=&quot;email&quot;&gt;e-mail&lt;/label&gt;&lt;br/&gt; 
    &lt;input type=&quot;submit&quot; id=&quot;versturen&quot; name=&quot;versturen&quot; value=&quot;Inschrijven&quot;&gt; 
  &lt;/fieldset&gt; 
&lt;/form&gt;
</pre>