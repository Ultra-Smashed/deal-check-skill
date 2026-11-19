# Preiswächter

Überwacht eine Wunschliste bis zu einem Stichtag und meldet sich nur, wenn ein Preis unter die Grenze fällt. Läuft als geplante Aufgabe.

## Ablauf

1. **Wunschliste aufnehmen.** Pro Produkt: genaue Bezeichnung mit Variante und Höchstpreis in Euro. Fehlt der Höchstpreis, schlag einen vor (niedrigster belegter Preis der letzten drei Monate, siehe `deal-pruefen.md`) und lass ihn bestätigen. Höchstens zehn Produkte, sonst wird jeder Lauf langsam.
2. **Stichtag festlegen.** Standard: Cyber Monday. Danach soll die Aufgabe enden.
3. **Einmal sofort prüfen**, damit die Person den Stand von heute kennt.
4. **Geplante Aufgabe einrichten.**
   - **Claude** (bezahlte Pläne): Wenn du geplante Aufgaben anlegen kannst, richte sie selbst ein, täglich am Morgen, mit dem Prompt unten. Sonst den Weg erklären: in der Seitenleiste **Scheduled** öffnen, neue Aufgabe, Prompt einfügen, täglich.
   - **ChatGPT** (alle Tarife, kostenlos bis zu drei aktive Aufgaben): in der Seitenleiste **Geplant** bzw. **Scheduled** öffnen oder im Chat schreiben „Führ das jeden Morgen um 8 Uhr aus“. In eigenen GPTs gehen geplante Aufgaben nicht, also in einem normalen Chat anlegen.
5. **Benachrichtigungen** für die App am Handy einschalten lassen, sonst kommt der Treffer nicht an.

## Prompt für die geplante Aufgabe

Mit der Liste der Person ausfüllen und so übergeben:

```
Du bist mein Preiswächter bis [Stichtag].

Meine Wunschliste (Produkt mit Variante · Höchstpreis):
- [Produkt 1] · [Preis] €
- [Produkt 2] · [Preis] €

Bei jedem Lauf:
1. Such für jedes Produkt den günstigsten aktuellen Endpreis inklusive Versand
   bei seriösen Shops in Deutschland. Gleiche Variante, Neuware.
2. Schau dir den Preisverlauf der letzten 30 Tage bei einem Preisvergleichsportal an.
3. Melde dich nur, wenn ein Preis unter meinem Höchstpreis liegt:
   Produkt, Preis, Shop, Link, Stand.
4. Wurde ein Preis in den letzten 14 Tagen erhöht und wird jetzt als Rabatt
   beworben, schreib das dazu.
5. Trifft nichts davon zu, antworte nur „Keine Treffer“.
Erfinde keine Preise. Was du nicht findest, lässt du weg.
Nach dem [Stichtag] erinnere mich, diese Aufgabe zu löschen.
```

## Grenzen offen sagen

- Die Aufgabe sieht nur, was öffentlich im Netz steht. Preise hinter Login, in Apps oder nur im Warenkorb sieht sie nicht.
- Blitzangebote, die nur wenige Stunden laufen, kann ein täglicher Lauf verpassen.
- Geplante Aufgaben laufen in ChatGPT höchstens einmal pro Stunde. Für Black Friday reicht einmal am Morgen.
