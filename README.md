🇩🇪 [Diese Seite auf Deutsch](README_DE.md)

# 🔍 S-IT FileFinder

**Version 2.0 · Freeware · Windows 10 / 11 · 18 languages**

A simple, fast search tool for Windows – made for people who have no experience with Windows search or technical search tools.

![S-IT FileFinder – main window with sidebar and search results](Screenshots/1_FF-Hero_Uebersicht.png)

---

## Who is this tool for?

Windows search and many search programs require experience: you need to know how to enter search terms, which drives are searched and where to start in the first place. For many users – especially older users, customers in everyday IT service or people after moving to a new PC – that is a real hurdle.

**S-IT FileFinder** offers instead:

- **Clear, labelled input fields** – no guessing what goes where
- **Simply click the drives** or search one specific folder
- **Search by parts of a name** – even if only part of the file name is known
- **Narrow down by date and file size** – without any syntax
- **Results ready to use** – open, sort, save, copy, move

---

## Interface

On the left is a sidebar with **Search**, **Large files**, **Results Manager**, **Settings** and **Help**. To its right, search criteria, drives and folder sit in separate boxes with their own background colours, with the result list below. **“Clear fields”** at the top right resets the view.

Five colour schemes are available: Standard, Soft light, Muted (default), Strongly muted and Dark.

---

## Features

### Search criteria

| Field | Description |
|---|---|
| **File name contains** | One or more fragments, separated by spaces (AND search) |
| **File type / extension** | e.g. `jpg`, `.pdf`, `docx` – with or without the dot |
| **Created from / to** | Date in the format `DD.MM.YYYY` |
| **Modified from / to** | Date in the format `DD.MM.YYYY` |
| **Size min. / max.** | In megabytes – both fields optional |

All fields are optional and can be combined freely. The advanced filters for date and size are shown or hidden with **F11**.

### Search scope

All detected drives (local and mapped network drives) appear automatically as check boxes; **“All”** checks or unchecks them at once. Alternatively, the **“Folder only”** field limits the search to one specific folder – the drive selection is disabled meanwhile and returns when the field is cleared.

**“Include subfolders”** sets whether the subfolders are searched as well or only the files directly in the folder. If the file you are looking for is directly in that folder, the search finishes considerably faster.

### Result list

- **Click a column heading** → sort by name, size, date or path (by the real value, not the displayed text)
- **Double-click** → open the folder in Explorer with the file selected
- **Right-click** → context menu: open folder, open file, copy path, file actions

### Large files

A view of its own in the sidebar shows the 100 largest files on the selected drives or in the selected folder at the push of a button – to track down space hogs quickly. The view has its own result list; the hits of the normal search are kept when you switch.

![S-IT FileFinder – Large files view](Screenshots/5_FF-GrosseDateien.png)

### File actions

Select several hits and **copy them, move them or send them to the Recycle Bin** in a separate window – with a byte-accurate progress bar and without overwriting (automatic renaming if a name already exists).

### Saving results & Results Manager

Save search results, load them again later or view them as an **HTML report** – file names and paths there are directly clickable. Everything is managed in the Results Manager; saved searches can be deleted one by one or by date range.

### Settings

Central dialog for display size (90–200 %), advanced filters at startup, default sorting, language and colour scheme. The selected display size applies regardless of the scaling set in Windows. The settings are stored in `Config\FileFinder-config.ini`.

---

## Languages

The program speaks 18 languages: **German, English, French, Spanish, Italian, Dutch, Polish, Danish, Croatian, Bosnian, Serbian, Montenegrin, Slovenian, Albanian, Romanian, Turkish, Bulgarian and Macedonian.** The language is chosen in the settings via a selection window; after a short confirmation, FileFinder restarts in the language you chose. Translated are the interface, all messages, the Results Manager, the window for file actions and the HTML result report.

The help is available in four languages; for all other languages the program opens the English version:

- 🇩🇪 [Hilfe & Dokumentation](https://sattlerit.github.io/S-IT-FileFinder/S-IT-FileFinder-Hilfe.html)
- 🇬🇧 [Help & documentation](https://sattlerit.github.io/S-IT-FileFinder/S-IT-FileFinder-Help.html)
- 🇫🇷 [Aide & documentation](https://sattlerit.github.io/S-IT-FileFinder/S-IT-FileFinder-Aide.html)
- 🇪🇸 [Ayuda y documentación](https://sattlerit.github.io/S-IT-FileFinder/S-IT-FileFinder-Ayuda.html)

Changelog: 🇬🇧 [English](https://sattlerit.github.io/S-IT-FileFinder/S-IT-FileFinder-Changelog-en.html) · 🇩🇪 [Deutsch](https://sattlerit.github.io/S-IT-FileFinder/S-IT-FileFinder-Changelog.html)

File names stay the same in every language – saved searches and settings are kept unchanged after a language change.

---

## Download & installation

The current version is available on the **[Releases page](../../releases)**: `s-it-filefinder_latest.zip`.

No installation needed: unpack the ZIP, put the folder anywhere you like and start `S-IT-FileFinder.exe`. The program folder looks like this:

```
S-IT-FileFinder\
├── S-IT-FileFinder.exe
├── _internal\        runtime files
├── Lang\             language packs
├── Help\             help and changelog
├── License\          licence and disclaimer
└── Config\           settings (created when first saved)
```

The subfolders belong to the program and must stay with the EXE. The help is opened via **“Help”** in the sidebar – in the language that is set.

---

## Technical notes

- Display size 90–200 %, regardless of Windows scaling; the window stays above the taskbar
- The search runs in the background; the window stays usable at all times
- Windows system folders (`Windows`, `$Recycle.Bin` and others) are skipped in the root of each drive – searches across the system drive are noticeably faster as a result
- Locked folders are skipped; their number appears in the status line
- No administrator rights required

---

## Support / donation

S-IT FileFinder is free and can be used without restrictions.
If you find the tool useful, you are welcome to support me via PayPal:

**[tool-entwicklung@sattler-it.de](mailto:tool-entwicklung@sattler-it.de)**

---

## More tools

More freeware tools from Sattler IT-Service:

- **[S-IT-3Kopier](https://sattlerit.github.io/sit-3kopier/)** – triple copier with log and scheduling, also multilingual
- **[S-IT LAN Device Scanner](https://www.wintotal.de/download/s-it-lan-device-scanner/)** – scan, identify and document network devices
- **[Tool overview](https://sattlerit.github.io/sattlerit-tools/)** – all tools at a glance

---

## Licence

© 2026 Sattler IT-Service, Greifenstein
Author: Hans Udo Sattler

Freeware – free use and redistribution permitted.
Commercial reuse or modification without permission is not allowed.
