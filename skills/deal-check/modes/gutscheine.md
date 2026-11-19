# Gutscheine

Findet Gutscheincodes für den Shop mit dem besten Angebot und probiert sie im Warenkorb aus, damit am Ende ein echter Endpreis steht statt einer Liste von Codes, die vielleicht nicht gehen.

Läuft eigenständig („Gibt es einen Gutscheincode für …?“) oder als letzter Schritt von **Deal prüfen**, nachdem der günstigste seriöse Shop feststeht.

## 1. Codes finden

Such für **genau diesen Shop** und, wenn möglich, genau dieses Produkt. In dieser Reihenfolge, weil die Trefferquote sinkt:

| Quelle | Was du suchst |
|---|---|
| **Shop selbst** | Aktionsseite, Banner, App-Rabatt, Neukunden- oder Newsletter-Rabatt, Rabatt in den AGB oder FAQ |
| **Postfach** (wenn verbunden) | Codes aus Werbemails dieses Shops, siehe `postfach.md` |
| **Deal-Communities** (z. B. mydealz) | Beiträge der letzten 7 Tage, in denen andere bestätigen, dass der Code funktioniert |
| **Gutscheinportale** | Nur als letzte Quelle. Viele Codes dort sind abgelaufen oder erfunden. |

Notiere pro Code: **Code, Wert, Bedingungen** (Mindestbestellwert, nur Neukunden, nur App, ausgeschlossene Marken oder Kategorien, nicht mit reduzierter Ware kombinierbar), **Ablaufdatum, Quelle mit Link, Datum des Beitrags**.

Zusätzlich kurz prüfen, ob es **Cashback oder Bonuspunkte** gibt (z. B. über ein Cashback-Portal oder ein Bonusprogramm des Shops). Nur nennen, nicht anmelden.

**Nicht tun:**
- Keine Codes erraten oder Varianten durchprobieren (BF10, BF15, BF20 …).
- Keine personalisierten Einmalcodes verwenden, die erkennbar für jemand anderen ausgestellt wurden.
- Für einen Newsletter-Rabatt nichts anmelden. Sag der Person, dass es ihn gibt, und lass sie entscheiden.

Höchstens fünf Codes weiterverfolgen, die wahrscheinlichsten zuerst.

## 2. Codes ausprobieren

Geht nur mit einem Browser-Werkzeug (z. B. Claude in Chrome, der Browser in der Claude-App oder Computer Use; in Claude Code ein verbundener Browser). Ohne Browser: weiter mit Schritt 3 und alle Codes als **ungetestet** kennzeichnen.

**Vorher fragen**, in einem Satz: „Soll ich die Codes im Warenkorb von [Shop] testen? Ich lege das Produkt in den Warenkorb, gebe die Codes ein und kaufe nichts.“ Erst nach einem Ja weiter.

Ablauf:
1. Produktseite öffnen, **gleiche Variante** in den Warenkorb legen. Als Gast, kein Konto anlegen. Ist die Person im Shop schon eingeloggt, ist das in Ordnung, aber nichts am Konto ändern.
2. Den Warenkorb öffnen und den Endpreis **ohne Code** notieren.
3. Codes einzeln eingeben. Nach jedem Code den Endpreis inklusive Versand ablesen, die Meldung des Shops wörtlich notieren („Code ungültig“, „Mindestbestellwert nicht erreicht“) und den Code wieder entfernen, bevor der nächste kommt.
4. Am Ende den Code mit dem niedrigsten Endpreis eingelöst lassen und der Person sagen, dass der Warenkorb so bereitliegt.

**Harte Grenzen:**
- **Nie auf „Zur Kasse“, „Jetzt kaufen“ oder „Zahlungspflichtig bestellen“ klicken.** Endstation ist der Warenkorb.
- Keine Adresse, keine Zahlungsdaten, keine E-Mail eingeben. Zeigt der Shop das Gutscheinfeld erst nach der Adresseingabe: aufhören und „Gutscheinfeld erst an der Kasse, nicht getestet“ notieren.
- Bei Captcha, Bot-Schutz oder einer Sperre wegen zu vieler Versuche aufhören. Nichts umgehen.

## 3. Ausgabe

```
GUTSCHEINE · [Shop] · [Produkt]
Stand: [Datum, Uhrzeit]

Endpreis ohne Code: [Betrag]
Bester Endpreis mit Code: [Betrag] mit [CODE] (getestet / ungetestet)

| Code | Wert | Bedingung | Ergebnis im Warenkorb | Quelle |
| … | … | … | funktioniert: [Endpreis] / abgelehnt: „[Meldung]“ / ungetestet | Link, Datum |

Zusätzlich möglich: [Cashback, Bonuspunkte, Newsletter-Rabatt], nicht eingerechnet
```

Nur **getestete** Codes fließen in den Endpreis und ins Urteil von **Deal prüfen** ein. Ungetestete Codes stehen dabei, ändern das Urteil aber nicht.
