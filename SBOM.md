# SBOM

Software installed on top of a stock **Ubuntu 26.04.1 LTS (GNOME)** desktop.
Anything that ships with the default install is left out.

- **Taken:** 2026-10-15
- **Base image:** Ubuntu 26.04 "Resolute Raccoon" amd64 (20260423.1)
- **Total:** 41 GUI apps, 111 CLI tools

Apps with a package in the official repos of **Ubuntu 26.04** (`apt`) or **Fedora 44** (`dnf`)
are listed by package name. "—" means that distro doesn't package it. Apps packaged in neither
are listed with their homepage. PPAs, COPR, RPM Fusion and vendor repos (Google, Docker, Microsoft,
etc.) don't count.

## Quick lists

**GUI**

```
alacritty, bruno, chatgpt, claude, cpu-x, dadroit json viewer, draw.io, duplicati, extension manager, fedora media writer, foldersync desktop, foliate, gear lever, genius, gnome boxes, gnome package updater, gnome tweaks, google chrome, google chrome beta, gramps, hardinfo2, insync, kitty, kopiaui, master pdf editor 5, mission center, mongodb compass, obsidian, onlyoffice, piper, prettify, slack, smartgit, smoothcsv, sublime merge, sublime text, tableplus, transmission, typora, vlc, zed
```

**CLI**

```
7zip, antidote, aria2, autoconf, automake, bat, broot, btop, build-essential, canonical-livepatch, cifs-utils, claude code, cmatrix, containerd, cpufetch, ctop, curl, delta, docker, docker buildx, docker compose, docker sbx, duf, dust, eza, fastfetch, fd, ffmpeg, fio, flatpak, fnt, fx, fzf, gcloud, genius, gh, git, git-crypt, git-lfs, glances, go, gping, graphviz, htop, hwinfo, hyperfine, iftop, intel-gpu-tools, inxi, iotop, irqbalance, java, jless, jnv, libdrm-tests, libvirt, linuxlogo, lm-sensors, mesa-utils, miller, mise, mongodb-database-tools, mongosh, ncdu, neovim, neowofetch, nethogs, node, nvme-cli, openssh-server, perf, pip, pipes.sh, pkg-config, powershell, powertop, procs, qemu, ranger, ratbagd, recutils, restic, resticagent, ripgrep, rustup, shellcheck, shfmt, smartmontools, smbclient, stress-ng, swtpm, tmux, tmuxinator, tokei, tre, tree, tree-sitter, ttyper, util-linux-extra, uv, vainfo, vim, vulkan-tools, waypipe, wl-clipboard, xclip, xsel, yq, zile, zoxide, zsh
```

## GUI apps

### Packaged

| App | apt (Ubuntu) | dnf (Fedora) |
| --- | --- | --- |
| Alacritty | `alacritty` | `alacritty` |
| CPU-X | `cpu-x` | `cpu-x` |
| Extension Manager | `gnome-shell-extension-manager` | — |
| Fedora Media Writer | — | `mediawriter` |
| Foliate | `foliate` | `foliate` |
| Genius | `gnome-genius` | `gnome-genius` |
| GNOME Boxes | `gnome-boxes` | `gnome-boxes` |
| GNOME Package Updater | `gnome-package-updater` | `gnome-packagekit-updater` |
| GNOME Tweaks | `gnome-tweaks` | `gnome-tweaks` |
| Gramps | `gramps` | `gramps` |
| Hardinfo2 | `hardinfo2` | `hardinfo2` |
| kitty | `kitty` | `kitty` |
| Piper | `piper` | `piper` |
| Transmission | `transmission-gtk` | `transmission-gtk` |
| VLC | `vlc` | `vlc` |

### Not packaged

| App | Homepage |
| --- | --- |
| Bruno | https://www.usebruno.com |
| ChatGPT | https://developers.openai.com/codex/app |
| Claude | https://claude.ai |
| Dadroit JSON Viewer | https://dadroit.com |
| draw.io | https://www.drawio.com |
| Duplicati | https://duplicati.com |
| FolderSync Desktop | https://foldersync.io |
| Gear Lever | https://gearlever.mijorus.it |
| Google Chrome | https://www.google.com/chrome/ |
| Google Chrome Beta | https://www.google.com/chrome/beta/ |
| Insync | https://www.insynchq.com |
| KopiaUI | https://kopia.io |
| Master PDF Editor 5 | https://code-industry.net/free-pdf-editor/ |
| Mission Center | https://missioncenter.io |
| MongoDB Compass | https://www.mongodb.com/products/compass |
| Obsidian | https://obsidian.md |
| ONLYOFFICE | https://www.onlyoffice.com |
| Prettify | — |
| Slack | https://slack.com |
| SmartGit | https://www.syntevo.com/smartgit/ |
| SmoothCSV | https://smoothcsv.com |
| Sublime Merge | https://www.sublimemerge.com |
| Sublime Text | https://www.sublimetext.com |
| TablePlus | https://tableplus.com |
| Typora | https://typora.io |
| Zed | https://zed.dev |

## CLI tools

### Packaged

| Tool | apt (Ubuntu) | dnf (Fedora) |
| --- | --- | --- |
| 7zip | `7zip` | `7zip` |
| antidote | `zsh-antidote` | — |
| aria2 | `aria2` | `aria2` |
| autoconf | `autoconf` | `autoconf` |
| automake | `automake` | `automake` |
| bat | `bat` | `bat` |
| broot | `broot` | — |
| btop | `btop` | `btop` |
| build-essential | `build-essential` | `gcc gcc-c++ make` |
| cifs-utils | `cifs-utils` | `cifs-utils` |
| cmatrix | `cmatrix` | `cmatrix` |
| containerd | `containerd` | `containerd` |
| cpufetch | `cpufetch` | `cpufetch` |
| curl | `curl` | `curl` |
| delta | `git-delta` | `git-delta` |
| docker | `docker.io` | `moby-engine` |
| docker buildx | `docker-buildx` | `docker-buildx` |
| docker compose | `docker-compose-v2` | `docker-compose` |
| duf | `duf` | `duf` |
| dust | `du-dust` | `du-dust` |
| eza | `eza` | `eza` |
| fastfetch | `fastfetch` | `fastfetch` |
| fd | `fd-find` | `fd-find` |
| ffmpeg | `ffmpeg` | `ffmpeg-free` ¹ |
| fio | `fio` | `fio` |
| flatpak | `flatpak` | `flatpak` |
| fnt | `fnt` | — |
| fzf | `fzf` | `fzf` |
| genius | `genius` | `genius` |
| gh | `gh` | `gh` |
| git | `git` | `git` |
| git-crypt | `git-crypt` | `git-crypt` |
| git-lfs | `git-lfs` | `git-lfs` |
| glances | `glances` | `glances` |
| go | `golang-go` | `golang` |
| gping | `gping` | — |
| graphviz | `graphviz` | `graphviz` |
| htop | `htop` | `htop` |
| hwinfo | `hwinfo` | `hwinfo` |
| hyperfine | `hyperfine` | `hyperfine` |
| iftop | `iftop` | `iftop` |
| intel-gpu-tools | `igt-gpu-tools` | `igt-gpu-tools` |
| inxi | `inxi` | `inxi` |
| iotop | `iotop` | `iotop-c` ² |
| irqbalance | `irqbalance` | `irqbalance` |
| java | `openjdk-25-jdk` | `java-25-openjdk-devel` ³ |
| libdrm-tests | `libdrm-tests` | `drm-utils` |
| libvirt | `libvirt-daemon-system libvirt-clients` | `libvirt` |
| linuxlogo | `linuxlogo` | — |
| lm-sensors | `lm-sensors` | `lm_sensors` |
| mesa-utils | `mesa-utils` | `glx-utils mesa-demos` |
| miller | `miller` | `miller` |
| ncdu | `ncdu` | `ncdu` |
| neovim | `neovim` | `neovim` |
| neowofetch | `neowofetch` | — |
| nethogs | `nethogs` | `nethogs` |
| node | `nodejs` | `nodejs` ⁴ |
| nvme-cli | `nvme-cli` | `nvme-cli` |
| openssh-server | `openssh-server` | `openssh-server` |
| perf | `linux-tools-generic` | `perf` |
| pip | `python3-pip` | `python3-pip` |
| pipes.sh | `pipes-sh` | — |
| pkg-config | `pkgconf` | `pkgconf-pkg-config` |
| powertop | `powertop` | `powertop` |
| procs | `procs` | `procs` |
| qemu | `qemu-system-x86 qemu-utils` | `qemu-system-x86 qemu-img` |
| ranger | `ranger` | `ranger` |
| ratbagd | `ratbagd` | `libratbag-ratbagd` |
| recutils | `recutils` | `recutils` |
| restic | `restic` | `restic` |
| ripgrep | `ripgrep` | `ripgrep` |
| rustup | `rustup` | `rustup` |
| shellcheck | `shellcheck` | `ShellCheck` |
| shfmt | `shfmt` | `shfmt` |
| smartmontools | `smartmontools` | `smartmontools` |
| smbclient | `smbclient` | `samba-client` |
| stress-ng | `stress-ng` | `stress-ng` |
| swtpm | `swtpm` | `swtpm` |
| tmux | `tmux` | `tmux` |
| tmuxinator | `tmuxinator` | — |
| tokei | `tokei` | `tokei` |
| tre | `tre-command` | — |
| tree | `tree` | `tree` |
| tree-sitter | `tree-sitter-cli` | `tree-sitter-cli` |
| util-linux-extra | `util-linux-extra` | `util-linux` |
| uv | — | `uv` |
| vainfo | `vainfo` | `libva-utils` |
| vim | `vim` | `vim-enhanced` |
| vulkan-tools | `vulkan-tools` | `vulkan-tools` |
| waypipe | `waypipe` | `waypipe` |
| wl-clipboard | `wl-clipboard` | `wl-clipboard` |
| xclip | `xclip` | `xclip` |
| xsel | `xsel` | `xsel` |
| yq | `yq` | — ⁵ |
| zile | `zile` | `zile` |
| zoxide | `zoxide` | `zoxide` |
| zsh | `zsh` | `zsh` |

1. Fedora's build leaves out patent-encumbered codecs. The full `ffmpeg` is in RPM Fusion.
2. A C rewrite of the original Python `iotop`, with the same command name.
3. OpenJDK from the distro. The Temurin build used here comes from mise.
4. Installs the distro's default Node version (22 on Fedora 44). The version used here, 26, comes from mise.
5. Fedora's `yq` is a different project ([mikefarah/yq](https://github.com/mikefarah/yq)). The one used here is the jq wrapper from [kislyuk/yq](https://github.com/kislyuk/yq).

### Not packaged

| Tool | Homepage |
| --- | --- |
| canonical-livepatch | https://ubuntu.com/security/livepatch |
| claude code | https://claude.com/claude-code |
| ctop | https://github.com/bcicen/ctop |
| docker sbx | https://docs.docker.com/sandbox/ |
| fx | https://fx.wtf |
| gcloud | https://cloud.google.com/sdk |
| jless | https://github.com/PaulJuliusMartinez/jless |
| jnv | https://github.com/ynqa/jnv |
| mise | https://mise.jdx.dev |
| mongodb-database-tools | https://www.mongodb.com/try/download/database-tools |
| mongosh | https://www.mongodb.com/products/tools/shell |
| powershell | https://github.com/PowerShell/PowerShell |
| resticagent | — (own script) |
| ttyper | https://github.com/max-niederman/ttyper |

## Left out

### GUI

| Item | Why it's left out |
| --- | --- |
| htop, ranger, cmatrix, PowerShell | Run inside a terminal, so they're listed under CLI |
| WhatsApp Web, Perplexity | Chrome web-app shortcuts, not installed programs |
| TeXdoctk | Came in with `texlive-base` as a dependency of `fnt` |
| QEMU | Hidden launcher (`NoDisplay=true`), pulled in as a dependency |
| Helper launchers (Insync helper, SmoothCSV handler, Claude Code URL handler, etc.) | Hidden launchers (`NoDisplay=true`) |

### CLI

| Item | Why it's left out |
| --- | --- |
| `subl`, `smerge`, `kitten`, `duplicati-cli`, `smoothcsv-cli`, etc. | Command-line launchers that come with GUI apps listed above |
| gcc, g++, make | Come with build-essential |
| ruby, texlive, postfix, mailutils | Pulled in as dependencies (by tmuxinator, fnt and smartmontools) |
| cups snap | Added automatically by snapd |
| npm | Bundled with node |
| zsh plugins | Managed by antidote |
| Libraries, `-dev` headers, drivers, firmware, kernel packages | Not programs you run |
| tailscale-archive-keyring | Leftover keyring; Tailscale itself is uninstalled |

### Already in the default install

- **GUI:** Resources, Sysprof, Papers, Loupe, Ptyxis, Text Editor, Disks, Disk Usage Analyzer,
  Firefox, App Center, Security Center and Firmware Updater.
- **CLI:** jq. It's also managed by mise here, but it ships with 26.04.

## How this list was made

1. **Find GUI apps.** Read every `.desktop` launcher in `/usr/share/applications`,
   `/var/lib/snapd/desktop/applications`, `/var/lib/flatpak/exports/share/applications`
   and `~/.local/share/applications`. Skip entries with `NoDisplay=true` or `Terminal=true`.
2. **Find CLI tools.** Take manually installed apt packages (`apt-mark showmanual`) that ship
   executables, plus tools from mise (`mise ls`), snaps, rustup, the gcloud SDK, `~/.local/bin`
   and `/usr/local/bin`.
3. **Find the default debs.** `/var/log/dpkg.log.1` starts on the day the install image was
   built (2026-04-23), so any package installed that day shipped with the image. Installer
   extras such as `ubuntu-restricted-addons` show up in `/var/log/apt/history.log` without a
   `Requested-By:` line.
4. **Find the default snaps.** They're listed in `/var/lib/snapd/seed/seed.yaml`.
5. **Look up package names.**
   - **Ubuntu:** `apt-cache policy`, counting only packages served from `archive.ubuntu.com`
     or `security.ubuntu.com`.
   - **Fedora:** `dnf repoquery --whatprovides /usr/bin/<command>` in a `fedora:44` container,
     which finds packages by the command they install even when the package name differs.
