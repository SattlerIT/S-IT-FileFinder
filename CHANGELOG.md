# Changelog – S-IT FileFinder

Alle nennenswerten Änderungen an S-IT FileFinder, neueste Version oben.
Die Versionen 1.2.5–1.2.11 waren interne Zwischenschritte und sind in v1.2.12 zusammengefasst.

## v1.2.15 – Start-Knopf, Suchbereich im Bericht & Webseiten-Link

- **Start-Knopf:** Neue Schaltfläche „🏠 Start" in der Kopfleiste – bringt das Programm jederzeit zurück zur leeren Startansicht, auch aus einem geladenen Ergebnis oder der Ansicht „Große Dateien" heraus.
- **Suchbereich im Bericht:** Bei einer Ordnersuche zeigen Ergebnisbericht und Ergebnis-Manager jetzt den durchsuchten Ordnerpfad an (Angabe heißt nun „Suchbereich" statt „Laufwerke"). Beim Laden einer gespeicherten Ordnersuche wird der Ordner wieder ins Feld „Nur Ordner" übernommen.
- **Webseiten-Link:** Neuer Link „🌐 Webseite" in der Fußzeile – öffnet die FileFinder-Projektseite im Browser.
- Umsetzung von Nutzervorschlägen aus der Praxis – danke dafür!

## v1.2.14 – Ordnersuche, schnellere Laufwerkssuche & 90-%-Skalierung

- **Ordnersuche:** Über das neue Feld „Nur Ordner" wird gezielt ein bestimmter Ordner samt Unterordnern durchsucht statt ganzer Laufwerke – gilt auch für „Große Dateien". Die Laufwerksauswahl wird währenddessen deaktiviert; beim Leeren des Felds kehrt die vorherige Auswahl automatisch zurück.
- **Schnellere Laufwerkssuche:** Der Ausschluss der Windows-Systemordner (Windows, $Recycle.Bin, System Volume Information u. a.) im Wurzelverzeichnis der Laufwerke greift jetzt zuverlässig – Suchen über das Systemlaufwerk laufen dadurch spürbar schneller und liefern keine Treffer mehr aus den Systemordnern.
- **Skalierung ab 90 %:** Neue 90-%-Stufe im Konfig-Dialog für kompaktere Darstellung auf kleineren Bildschirmen.
- **Hilfe überarbeitet:** Neuer Abschnitt zum Suchbereich (Ordner oder Laufwerke), zusätzlicher Praxis-Tipp zur gezielten Ordnersuche.
- Lizenz und Haftungsausschluss (Disclaimer) liegen dem Paket jetzt bei.

## v1.2.12 – Sortierung, Große Dateien, Dateiaktionen & Ergebnis-Manager

- **Sortierung:** Treffer per Klick auf die Spaltenüberschrift sortieren (Name, Größe, Datum, Pfad). Größe und Datum werden nach echtem Wert sortiert, nicht nach angezeigtem Text.
- **Große Dateien:** Auf Knopfdruck die 100 größten Dateien der gewählten Laufwerke anzeigen – zum schnellen Aufspüren von Speicherfressern.
- **Dateiaktionen:** Mehrere Treffer markieren und im eigenen Fenster kopieren, verschieben oder in den Papierkorb legen – mit Byte-genauem Fortschrittsbalken und ohne Überschreiben (automatische Umbenennung bei Namensgleichheit).
- **Ergebnisse speichern:** Suchergebnisse speichern, später wieder laden oder als HTML-Bericht ansehen – verwaltet im neuen Ergebnis-Manager.
- **Konfiguration:** Zentraler Dialog für Darstellungsgröße, erweiterte Filter beim Start und Standard-Sortierung (gespeichert in `FileFinder-config.ini`).
- Aktualisierte Hilfe-Datei und zahlreiche Detailverbesserungen.

## v1.2.4 – 2026-04-16 – Stabiler Neustart

- **Neustart-Fix:** Die DPI-Umschaltung startet die neue Instanz zuverlässig ohne „Failed to import encodings“; die kompilierte EXE wird direkt gestartet.
- **--onedir:** Umstellung auf ordnerbasierte EXE – kein Entpacken in Temp beim Start.
- Neustart-Verzögerung (200 ms) verhindert eine Race Condition beim Schließen.

## v1.2.3 – Layout erweiterte Filter

- Verständlichere Bezeichnungen: „Erstelldatum“ und „Änderungsdatum“.
- Einheitliche Symbole (📅 📏 ✏️), bündig untereinander.
- Von/bis-Felder dichter beieinander, Labels linksbündig.

## v1.2.1 – Größenangaben in MB

- Größenfilter arbeitet in Megabyte statt Kilobyte.
- Maximalgröße erkennt automatisch MB oder GB im HTML-Ergebnislog.

## v1.2.0 – Ansicht & erweiterte Filter

- F11-Umschalter für Datum- und Größenfilter; die Fensterhöhe passt sich automatisch an.
- Darstellungsgröße wählbar (100–200 %) mit optionalem Programm-Neustart.
- Vollständige DPI-/4K-Skalierung für hochauflösende Bildschirme.
- Automatische Fensterbreite bei vielen Laufwerksbuchstaben.
- Verbesserte Datumsbeschriftungen, überarbeiteter Header, automatische Startgröße und -position.

## v1.0.1 – Bugfix Startverhalten

- Einfrieren beim Start auf Systemen mit DVD-Laufwerk oder Kartenleser ohne eingelegtes Medium behoben (Laufwerke werden über die Windows-API ermittelt).

## v1.0.0 – Erstveröffentlichung

- Suche nach Namensbruchstücken, Dateityp, Erstell-/Änderungsdatum und Dateigröße.
- Multi-Laufwerk-Unterstützung mit Alle-Checkbox.
- HTML-Ergebnislog mit klickbaren Pfaden.
- Kontextmenü: Ordner öffnen, Datei öffnen, Pfad kopieren.
- Hilfe-Button mit HTML-Dokumentation.
