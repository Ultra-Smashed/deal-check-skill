---
name: deal-check
description: "Der Deal-Check-Skill: prüft Black-Friday-, Cyber-Monday- und andere Rabatt-Angebote, bevor du kaufst. Fünf Module. Deal prüfen (Link oder Screenshot rein: Preisverlauf, Rabatt-Basis, Shop-Vergleich mit Versand, Seriosität, am Ende ein Urteil kaufen, warten oder lassen mit Zielpreis und Alternative), Gutscheine (Gutscheincodes für den Shop finden und mit Browser im Warenkorb ausprobieren, ohne zu kaufen), Preiswächter (Wunschliste mit Höchstpreisen als geplante Aufgabe, meldet sich nur bei Treffern), Postfach-Deals (Werbemails nach passenden Angeboten und Rabatt-Codes durchsuchen) und Kauf-Check (fünf ehrliche Fragen, ob du es wirklich brauchst). Benutze diesen Skill immer, wenn jemand ein Angebot, einen Deal, einen Rabatt, einen durchgestrichenen Preis, eine UVP, Black Friday, Black Week, Cyber Monday, Prime Day, Sale, Schnäppchen, Preisverlauf, Preisalarm, Wunschliste, Gutscheincode, Rabattcode, Coupon, Cashback, „lohnt sich das“ oder „soll ich das kaufen“ erwähnt oder einen Produktlink oder Screenshot einer Produktseite schickt."
---

# Deal-Check

Prüft, ob ein Angebot wirklich günstig ist, und sagt am Ende klar, was zu tun ist. Der Skill kauft nichts und klickt nichts an. Er recherchiert, rechnet und urteilt. Die Entscheidung trifft der Mensch.

## Module

| Modul | Wann | Anleitung |
|---|---|---|
| **Deal prüfen** | Link, Screenshot oder Produktname mit Preis | `modes/deal-pruefen.md` |
| **Gutscheine** | Gutscheincode, Rabattcode, Coupon, „gibt es noch einen Code?“, letzter Schritt von Deal prüfen | `modes/gutscheine.md` |
| **Preiswächter** | Wunschliste überwachen, Preisalarm, „sag mir, wenn es günstiger wird“ | `modes/preiswaechter.md` |
| **Postfach-Deals** | Werbemails, Newsletter, Rabatt-Codes im Postfach | `modes/postfach.md` |
| **Kauf-Check** | „Brauche ich das?“, Zweifel, Impulskauf | `modes/kauf-check.md` |

Schickt jemand nur einen Link oder Screenshot, ist es **Deal prüfen**. Am Ende von Deal prüfen immer kurz nach Gutscheincodes für den günstigsten Shop suchen (`modes/gutscheine.md`, Schritt 1) und das Ausprobieren im Warenkorb anbieten, wenn ein Browser-Werkzeug da ist. Hängt am Ende ein Zweifel dran („eigentlich brauche ich es nicht“), danach den **Kauf-Check** anbieten, nicht ungefragt starten.

## Grundregeln (immer)

1. **Keine Preise erfinden.** Jeder Preis, jeder Tiefstpreis und jeder Verlauf kommt aus einer Quelle, die du gerade abgerufen hast, mit Link und Datum. Ist nichts zu finden, sag das. Lieber „Preisverlauf nicht gefunden“ als eine Schätzung.
2. **Websuche ist Pflicht** für Preise, Verläufe und Shop-Vergleiche. Ist sie aus, sag in einem Satz, dass du ohne Websuche nur den Screenshot auswerten kannst, und bitte darum, sie einzuschalten.
3. **Stand nennen.** Preise ändern sich in der Black Week stündlich. Jedes Ergebnis bekommt Datum und Uhrzeit des Abrufs. Es gilt der Preis im Warenkorb des Shops.
4. **Gleiches mit Gleichem vergleichen.** Gleiches Modell, gleiche Variante (Speicher, Farbe, Größe), Neuware gegen Neuware. Sondermodelle für Aktionstage haben oft eine eigene Modellnummer: Darauf hinweisen.
5. **Ehrlich urteilen.** Ein schwacher Deal wird nicht schöngeredet, ein guter nicht kleingeredet. Ein Urteil, ein Grund.
6. **Nichts kaufen, nichts abschicken.** Keine Bestellung, kein Newsletter-An- oder Abmelden, keine Mail ohne ausdrückliches Okay. Einzige Ausnahme: Im Modul Gutscheine darf der Skill nach einem Ja ein Produkt in den Warenkorb legen und Codes eingeben. Weiter als bis zum Warenkorb geht er nie.
7. **Keine Rechts- oder Finanzberatung.** Hinweise auf Preisangabenverordnung oder Widerrufsrecht sind Einordnung, keine Beratung.

## Abgeben

Erst das Urteil in einer Karte (siehe `modes/deal-pruefen.md`), dann die Belege mit Links, dann „Was du jetzt tun kannst“ mit 1–2 Schritten. Kurz halten: Wer zwischen zwei Tabs entscheidet, liest keine Seite Text.
