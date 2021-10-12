---
layout: template
title: Meta elementen
url: /html/elementen/meta_elementen
collection: [html, elementen]
---

## {{ page.title }}

<div class="highlight">
    <h3>Meta informatie</h3>
    Meta informatie geeft informatie over informatie, in dit geval het HTML-document.

    Je zal meta informatie nooit zien op de webpagina zelf maar deze data wordt wel verwerkt door de browser en de zoekmachine.
</div>


<pre data-enlighter-language="html">
&lt;head&gt;
  &lt;meta charset=&quot;utf-8&quot;&gt;
  &lt;title&gt;Voorbeeld van meta-tags&lt;/title&gt;
  &lt;meta name=&quot;description&quot; content=&quot;Wij leren HTML&quot;&gt;
  &lt;meta name=&quot;keywords&quot; content=&quot;HTML,CSS,JavaScript&quot;&gt;
  &lt;meta name=&quot;author&quot; content=&quot;Syntra Brussel&quot;&gt;
  &lt;meta name=&quot;viewport&quot; content=&quot;width=device-width, initial-scale=1.0&quot;&gt; 
&lt;/head&gt;
</pre>

Het <code>&lt;meta&gt;</code> element <strong>description</strong> zorgt voor een korte samenvatting van het HTML document.

Het <code>&lt;meta&gt;</code> element <strong>keywords</strong> bevat de belangrijkste trefwoorden waarover het HTML document gaat.

Het <code>&lt;meta&gt;</code> element <strong>author</strong> bevat de naam van de auteur van de inhoud op de pagina.

A <code>&lt;meta&gt;</code> element <strong>viewport</strong> geeft instructies aan de browser hoe een pagina de pagina moet geladen worden wat betreft afmetingen en schalen.

Het <code>width=device-width</code> gedeelte stelt de breedte van de pagina in, in dit geval neemt hij de breedte (aantal pixels) van het toestel waarop de pagina wordt geopend.

Het <code>initial-scale=1.0</code> gedeelte stelt het initiële zoom niveau in.

Hieronder zie je een voorbeeld van een pagina met (rechts) en zonder (links) <code>&lt;meta&gt;</code> viewport element:

<img src="{{ '/html/elementen/images/viewport.png' | relative_url}}" />

