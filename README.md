<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/dzesi-dark.svg">
    <img src="assets/dzesi-light.svg" alt="dzesi" width="280">
  </picture>
</p>

# Dzesi

*Formerly Jesi.* **A free, offline editor for writing and typesetting Ewe, Twi and Ga.**

Dzesi lets you type every letter and tone mark these languages need (ɖ, ƒ, ɣ, ŋ, ɔ, ɛ, ʋ, ɛ́, ɔ̃ and the rest), keeps your text tidy so it displays and searches correctly everywhere, and exports print-ready PDFs set in Gentium Plus.

This repository holds the installers only. **[Download the latest version →](https://github.com/Psirdem/jesi-builds/releases/latest)**

---

## Download

Open the [latest release](https://github.com/Psirdem/jesi-builds/releases/latest) and choose the file for your computer:

| Computer | File | Notes |
| --- | --- | --- |
| Windows 10 or 11 (64-bit) | `Dzesi_<version>_x64_en-US.msi` | Standard Windows installer |
| Ubuntu, Debian, Linux Mint | `Dzesi_<version>_amd64.deb` | Ubuntu 22.04 or later, Debian 12 or later |
| Any other Linux (64-bit) | `Dzesi_<version>_amd64.AppImage` | Runs without installing |

A Mac version is coming later.


## Install

Dzesi isn't code-signed yet, so your computer may warn you the first time you open it. This is expected, and the steps below get you past it.

### Windows

1. Double-click the `.msi` file and follow the installer.
2. If Windows says **"Windows protected your PC"**, click **More info**, then **Run anyway**.
3. Open Dzesi from the Start menu.

Dzesi uses Microsoft Edge WebView2, which comes with Windows 11 and most up-to-date Windows 10 PCs. If it's missing, the installer downloads it once; after that, Dzesi needs no internet connection.


### Linux (.deb)

From the folder you saved the file to:

```sh
sudo apt install ./Dzesi_<version>_amd64.deb
```

Dzesi then appears in your applications menu. To remove it: `sudo apt remove dzesi`.

### Linux (.AppImage)

```sh
chmod +x Dzesi_<version>_amd64.AppImage
./Dzesi_<version>_amd64.AppImage
```

Or right-click the file, open **Properties → Permissions**, tick **Allow executing file as program**, and double-click it.

---

## What Dzesi does

### Type every letter and tone mark

- **On-screen keyboard.** The Keys panel shows your language's letters, tone marks and typographic punctuation. Click a key to type it; press ⇧ for capitals.
- **Letter shortcuts.** Type a semicolon and a letter: **;d** gives ɖ, **;D** gives Ɖ. Type **;;** for a plain semicolon.
- **Tone marks that stay put.** Click high, low or nasal to mark the letter before the cursor. **Backspace** removes marks one at a time (ɛ́ → ɛ).
- **Tidy text.** Files are saved in the standard Unicode form (NFC), so tone marks display and search reliably in other programs too.

### Find, compare and preview

- **Search that knows ɔ from o.** Find (**Ctrl+F**), replace (**Ctrl+H**) and search the whole folder (**Ctrl+Shift+F**). Searching for o never matches ɔ.
- **Go to any file** with **Ctrl+P**, split the editor side by side with **Ctrl+\\**, and preview Markdown with **Ctrl+Shift+V**.

### Export for print and the web

- **PDF, LaTeX, plain text and Markdown**, saved next to the original file.
- **Print-ready PDFs** set in Gentium Plus, with ruled tables and numbered footnotes, in A4 or US Letter.
- **LaTeX** that compiles with XeLaTeX as it is.

### Open Dzesi from any terminal

Type `dzesi` for a new window, `dzesi .` to open the folder you're in, or `dzesi notes.md` to open a file, the way `code .` opens VS Code. If a window already has it open, that window comes to the front. Installing the .deb or the Windows installer puts `dzesi` on your path.

### Several windows

**File → New Window** (Ctrl+Shift+N). Each window has its own folder, tabs, panel and terminals; settings are shared. Your windows come back the next time you open Dzesi.

### A terminal with Dzesi built in

Press **Ctrl+J** to open a terminal in your folder. The `dzesi` command lists keys (`dzesi keys ewe`), counts words and letters (`dzesi count notes.md`), tidies files (`dzesi nfc notes.md`) and exports (`dzesi export pdf notes.md`). Type `dzesi help` for the full list. Split the terminal with **Ctrl+Shift+5**, and drag the panel to the right of the window (the padlock keeps it there).

### Make it yours

Light or dark theme, text size, word wrap, PDF page size and more in **Settings** (**Ctrl+,**). Dzesi reopens your last folder with the same files and splits.


Full release notes are on each [release page](https://github.com/Psirdem/jesi-builds/releases), and inside Dzesi under **Help → What's New**.

---

## Privacy

Dzesi never connects to the internet unless you ask it to check for updates, and it asks you first. There's no account, no tracking and no telemetry. Fonts and the PDF engine are built in, and your files stay on your computer.

## Updating

From version 0.2.0, Dzesi updates itself when you ask: choose **Check for updates** in Settings, in **Help → About Dzesi**, or in the Help menu. Dzesi asks before going online, shows what's new, and installs the update with **Install and restart** once your work is saved. Updates are signed, and Dzesi refuses one that isn't.

On 0.1.0? Download the latest version from the [releases page](https://github.com/Psirdem/jesi-builds/releases) and install it over the old one, once. Your settings and files are kept. Click **Watch → Custom → Releases** at the top of this page to be told when a new version comes out.

## Problems and suggestions

If something doesn't work, or a letter or tone mark you need is missing, please [open an issue](https://github.com/Psirdem/jesi-builds/issues). Tell us your operating system, the Dzesi version (shown at the top of **Help → What's New**) and what happened.

## Licences

Dzesi includes the Gentium Plus and JetBrains Mono fonts, both under the [SIL Open Font License 1.1](https://openfontlicense.org).
