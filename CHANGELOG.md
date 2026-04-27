# S-IT FileFinder – Änderungshistorie

## v1.2.0 (April 2026)

### Neu
- **Erweiterte Filter (F11):** Datum- und Größenfelder lassen sich per Taste F11 oder
  Schaltfläche ein- und ausklappen. Das Fenster passt seine Höhe automatisch an.
  Beim Programmstart sind die erweiterten Filter ausgeblendet, der Zustand wird gespeichert.
- **Ansicht-Schaltfläche:** Neue Schaltfläche 🖥️ Ansicht in der Kopfleiste zur Auswahl
  der Darstellungsgröße (100 % / 125 % / 150 % / 175 % / 200 % / Automatisch).
  Nach Änderung kann das Programm auf Wunsch sofort neu gestartet werden.
- **DPI-Skalierung:** Vollständige Unterstützung für UHD/4K-Bildschirme und
  Windows-Skalierungen ab 100 %. Schriften, Abstände und Spaltenbreiten passen
  sich automatisch an die Bildschirmauflösung an.
- **Automatische Fensterbreite:** Das Fenster verbreitert sich beim Start automatisch,
  wenn viele Laufwerksbuchstaben vorhanden sind, damit alle Checkboxen sichtbar bleiben.
- **Verbesserte Datumsbeschriftungen:** „📅 Erstellt" und „✏️ Geändert" mit erklärendem
  Hinweistext direkt in der Oberfläche.

### Verbessert
- Header neu gestaltet: Versionsnummer links neben dem Titel, Schaltflächen rechts
  mit großzügigem Abstand.
- Startgröße und -position werden automatisch an die verfügbare Bildschirmfläche
  angepasst (max. 95 % Breite, 92 % Höhe, Position nahe oberer Bildschirmrand).
- Konfigurationsdatei `FileFinder-config.json` speichert den Zustand der erweiterten Filter.
- Konfigurationsdatei `FileFinder-config.ini` speichert die Ansichts-Skalierung.

---

## v1.0.1 (März 2026)

### Behoben
- Icon-Setzung im Hintergrund verzögert, um Einfrieren beim Start auf Systemen mit
  Netzlaufwerken oder Kartenlesern zu vermeiden.

---

## v1.0.0 (März 2026)

Erste Veröffentlichung als Freeware.

### Funktionen
- Dateisuche nach Name (mehrere Bruchstücke, Leerzeichen-getrennt), Dateityp/Endung,
  Erstelldatum, Änderungsdatum und Dateigröße
- Gleichzeitige Suche auf mehreren Laufwerken mit „Alle"-Checkbox
- Automatische Laufwerkserkennung ohne Blockieren (GetLogicalDrives-API)
- Ergebnistabelle mit Doppelklick (Explorer) und Rechtsklick-Kontextmenü
  (Ordner öffnen, Datei öffnen, Pfad kopieren, Kopieren/Verschieben)
- Suchergebnis als HTML-Datei speichern und öffnen
- Fortschrittsbalken und Statuszeile mit Trefferanzahl
- Systemordner auf C:\ werden automatisch übersprungen
- Vollständige DPI-Awareness (SetProcessDpiAwareness)
- ESC beendet das Programm
