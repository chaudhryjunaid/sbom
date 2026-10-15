# GUI software inventory

GUI apps installed on top of a stock **Ubuntu 26.04.1 LTS (GNOME)** desktop.
Apps that ship with the default install are left out.

- **Taken:** 2026-10-15
- **Base image:** Ubuntu 26.04 "Resolute Raccoon" amd64 (20260423.1)
- **Total:** 41 apps

## Quick list

```
alacritty, bruno, chatgpt, claude, cpu-x, dadroit json viewer, draw.io, duplicati, extension manager, fedora media writer, foldersync desktop, foliate, gear lever, genius, gnome boxes, gnome package updater, gnome tweaks, google chrome, google chrome beta, gramps, hardinfo2, insync, kitty, kopiaui, master pdf editor 5, mission center, mongodb compass, obsidian, onlyoffice, piper, prettify, slack, smartgit, smoothcsv, sublime merge, sublime text, tableplus, transmission, typora, vlc, zed
```

## Full inventory

| App | What it is | Version | Source | Homepage |
| --- | --- | --- | --- | --- |
| Alacritty | Terminal emulator | 0.16.1 | deb | https://alacritty.org |
| Bruno | API client | 4.1.0 | AppImage | https://www.usebruno.com |
| ChatGPT | AI assistant / Codex app | 26.1007.71326 | deb | https://developers.openai.com/codex/app |
| Claude | AI assistant | 2.37337.1 | deb | https://claude.ai |
| CPU-X | Hardware info | 5.4.0 | deb | https://github.com/X0rg/CPU-X |
| Dadroit JSON Viewer | Large JSON viewer | — | AppImage | https://dadroit.com |
| draw.io | Diagramming | 31.5.3 | deb | https://www.drawio.com |
| Duplicati | Backup | 2.4.0.1 | deb | https://duplicati.com |
| Extension Manager | GNOME Shell extensions | 0.6.5 | deb | https://github.com/mjakeman/extension-manager |
| Fedora Media Writer | Bootable USB writer | 5.3.2 | flatpak | https://github.com/FedoraQt/MediaWriter |
| FolderSync Desktop | File sync | 2.13.0 | deb | https://foldersync.io |
| Foliate | E-book reader | 3.3.0 | snap | https://johnfactotum.github.io/foliate/ |
| Gear Lever | AppImage manager | 4.6.2 | flatpak | https://gearlever.mijorus.it |
| Genius | Math tool | 1.0.27 | deb | https://www.5z.com/jirka/genius.html |
| GNOME Boxes | Virtual machines | 49.1 | deb | https://apps.gnome.org/Boxes/ |
| GNOME Package Updater | Package updates (PackageKit) | 43.0 | deb | https://help.gnome.org/users/gnome-packagekit/stable/ |
| GNOME Tweaks | Desktop tweaks | 49.0 | deb | https://gitlab.gnome.org/GNOME/gnome-tweaks |
| Google Chrome | Web browser | 155.0.8059.79 | deb | https://www.google.com/chrome/ |
| Google Chrome Beta | Web browser (beta channel) | 156.0.8078.12 | deb | https://www.google.com/chrome/beta/ |
| Gramps | Genealogy | 6.0.8 | snap | https://gramps-project.org |
| Hardinfo2 | System info / benchmarks | 2.2.16 | deb | https://github.com/hardinfo2/hardinfo2 |
| Insync | Google Drive / OneDrive sync | 3.9.11 | deb | https://www.insynchq.com |
| kitty | Terminal emulator | 0.45.0 | deb | https://sw.kovidgoyal.net/kitty/ |
| KopiaUI | Backup | 0.23.1 | deb | https://kopia.io |
| Master PDF Editor 5 | PDF editor | 5.9.99 | deb | https://code-industry.net/free-pdf-editor/ |
| Mission Center | System monitor | 1.2.0 | flatpak | https://missioncenter.io |
| MongoDB Compass | MongoDB GUI | 1.50.0 | deb | https://www.mongodb.com/products/compass |
| Obsidian | Notes | 1.13.7 | deb | https://obsidian.md |
| ONLYOFFICE | Office suite | 9.4.0 | snap | https://www.onlyoffice.com |
| Piper | Gaming mouse config | 0.8 | deb | https://github.com/libratbag/piper |
| Prettify | JSON/YAML/CSV/XML viewer | 0.12.0 | deb | — |
| Slack | Team chat | 4.52.178 | deb | https://slack.com |
| SmartGit | Git client | 23.1.4 | tarball (`/opt`) | https://www.syntevo.com/smartgit/ |
| SmoothCSV | CSV editor | 3.25.1 | deb | https://smoothcsv.com |
| Sublime Merge | Git client | build 2132 | deb | https://www.sublimemerge.com |
| Sublime Text | Text editor | build 4215 | deb | https://www.sublimetext.com |
| TablePlus | Database GUI | 0.1.316 | deb | https://tableplus.com |
| Transmission | BitTorrent client | 4.1.3 | snap | https://transmissionbt.com |
| Typora | Markdown editor | 1.14.9 | deb | https://typora.io |
| VLC | Media player | 3.0.23 | deb | https://www.videolan.org/vlc/ |
| Zed | Code editor | 1.23.3 | install script (`~/.local`) | https://zed.dev |

### By source

| Source | Count |
| --- | --- |
| deb (apt repo or downloaded `.deb`) | 30 |
| snap | 4 |
| flatpak | 3 |
| AppImage (`~/AppImages`) | 2 |
| Tarball / install script | 2 |

## Left out

These have menu entries but don't count as standalone GUI apps added on purpose.

| Item | Why it's left out |
| --- | --- |
| htop, ranger, cmatrix, PowerShell | Run inside a terminal (`Terminal=true`) |
| WhatsApp Web, Perplexity | Chrome web-app shortcuts, not installed programs |
| TeXdoctk | Came in with `texlive-base` as a dependency of `apt install fnt` |
| QEMU | Hidden launcher (`NoDisplay=true`), pulled in as a dependency |
| Helper launchers (Insync helper, SmoothCSV handler, Claude Code URL handler, etc.) | Hidden launchers (`NoDisplay=true`) |

Some GUI apps that look added are actually part of the default 26.04 install:
Resources, Sysprof, Papers, Loupe, Ptyxis, Text Editor, Disks, Disk Usage Analyzer,
Firefox, App Center, Security Center and Firmware Updater.

## How this list was made

1. **Find GUI apps.** Read every `.desktop` launcher in `/usr/share/applications`,
   `/var/lib/snapd/desktop/applications`, `/var/lib/flatpak/exports/share/applications`
   and `~/.local/share/applications`. Skip entries with `NoDisplay=true` or `Terminal=true`.
2. **Find the default debs.** `/var/log/dpkg.log.1` starts on the day the install image
   was built (2026-04-23), so any package installed that day shipped with the image.
   Installer extras such as `ubuntu-restricted-addons` show up in `/var/log/apt/history.log`
   without a `Requested-By:` line.
3. **Find the default snaps.** They're listed in `/var/lib/snapd/seed/seed.yaml`.
4. **Everything else was added later.** Debs come from `dpkg -S` and `dpkg-query`, snaps from
   `snap list`, flatpaks from `flatpak list --app`, and AppImages / `/opt` installs from their
   launchers.
