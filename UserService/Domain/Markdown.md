# 🎯 Strategisk DDD Analyse - HaaV

Dette dokument beskriver forretningsdomænet og de strategiske valg for HaaV-platformen.

---

## 🏛️ Opgave A: Forretningskompetencer (Business Capabilities)
Vi har identificeret tre kernekompetencer, der understøtter strategien direkte og er svære at kopiere.

| Kompetence | Beskrivelse                                                                          | Forretningsfunktioner                                                          |
| :--- |:-------------------------------------------------------------------------------------|:-------------------------------------------------------------------------------|
| **Sortiment- & Kategoristyring** | Evnen til at udvælge de rigtige produkter til de rigtige priser baseret på data      | Prisoptimering <br>• Sæsonplanlægning                                          |
| **Medlemsstyring & Onboarding** | Effektiv håndtering af selvstændige forretninger (medlemmer) på platformen           | • Validering af standarder <br>• Kontingentstyring                             |
| **Logistik-koordinering** | Sikring af effektiv varestrøm fra medlemmer til slutkunder.                          | • Ruteoptimering <br>• Leveringssporing                                        |

---

## 🧩 Opgave B: DDD Underdomæner
Vi har nedbrudt kompetencen **Sortiment- og kategoristyring** for at identificere kerneværdien.

### 1. Kerne-underdomæner (Core Domains) ⭐
Disse skaber reel konkurrencefordel
* **Kategoristrategi**: Definition af varekategorier (f.eks. økologi).
* **Performance Analyse**: Optimering af sortiment baseret på salgsdata.

### 2. Support-underdomæner 🛠️
Nødvendige for at understøtte kernen.
* **Produktkatalog**: Central styring af stamdata, billeder og beskrivelser.
* **Kampagnestyring**: Værktøjer til tidsbegrænsede tilbud.

### 3. Generiske underdomæner 📦
Standardfunktionalitet der kan købes eller løses med standardsoftware.
* **Lageroptælling**: Simpel tælle-funktion til beholdning.
* **Pris-sammenligning**: Opslag af markedspriser via eksterne API'er.

---

## 🗺️ Opgave C: Afgrænsede Kontekster (Bounded Contexts)
Vi har identificeret følgende kontekster, der skal fungere enestående:

* **Salgskontekst**: Alt hvad kunden ser (Katalog, Priser, Søgning).
* **Logistikkontekst**: Alt omkring fysisk flytning af varer og lagerstatus.