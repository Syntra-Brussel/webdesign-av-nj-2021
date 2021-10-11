---
layout: template
title: Belangrijkste termen
url: /git/belangrijkste_termen
collection: git
---

## Belangrijkste termen

### Repository
Een code base op een GIT server. Het bewaart de bestanden, de aanpassingen en door wie die aanpassingen zijn gedaan.

Aanpassingen gebeuren eerst lokaal en worden dan gesynchroniseerd met de repository.

Je kan een nieuwe (lege) repository maken of op een bestaande verder werken. In dat laatste geval die je een <em>clone</em> op basis van een git URL.

### Working directory
De lokale folder waarin gewerkt wordt. GIT houdt de aanpassingen bij.

### (un)tracked / (niet) gevolgd
Een bestand waarvan de aanpassingen nog niet worden gevolgd door GIT. Je ziet de laatste versie.

### (un)staged / (niet) klaarzetten
Bepaalde aanpassingen moeten worden klaar gezet om te synchroniseren. Enkel de klaar gezette aanpassingen kunnen worden gesyncroniseerd.

### commit / goedkeuren
De klaargezette aanpassingen kunnen nu samen gecommit worden. Dit gebeurd doorgaans wanneer een bepaalde taak is afgewerkt. Je geeft elke commit ook een omschrijving.

### push / duw
De bestanden die zijn gecommit kunnen nu naar de GIT server wordt geduwd.

### branch
Bij het opzetten van een repository heb je 1 branch. De hoofd branch (master of main). Je kan ook verschillende versies van je codebase bijhouden door daarvoor aparte branches maken. 

Je kan dan ook de code van verschillende branches mengen (merge) enzovoort.

We gaan daar in deze cursus niet dieper op in.

### pull / trek
Aanpassingen van anderen die via “stage” > “commit” > “push” naar de GIT server zijn gestuurd kan je nu synchroniseren met je working directory.

### conflict
Wanneer een aanpassing door een andere persoon is gedaan (“stage” > “commit” > “push”) wanneer jij ook een push wil doen van een aanpassing zal een conflict optreden.

Je krijgt dan een foutboodschap en zal eerst een pull moeten doen. GIT probeert dan de code nog te mengen (merge). Als dat niet lukt voegt plaats de 2 versies samen zodat het conflict manueel kan opgelost worden. 

Na een manuele aanpassing van een conflict doe je terug een “<i>stage</i>” > “<i>commit</i>” > “<i>push</i>”.