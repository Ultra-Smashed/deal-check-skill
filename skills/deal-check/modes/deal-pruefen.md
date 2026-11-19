# Deal prüfen

Eingabe: ein Produktlink, ein Screenshot der Produktseite oder Produktname plus Preis. Ziel: in wenigen Minuten ein belegtes Urteil.

## 1. Produkt genau bestimmen

- Hersteller, Modell, Variante (Speicher, Farbe, Größe), wenn sichtbar EAN oder Modellnummer.
- Verkauft der Shop selbst oder ein Drittanbieter über einen Marktplatz? Das steht meist klein unter dem Preis.
- Neuware, B-Ware, generalüberholt oder gebraucht?
- Ist etwas unklar, das den Preis ändert (z. B. 128 oder 256 GB), frag **eine** kurze Rückfrage. Sonst weiter.

## 2. Preisverlauf

- Suche den Preisverlauf bei Preisvergleichsportalen (z. B. idealo, geizhals, guenstiger.de). Bei Amazon-Artikeln zusätzlich Preis-Tracker wie Keepa oder camelcamelcamel, wenn erreichbar.
- Notiere nur, was die Quelle zeigt: niedrigster Preis der letzten 30 Tage, der letzten 3 Monate, typischer Preis im Oktober. Immer mit Quelle.
- Wurde der Preis kurz vor der Aktion erhöht und dann „rabattiert“? Das ist der wichtigste Befund und gehört ins Urteil.
- Findest du keinen Verlauf: sag es und urteile nur auf Basis des Shop-Vergleichs.

## 3. Rabatt-Basis prüfen

Was ist durchgestrichen?

| Durchgestrichen | Was es bedeutet |
|---|---|
| **UVP** | Unverbindliche Preisempfehlung des Herstellers. Viele Produkte kosten fast nie die UVP. Der Rabatt dazu sagt wenig. |
| **Eigener früherer Preis** („statt“, „vorher“) | Bei einer echten Preissenkung muss der Shop in Deutschland den niedrigsten Preis der letzten 30 Tage angeben (§ 11 PAngV). Prüfe, ob dieser Referenzpreis auf der Seite steht und was er ist. |
| **Kein Vergleichspreis, nur „Deal“-Badge** | Nur der aktuelle Preis zählt. Mit Verlauf und Shop-Vergleich einordnen. |

Rechne die **echte Ersparnis**: gegenüber dem niedrigsten belegten Preis der letzten 30 Tage und gegenüber dem typischen Marktpreis, nicht gegenüber der UVP. Rechne mit Code, wenn mehr als zwei Zahlen im Spiel sind.

Ob § 11 PAngV auch bei UVP-Vergleichen greift, ist umstritten. Bewerte deshalb keinen Shop als rechtswidrig. Formuliere neutral: „Der Rabatt ist von der UVP gerechnet, nicht vom bisherigen Preis.“

## 4. Shop-Vergleich

- Drei seriöse Shops mit dem **Endpreis inklusive Versand**, Lieferzeit und Verfügbarkeit.
- Gutscheincodes nur, wenn sie öffentlich bestätigt und gültig sind. Nicht raten.
- Marktplatz-Angebote von Drittanbietern als solche kennzeichnen.

## 5. Seriosität (nur bei unbekanntem Shop)

Warnzeichen: kein vollständiges Impressum, nur Vorkasse oder Überweisung, Preise weit unter allen anderen Shops, sehr junge Domain, keine oder nur auffällig gleichförmige Bewertungen. Bei Zweifel auf den kostenlosen Fakeshop-Finder der Verbraucherzentrale verweisen und vom Kauf abraten, bis das geklärt ist.

## 6. Urteil

Genau eins von drei:

- **KAUFEN**: Der Preis ist der niedrigste belegte der letzten drei Monate oder liegt höchstens wenige Prozent darüber, und der Shop ist seriös.
- **WARTEN**: Das Produkt war in den letzten Wochen belegbar günstiger, oder der Rabatt bezieht sich nur auf die UVP. Nenne einen **Zielpreis**: den niedrigsten belegten Preis der letzten drei Monate, auf glatte Euro gerundet. Biete den Preiswächter an.
- **LASSEN**: Lockangebot (Preis vorher hochgesetzt), zweifelhafter Shop, veraltetes Modell zum Neupreis oder eine deutlich bessere Alternative zum gleichen Preis.

**Alternative**: nur nennen, wenn sie für den Zweck der Person gleichwertig und günstiger ist, z. B. das Vorgängermodell oder ein anderer Hersteller. Kennst du den Zweck nicht, frag kurz danach oder lass die Alternative weg. Preis der Alternative ebenfalls belegen.

## Ausgabe

```
DEAL-CHECK · [Produkt, Variante]
Stand: [Datum, Uhrzeit]

Urteil: KAUFEN / WARTEN / LASSEN
Grund: [ein Satz]
Zielpreis: [nur bei WARTEN] · Alternative: [falls vorhanden, mit Preis]

Belege
| | Preis | Quelle |
| Angebot jetzt | … | Shop-Link |
| Tiefstpreis 30 Tage | … | Link |
| Tiefstpreis 3 Monate | … | Link |
| Günstigster anderer Shop (inkl. Versand) | … | Link |
Rabatt gerechnet von: [UVP / früherer Preis / keine Angabe]
Echte Ersparnis: [x € bzw. y %] gegenüber [Bezugsgröße]

Was du jetzt tun kannst
1. …
```

Fehlt ein Wert, steht „nicht gefunden“ in der Zeile. Keine leeren Felder füllen.
