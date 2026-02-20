# 📄 Forretningsentiteter - HaaV

Dette dokument definerer de centrale entiteter i konteksten **Salg og Ordrehåndtering**.

| Entitet | Beskrivelse                                                    | Rolle i Forretningen               |
| :--- |:---------------------------------------------------------------|:-----------------------------------|
| **Medlem** | En forretning eller selvstændig person i HaaV's infrastruktur. | Sælger af varer/services           |
| **Produkt** | Fysisk vare eller service leveret af et medlem.                | Kernen i salget                    |
| **Katalog** | En samling af tilgængelige varer og services.                  | Kundens indgang til sortimentet    |
| **Adresse** | Data omkring placering af medlem eller levering..              | Bruges til lokation og logistik    |
| **Kunde** | Personen eller virksomheden der foretager købet.               | Den ordregivende part              |
| **Ordre** | Binder kunde, produkt og medlem sammen ved et køb.             | Dokumentation for transaktionen    |
| **Lagerstatus** | Information om rådighed af et produkt hos et medlem.           | Sikrer korrekt leveringsevne       |