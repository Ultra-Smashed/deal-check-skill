# Deal-Check-Skill

Ein Skill für Claude, auch für ChatGPT nutzbar. Du schickst einen Link oder Screenshot von einem Angebot, und der Deal-Check prüft den Preisverlauf, rechnet die echte Ersparnis aus, vergleicht andere Shops mit Versandkosten, testet Gutscheincodes im Warenkorb und sagt dir am Ende klar: kaufen, warten oder lassen. Mit Zielpreis und, wenn es eine gibt, einer günstigeren Alternative. Kostenlos, MIT-Lizenz.

| Modul | Was es macht |
| --- | --- |
| **Deal prüfen** | Produkt genau bestimmen, Preisverlauf der letzten Monate, Rabatt-Basis (UVP oder echter früherer Preis), Shop-Vergleich inklusive Versand, Seriositäts-Check bei unbekannten Shops und ein Urteil mit Belegen. |
| **Gutscheine** | Sucht Gutscheincodes für den günstigsten Shop (Shop, Postfach, Deal-Communities) und probiert sie mit einem Browser-Werkzeug im Warenkorb aus. Am Ende steht der echte Endpreis mit dem besten Code. Bestellt wird nie. |
| **Preiswächter** | Deine Wunschliste mit Höchstpreisen als geplante Aufgabe. Meldet sich nur, wenn ein Preis unter deine Grenze fällt, und wenn ein Shop den Preis vor der Aktion erhöht hat. |
| **Postfach-Deals** | Durchsucht Werbemails nach Angeboten, die zu deiner Wunschliste passen, sammelt Rabatt-Codes mit Ablaufdatum und nennt die drei besten Deals des Tages. |
| **Kauf-Check** | Fünf ehrliche Fragen, eine nach der anderen, dann ein Urteil, ob du es wirklich brauchst. |

## Installation

### Claude-App (Web, Desktop)

Am schnellsten: den Link in einen neuen Chat einfügen und Claude bitten, den Skill zu installieren:

```
https://github.com/Ultra-Smashed/deal-check-skill

Installier diesen Skill für mich.
```

Oder von Hand:

1. [`deal-check.zip`](https://github.com/Ultra-Smashed/deal-check-skill/raw/main/deal-check.zip) herunterladen (nicht entpacken).
2. In Claude unter **Settings → Capabilities** den Schalter **Code execution and file creation** einschalten. In der neueren Ansicht heißt er **Create and edit files**.
3. **Customize → Skills** öffnen, auf **+** klicken, dann **Create skill → Upload a skill** und die ZIP-Datei wählen.

Als Plugin: **Customize → Plugins**, bei den persönlichen Plugins auf **+**, dann **Add from a repository** und `Ultra-Smashed/deal-check-skill` eintragen.

Die Menünamen stehen hier so, wie Anthropic sie in der Hilfe nennt. In der deutschen Oberfläche können sie übersetzt sein. Für Preise braucht Claude die Websuche.

### Claude Code

Als Plugin:

```
/plugin marketplace add Ultra-Smashed/deal-check-skill
/plugin install deal-check@deal-check
```

Oder den Ordner kopieren:

```bash
git clone https://github.com/Ultra-Smashed/deal-check-skill.git
cp -r deal-check-skill/skills/deal-check ~/.claude/skills/
```

### ChatGPT

Als Projekt mit Anweisungen oder als eigener GPT. Anleitung und der Text zum Einfügen: [`chatgpt/`](chatgpt/README.md).

## Benutzen

> Lohnt sich dieser Deal? https://…

> [Screenshot einer Produktseite] Kaufen oder warten?

> Gibt es für diesen Warenkorb noch einen Gutscheincode? Probier sie aus.

> Überwach meine Wunschliste bis Cyber Monday: Kopfhörer X unter 160 €, Saugroboter Y unter 300 €.

> Ich überlege, mir das zu kaufen. Brauche ich das überhaupt?

## Dateien

```
skills/deal-check/SKILL.md          Ablauf, Module, Regeln
skills/deal-check/modes/            eine Anleitung pro Modul (deal-pruefen, gutscheine, preiswaechter, postfach, kauf-check)
chatgpt/anweisungen.txt             dieselben Module als Anweisungen für ChatGPT
deal-check.zip                      der Skill-Ordner als ZIP für die Claude-App
.claude-plugin/                     plugin.json, marketplace.json
```

Nach einer Änderung im Skill-Ordner die ZIP neu bauen: `cd skills && zip -r ../deal-check.zip deal-check`.

## Hinweise

**Keine Gewähr.** Preise ändern sich in der Black Week stündlich, und Preisportale sind nicht immer aktuell. Der Skill nennt zu jedem Preis Quelle und Abrufzeit. Es gilt der Preis im Warenkorb des Shops.

**Keine Rechts- oder Finanzberatung.** Hinweise zur Preisangabenverordnung oder zum Widerrufsrecht sind eine Einordnung, keine Beratung.

**Nichts wird gekauft.** Der Skill bestellt nichts, meldet dich nirgends an oder ab und verschickt nichts. Zum Testen von Gutscheincodes legt er nach deinem Okay ein Produkt in den Warenkorb. Weiter als bis zum Warenkorb geht er nie, Adresse und Zahlungsdaten gibt er nicht ein. Das Ausprobieren braucht ein Browser-Werkzeug, zum Beispiel Claude in Chrome. Ohne Browser bekommst du die Codes als ungetestete Liste.

**Postfach.** Beim Modul Postfach-Deals liest die KI deine Werbemails. Persönliche Mails werden nicht zusammengefasst. Sieh in den Einstellungen deines Kontos nach, ob deine Chats zur Verbesserung der Modelle genutzt werden dürfen.

Anleitung: [thanisch.co/wissen/guides/deal-check-skill](https://thanisch.co/wissen/guides/deal-check-skill)

MIT-Lizenz, siehe [LICENSE](LICENSE). Von [Christopher Thanisch](https://thanisch.co).
