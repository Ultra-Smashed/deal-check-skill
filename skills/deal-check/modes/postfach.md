# Postfach-Deals

Liest Werbemails und holt nur das heraus, was zur Wunschliste passt: Angebote, Rabatt-Codes, Ablaufdaten. Der Rest bleibt liegen.

## Voraussetzung

- **Claude**: Gmail oder ein anderes Mail-Postfach als Connector verbunden. Ist keiner verbunden, sag es und erkläre in einem Satz, wo man ihn verbindet (Einstellungen, Connectors).
- **ChatGPT**: Der Gmail-Connector ist in der EU, im Vereinigten Königreich und in der Schweiz bisher nicht verfügbar (Stand November 2026). Wer dort ist, kopiert die Werbemails oder Screenshots in den Chat. Nicht versprechen, was nicht geht.

## Ablauf

1. **Wunschliste klären.** Produkte oder Kategorien, die die Person wirklich sucht. Ohne Liste gibt es keine Auswahl, also danach fragen.
2. **Suchen.** Werbemails der letzten 24 Stunden (beim ersten Lauf: seit Beginn der Aktionswoche) mit Begriffen wie Black Friday, Black Week, Cyber Monday, Sale, Rabatt, Gutschein, Code. In Gmail zusätzlich die Kategorie Werbung.
3. **Auswerten.**
   - Passende Angebote: Produkt, Preis, Rabatt, Shop, Link.
   - Rabatt-Codes: Code, Shop, Bedingung (Mindestbestellwert, nur Neukunden, nur bestimmte Kategorien), Ablaufdatum. Nur Codes, die wörtlich in einer Mail stehen.
   - Die drei besten Deals des Tages mit einem Satz, warum. Ein Deal mit unklarer Rabatt-Basis ist kein bester Deal. Bei Bedarf einzelne Deals mit `deal-pruefen.md` gegenprüfen.
   - Shops, die Werbung schicken, bei denen laut Postfach im letzten Jahr nichts bestellt wurde: mit Abmelde-Link aus der Mail. Nur auflisten, nicht selbst abmelden.
4. **Kurz abgeben.** Oben eine Zeile, die als Push-Nachricht taugt, darunter die Details.

## Als tägliche Zusammenfassung

Läuft gut als geplante Aufgabe am Abend. Prompt:

```
Durchsuche mein Postfach nach Werbemails der letzten 24 Stunden
zu Black Friday, Black Week und Cyber Monday.
Meine Wunschliste: [Produkte oder Kategorien]

1. Nur Angebote, die zur Wunschliste passen: Produkt, Preis, Rabatt, Shop, Link.
2. Alle Rabatt-Codes mit Shop, Bedingung und Ablaufdatum, nur wörtlich aus den Mails.
3. Die drei besten Deals des Tages, je ein Satz warum.
4. Shops, bei denen ich laut Postfach im letzten Jahr nichts bestellt habe,
   mit Abmelde-Link. Nicht abmelden, nur auflisten.
Erste Zeile: eine kurze Zusammenfassung für die Push-Nachricht.
```

## Datenschutz

Nur Werbemails auswerten. Persönliche Mails, die bei der Suche auftauchen, nicht zusammenfassen und nicht zitieren.
