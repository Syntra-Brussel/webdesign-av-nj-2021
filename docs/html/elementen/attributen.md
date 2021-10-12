---
layout: template
title: lementen hebben attributen
url: /html/elementen/attributen
collection: [html, elementen]
---

## {{ page.title }}

Elementen hebben doorgaans attributen om extra eigenschappen aan het element toe te voegen:

Een attribuut bestaat uit een <span style="color: green">naam</span>, een <span style="color: red">=</span> en vervolgens een <span style="color: blue">waarde</span> tussen dubbele quotes.

<img src="{{ '/html/elementen/images/attributen_1.png' | relative_url}}" />

In dit voorbeeld wordt een link getoond (een “<strong>a</strong>nchor”). De waarde van het <code>href</code> attribuut is de URL die wordt geopend als je er klikt.

<img src="{{ '/html/elementen/images/attributen_2.png' | relative_url}}" />

Standaard wordt een link geopend in het zelfde venster. Het <code>target</code> attribuut geeft aan dat de link wordt geopend in een nieuw venster.

<img src="{{ '/html/elementen/images/attributen_3.png' | relative_url}}" />

In dit voorbeeld wordt een beeld (“image”) getoond. Het attribuut <code>src</code> bevat de URL naar het beeld. Een <code>&lt;img&gt;</code> element heeft geen inhoud dus wordt het meteen gesloten.

Een belangrijk attribuut voor de opmaak van het HTML elementen is het <code>class</code> attribuut.

<img src="{{ '/html/elementen/images/attributen_4.png' | relative_url}}" />

Een ander belangrijk attribuut voor de interactie via JavaScript is het het <code>id</code> attribuut.

<img src="{{ '/html/elementen/images/attributen_5.png' | relative_url}}" />

De <code>id</code> moet uniek zijn per HTML-document. In dit geval mag er dus geen ander element zijn met het id “logo” voorkomen.



