# Jesi

**A free, offline editor for writing and typesetting Ewe, Twi and Ga.**

Jesi lets you type every letter and tone mark these languages need (ɖ, ƒ, ɣ, ŋ, ɔ, ɛ, ʋ, ɛ́, ɔ̃ and the rest), keeps your text tidy so it displays and searches correctly everywhere, and exports print-ready PDFs set in Gentium Plus.

This repository holds the installers only. **[Download the latest version →](https://github.com/Psirdem/jesi-builds/releases/latest)**

---

## Download

Open the [latest release](https://github.com/Psirdem/jesi-builds/releases/latest) and choose the file for your computer:

| Computer | File | Notes |
| --- | --- | --- |
| Windows 10 or 11 (64-bit) | `Jesi_<version>_x64_en-US.msi` | Standard Windows installer |
| Mac with Apple silicon (M1 and later) | `Jesi_<version>_aarch64.dmg` | |
| Mac with an Intel processor | `Jesi_<version>_x64.dmg` | |
| Ubuntu, Debian, Linux Mint | `Jesi_<version>_amd64.deb` | Ubuntu 22.04 or later, Debian 12 or later |
| Any other Linux (64-bit) | `Jesi_<version>_amd64.AppImage` | Runs without installing |

Not sure which Mac you have? Open the Apple menu → **About This Mac**. If it says **Chip: Apple M…**, choose Apple silicon; if it says **Processor: Intel**, choose Intel.

## Install

Jesi isn't code-signed yet, so your computer may warn you the first time you open it. This is expected, and the steps below get you past it.

### Windows

1. Double-click the `.msi` file and follow the installer.
2. If Windows says **"Windows protected your PC"**, click **More info**, then **Run anyway**.
3. Open Jesi from the Start menu.

Jesi uses Microsoft Edge WebView2, which comes with Windows 11 and most up-to-date Windows 10 PCs. If it's missing, the installer downloads it once; after that, Jesi needs no internet connection.

### macOS

1. Open the `.dmg` file and drag **Jesi** into **Applications**.
2. Open Jesi from Applications. If macOS says it can't check Jesi for malicious software, click **Done**.
3. Open **System Settings → Privacy & Security**, scroll down, and click **Open Anyway** next to the message about Jesi. Confirm with your password.

You only need to do this once.

### Linux (.deb)

From the folder you saved the file to:

```sh
sudo apt install ./Jesi_<version>_amd64.deb
```

Jesi then appears in your applications menu. To remove it: `sudo apt remove jesi`.

### Linux (.AppImage)

```sh
chmod +x Jesi_<version>_amd64.AppImage
./Jesi_<version>_amd64.AppImage
```

Or right-click the file, open **Properties → Permissions**, tick **Allow executing file as program**, and double-click it.

---

## What Jesi does

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

### A terminal with Jesi built in

Press **Ctrl+J** to open a terminal in your folder. The `jesi` command lists keys (`jesi keys ewe`), counts words and letters (`jesi count notes.md`), tidies files (`jesi nfc notes.md`) and exports (`jesi export pdf notes.md`). Type `jesi help` for the full list.

### Make it yours

Light or dark theme, text size, word wrap, PDF page size and more in **Settings** (**Ctrl+,**). Jesi reopens your last folder with the same files and splits.

On a Mac, use **⌘** wherever these notes say **Ctrl**.

Full release notes are on each [release page](https://github.com/Psirdem/jesi-builds/releases), and inside Jesi under **Help → What's New**.

---

## Privacy

Jesi never connects to the internet. There's no account, no tracking and no telemetry. Fonts and the PDF engine are built in, and your files stay on your computer.

## Updating

Jesi doesn't update itself yet. To get a new version, download it from the [releases page](https://github.com/Psirdem/jesi-builds/releases) and install it over the old one. Your settings and files are kept. Click **Watch → Custom → Releases** at the top of this page to be told when a new version comes out.

## Problems and suggestions

If something doesn't work, or a letter or tone mark you need is missing, please [open an issue](https://github.com/Psirdem/jesi-builds/issues). Tell us your operating system, the Jesi version (shown at the top of **Help → What's New**) and what happened.

## Licences

Jesi includes the Gentium Plus and JetBrains Mono fonts, both under the [SIL Open Font License 1.1](https://openfontlicense.org).
