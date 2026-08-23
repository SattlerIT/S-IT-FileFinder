# 🔍 S-IT FileFinder

**Version 1.2.16 · Freeware · Windows 10 / 11 · 🇩🇪 DE · 🇬🇧 EN · 🇫🇷 FR · 🇪🇸 ES**

Ein einfaches, schnelles Suchwerkzeug für Windows – entwickelt für Menschen, die keine Erfahrung mit der Windows-Suche oder technischen Suchtools haben.

![S-IT FileFinder – Hauptfenster mit Suchergebnissen und Kontextmenü](Screenshots/1_FF-Hero_Uebersicht.png)

---

## Für wen ist dieses Tool?

Windows-Bordmittel und Tools wie *Everything* sind für erfahrene Nutzer gemacht: man muss wissen, wie man Suchoperatoren eingibt, welche Laufwerke durchsucht werden und wo man überhaupt anfängt. Für viele Anwender – besonders ältere Nutzer, Kunden im IT-Service-Alltag oder Menschen nach einem PC-Umzug – ist das eine echte Hürde.

**S-IT FileFinder** bietet stattdessen:

- **Klare, beschriftete Eingabefelder** – kein Raten, was wohin gehört
- **Laufwerke einfach anklicken** oder gezielt einen einzelnen Ordner durchsuchen
- **Suche nach Namensbruchstücken** – auch wenn nur ein Teil des Dateinamens bekannt ist
- **Datum und Dateigröße eingrenzen** – ohne Syntaxkenntnisse
- **Ergebnisse sofort nutzbar** – öffnen, sortieren, speichern, kopieren, verschieben

---

## Sprachen

Das Programm spricht vier Sprachen: **Deutsch, Englisch, Französisch und Spanisch.** Die Sprache wird im Konfig-Dialog gewählt; nach einer kurzen Rückfrage startet FileFinder in der gewählten Sprache neu. Übersetzt sind die Oberfläche, das Kontextmenü, alle Meldungen, der Ergebnis-Manager, das Fenster für Dateiaktionen und der HTML-Ergebnisbericht.

Zu jeder Sprache gehören eine eigene Hilfeseite und ein eigener Änderungsverlauf:

| Sprache | Hilfe | Änderungsverlauf |
|---|---|---|
| 🇩🇪 Deutsch | [Hilfe & Dokumentation](S-IT-FileFinder-Hilfe.html) | [Änderungsverlauf](CHANGELOG.md) |
| 🇬🇧 English | [Help & documentation](S-IT-FileFinder-Help.html) | [Changelog](CHANGELOG-en.md) |
| 🇫🇷 Français | [Aide & documentation](S-IT-FileFinder-Aide.html) | [Journal des modifications](CHANGELOG-fr.md) |
| 🇪🇸 Español | [Ayuda y documentación](S-IT-FileFinder-Ayuda.html) | [Registro de cambios](CHANGELOG-es.md) |

Dateinamen bleiben in jeder Sprache gleich – gespeicherte Suchen und Einstellungen bleiben nach einem Sprachwechsel unverändert erhalten.

---

## Funktionen

### Suchkriterien

| Feld | Beschreibung |
|---|---|
| **Dateiname enthält** | Ein oder mehrere Bruchstücke, durch Leerzeichen getrennt (UND-Verknüpfung) |
| **Dateityp / Endung** | z. B. `jpg`, `.pdf`, `docx` – mit oder ohne Punkt |
| **Nur Ordner** | Einen bestimmten Ordner samt Unterordnern durchsuchen statt ganzer Laufwerke |
| **Erstellt von / bis** | Datum im Format `TT.MM.JJJJ` |
| **Geändert von / bis** | Datum im Format `TT.MM.JJJJ` |
| **Größe mind. / höchstens** | In Megabyte – beide Felder optional |

Alle Felder sind optional und frei kombinierbar. Die erweiterten Filter für Datum und Größe lassen sich mit **F11** ein- und ausklappen.

### Suchbereich

Alle erkannten Laufwerke (lokal und eingebundene Netzlaufwerke) erscheinen automatisch als Checkboxen; mit **„Alle"** werden sie auf einmal an- oder abgehakt. Alternativ wird über das Feld **„Nur Ordner"** gezielt ein einzelner Ordner samt Unterordnern durchsucht – die Laufwerksauswahl ist währenddessen deaktiviert und kehrt beim Leeren des Feldes zurück.

### Ergebnistabelle

- **Klick auf die Spaltenüberschrift** → sortieren nach Name, Größe, Datum oder Pfad (nach echtem Wert, nicht nach angezeigtem Text)
- **Doppelklick** → Ordner im Explorer öffnen, Datei markiert
- **Rechtsklick** → Kontextmenü: Ordner öffnen, Datei öffnen, Pfad kopieren

### Große Dateien

Auf Knopfdruck die 100 größten Dateien der gewählten Laufwerke oder des gewählten Ordners anzeigen – zum schnellen Aufspüren von Speicherfressern.

### Dateiaktionen

Mehrere Treffer markieren und in einem eigenen Fenster **kopieren, verschieben oder in den Papierkorb legen** – mit Byte-genauem Fortschrittsbalken und ohne Überschreiben (bei Namensgleichheit wird automatisch umbenannt).

### Ergebnisse speichern & Ergebnis-Manager

Suchergebnisse speichern, später wieder laden oder als **HTML-Bericht** ansehen – Dateinamen und Pfade sind dort direkt anklickbar. Verwaltet wird alles im Ergebnis-Manager; gespeicherte Suchen lassen sich einzeln oder nach Zeitraum löschen.

### Konfiguration

Zentraler Dialog für Sprache, Darstellungsgröße (90–200 %), erweiterte Filter beim Start und Standard-Sortierung. Die Einstellungen stehen in `Config\FileFinder-config.ini`.

---

## Download & Installation

Die aktuelle Version als kompilierte Windows-EXE steht auf der **[Releases-Seite](../../releases)** bereit: `s-it-filefinder_latest.zip`.

Keine Installation notwendig: ZIP entpacken, den Ordner an einen beliebigen Ort legen und `S-IT-FileFinder.exe` starten. Der Programmordner sieht so aus:

```
S-IT-FileFinder\
├── S-IT-FileFinder.exe
├── _internal\        Laufzeitdateien
├── Lang\             Sprachpakete
├── Help\             Hilfe und Änderungsverlauf in vier Sprachen
├── License\          Lizenz und Haftungsausschluss
└── Config\           Einstellungen (wird beim ersten Speichern angelegt)
```

Die Unterordner gehören zum Programm und müssen bei der EXE bleiben. Die Hilfe wird über den **„? Hilfe"**-Knopf im Programm geöffnet – in der eingestellten Sprache.

---

## Technische Hinweise

- Entwickelt mit Python und tkinter, kompiliert mit PyInstaller (`--onedir`)
- DPI-Unterstützung für HiDPI-Monitore, Darstellungsgröße 90–200 % einstellbar
- Suche läuft im Hintergrund-Thread, das Fenster bleibt jederzeit bedienbar
- Windows-Systemordner (`Windows`, `$Recycle.Bin` u. a.) werden im Wurzelverzeichnis der Laufwerke übersprungen – Suchen über das Systemlaufwerk laufen dadurch deutlich schneller
- Gesperrte Ordner werden ohne Absturz übersprungen, die Anzahl erscheint in der Statuszeile
- Keine Administratorrechte erforderlich

---

## Unterstützung / Spende

S-IT FileFinder ist kostenlos und ohne Einschränkungen nutzbar.
Wer das Tool nützlich findet, darf mich gern über PayPal unterstützen:

**[tool-entwicklung@sattler-it.de](mailto:tool-entwicklung@sattler-it.de)**

---

## Weitere Tools

Weitere Freeware-Tools von Sattler IT-Service:

- **[S-IT-3Kopier](https://sattlerit.github.io/S-IT-3Kopier/)** – Dreifach-Kopierer mit Protokoll und Zeitsteuerung, ebenfalls in vier Sprachen
- **[S-IT LAN Device Scanner](https://www.wintotal.de/download/s-it-lan-device-scanner/)** – Netzwerkgeräte scannen, identifizieren und dokumentieren
- **[Tool-Übersicht](https://sattlerit.github.io/sattlerit-tools/)** – alle Tools auf einen Blick

---

## Lizenz

© 2026 Sattler IT-Service, Greifenstein
Autor: Hans Udo Sattler

Freeware – kostenlose Nutzung und Weitergabe erlaubt.
Kommerzielle Weiterverwendung oder Modifikation ohne Genehmigung nicht gestattet.
