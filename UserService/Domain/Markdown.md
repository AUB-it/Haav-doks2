# 🎯 Strategisk DDD Analyse - HaaV

[cite_start]Dette dokument beskriver forretningsdomænet og de strategiske valg for HaaV-platformen[cite: 3, 5].

---

## 🏛️ Opgave A: Forretningskompetencer (Business Capabilities)
[cite_start]Vi har identificeret tre kernekompetencer, der understøtter strategien direkte og er svære at kopiere[cite: 25, 29, 32].

| Kompetence | Beskrivelse | Forretningsfunktioner |
| :--- | :--- | :--- |
| **Sortiment- & Kategoristyring** | [cite_start]Evnen til at udvælge de rigtige produkter til de rigtige priser baseret på data[cite: 24, 38]. | [cite_start]• Prisoptimering [cite: 26][cite_start]<br>• Sæsonplanlægning [cite: 26, 39] |
| **Medlemsstyring & Onboarding** | [cite_start]Effektiv håndtering af selvstændige forretninger (medlemmer) på platformen[cite: 61]. | [cite_start]• Validering af standarder [cite: 26][cite_start]<br>• Kontingentstyring [cite: 26] |
| **Logistik-koordinering** | Sikring af effektiv varestrøm fra medlemmer til slutkunder. | [cite_start]• Ruteoptimering [cite: 26][cite_start]<br>• Leveringssporing [cite: 26] |

---

## 🧩 Opgave B: DDD Underdomæner
[cite_start]Vi har nedbrudt kompetencen **Sortiment- og kategoristyring** for at identificere kerneværdien[cite: 38, 41].

### 1. Kerne-underdomæner (Core Domains) ⭐
[cite_start]*Disse skaber reel konkurrencefordel[cite: 30, 33].*
* [cite_start]**Kategoristrategi**: Definition af varekategorier (f.eks. økologi)[cite: 39, 42].
* [cite_start]**Performance Analyse**: Optimering af sortiment baseret på salgsdata[cite: 39, 42].

### 2. Support-underdomæner 🛠️
[cite_start]*Nødvendige for at understøtte kernen[cite: 43].*
* [cite_start]**Produktkatalog**: Central styring af stamdata, billeder og beskrivelser[cite: 42, 62].
* [cite_start]**Kampagnestyring**: Værktøjer til tidsbegrænsede tilbud[cite: 42].

### 3. Generiske underdomæner 📦
[cite_start]*Standardfunktionalitet der kan købes eller løses med standardsoftware[cite: 44].*
* [cite_start]**Lageroptælling**: Simpel tælle-funktion til beholdning[cite: 44].
* [cite_start]**Pris-sammenligning**: Opslag af markedspriser via eksterne API'er[cite: 44].

---

## 🗺️ Opgave C: Afgrænsede Kontekster (Bounded Contexts)
[cite_start]Vi har identificeret følgende kontekster, der skal fungere enestående[cite: 45, 46]:

* [cite_start]**Salgskontekst**: Alt hvad kunden ser (Katalog, Priser, Søgning)[cite: 53, 71].
* [cite_start]**Logistikkontekst**: Alt omkring fysisk flytning af varer og lagerstatus[cite: 53, 75].