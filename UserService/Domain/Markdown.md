🎯Opgave A: Forretningskompetencer

Vi har identificeret tre centrale kernekompetencer for HaaV:

Sortiment- og kategoristyring

* Beskrivelse: Evnen til at udvælge de helt rigtige produkter til de rigtige priser baseret på data.

* Forretningsfunktioner: Prisoptimering og Sæsonplanlægning.


Medlemsstyring & Onboarding

* Beskrivelse: Effektiv håndtering af selvstændige forretninger (medlemmer), så de hurtigt kan sælge gennem platformen.

* Forretningsfunktioner: Validering af medlemmer og medlemskontingent-styring.


Logistik-koordinering 

* Beskrivelse: Sikring af at varer flyttes effektivt fra de enkelte medlemmer til slutkunden. 

* Forretningsfunktioner: Ruteoptimering og leveringssporing.


🎯Opgave B: DDD Underdomæner

Vi har nedbrudt kompetencen Sortiment- og kategoristyring i følgende underdomæner:

1. Kerne-underdomæner (Core Domains)

Disse skaber reel konkurrencefordel og er svære at kopiere:

* Kategoristrategi: Ansvarlig for at definere hvilke varekategorier HaaV skal satse på (f.eks. økologi eller lokalt håndværk).

* Performance Analyse: Overvågning af hvilke varer der sælger, så sortimentet løbende kan optimeres.


2. Support-underdomæner

Nødvendige funktioner, der understøtter kernen:

* Produktkatalog: Systemet der holder styr på billeder, beskrivelser og tekniske data for alle varer.

* Kampagnestyring: Værktøjer til at køre tidsbegrænsede tilbud på specifikke kategorier.


3. Generiske underdomæner

* Standardfunktionalitet som kan købes eller løses med standard-software:

* Lageroptælling: En simpel tælle-funktion til at holde styr på beholdning.

* Pris-sammenligning: Eksterne opslag til at tjekke markedspriser.


🎯Opgave C: Afgrænsede Kontekster (Bounded Contexts)

* Vi har identificeret følgende afgrænsede kontekster:


* Salgskontekst: Håndterer alt hvad kunden ser, herunder produktvisning, søgning og prisberegning.


* Logistikkontekst: Håndterer alt omkring den fysiske flytning af varer og lagerstatus