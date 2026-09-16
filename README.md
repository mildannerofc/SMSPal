# SMSPal

SMSPal is a browser-based viewer and editor for palettes stored in Sega Master System ROM files. Inspired by HivePal, it helps you inspect SMS VDP colors, locate palette data, edit individual color entries, and export modified ROM data directly from your browser.

## Features

- Load `.sms` and `.bin` ROM files locally.
- View ROM bytes as Master System palette colors.
- Inspect the complete 64-color SMS VDP palette.
- Edit colors using the color picker, HEX values, or SMS color bytes.
- Rotate or reverse palette entries.
- Navigate to offsets using hexadecimal or decimal notation.
- Configure colors per row, palette rows, layout, display size, and theme.
- View generated assembly-style `.db $XX` output for the selected palette.
- Save the edited ROM or save it under a new filename.

## Requirements

SMSPal is a standalone HTML application and has no external dependencies or build process. You only need:

- A modern web browser with JavaScript enabled.
- A local copy of this repository.

## Clone the repository

Clone SMSPal with Git:

```bash
git clone https://github.com/mildannerofc/SMSPal.git
cd SMSPal
```

Alternatively, download the repository as a ZIP file from GitHub and extract it locally.

## Installation and usage

There is nothing to install with a package manager. SMSPal runs directly from `index.html`.

### Option 1: Open the file directly

Open `index.html` in a modern web browser.

### Option 2: Run a local web server

Running a local server is recommended for a more consistent browser experience. If Python is installed, run:

```bash
python3 -m http.server 8000
```

Then open the following address in your browser:

```text
http://localhost:8000
```

To use the application, click **Carregar ROM** and select an SMS-compatible `.sms` or `.bin` file. After making changes, use **Salvar** or **Salvar como...** to download the edited data.

> **Important:** Always keep a backup of your original ROM before editing. SMSPal modifies data in memory and cannot undo changes after an exported file has been downloaded.

## AI disclosure

Parts of this project, including code, documentation, or development assistance, may have been created or refined with the help of artificial intelligence tools. All AI-assisted output was reviewed and adapted by the project author. The author remains responsible for the final contents, behavior, and maintenance of this repository.

## Disclaimer

SMSPal is provided for educational, preservation, and development purposes. Use it only with ROM files that you own or are legally authorized to modify. The project is not affiliated with, endorsed by, or sponsored by Sega or the creators of HivePal. The author is not responsible for data loss, damaged files, or any consequences resulting from the use of this software.

## License

No license has been specified for this repository yet. Until a license is added, all rights are reserved by the copyright holder.
