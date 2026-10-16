# SBOM

Software installed on top of a stock **Ubuntu 26.10 (GNOME)** desktop.
Anything that ships with the default install is left out.

- **Taken:** 2026-10-16
- **Base image:** Ubuntu 26.10 "Stonking Stingray" amd64 (20261013)
- **Total:** 26 GUI apps, 88 CLI tools

Apps with a package in the official repos of **Ubuntu 26.10** (`apt`) or **Fedora 44** (`dnf`)
are listed by package name. "—" means that distro doesn't package it. Apps packaged in neither
are listed with their homepage. PPAs, COPR, RPM Fusion and vendor repos (Google, Docker, Microsoft,
etc.) don't count.

## Quick lists

**GUI**

```
chatgpt, claude, cpu-x, extension manager, foliate, gear lever, gnome boxes, gnome tweaks, google chrome, hardinfo2, kitty, mission center, mongodb compass, obsidian, onlyoffice, postman, prettify, slack, smoothcsv, sublime merge, sublime text, thunderbird, transmission, typora, visual studio code, vlc
```

**CLI**

```
antidote, aria2, autoconf, automake, bat, btop, build-essential, cifs-utils, claude code, cmatrix, codex, containerd, cpufetch, ctop, curl, delta, docker, docker buildx, docker compose, duf, dust, eza, fastfetch, fd, ffmpeg, fio, flatpak, fnt, fzf, gh, git, git-crypt, git-lfs, glances, go, gping, hwinfo, hyperfine, iftop, intel-gpu-tools, inxi, iotop, java, libdrm-tests, libvirt, linuxlogo, lm-sensors, mesa-utils, mise, mongodb-database-tools, mongosh, ncdu, neovim, nethogs, node, nvme-cli, perf, pip, pipes.sh, pkg-config, powertop, procs, qemu, ripgrep, rustup, shellcheck, shfmt, smartmontools, smbclient, stress-ng, swtpm, tmux, tmuxinator, tokei, tree, tree-sitter, util-linux-extra, uv, vainfo, vulkan-tools, waypipe, wl-clipboard, xclip, xsel, yq, zile, zoxide, zsh
```

## GUI apps

### Packaged

| App | apt (Ubuntu) | dnf (Fedora) |
| --- | --- | --- |
| CPU-X | `cpu-x` | `cpu-x` |
| Extension Manager | `gnome-shell-extension-manager` | — |
| Foliate | `foliate` | `foliate` |
| GNOME Boxes | `gnome-boxes` | `gnome-boxes` |
| GNOME Tweaks | `gnome-tweaks` | `gnome-tweaks` |
| Hardinfo2 | `hardinfo2` | `hardinfo2` |
| kitty | `kitty` | `kitty` |
| Thunderbird | `thunderbird` | `thunderbird` |
| Transmission | `transmission-gtk` | `transmission-gtk` |
| VLC | `vlc` | `vlc` |

### Not packaged

| App | Homepage |
| --- | --- |
| ChatGPT | https://developers.openai.com/codex/app |
| Claude | https://claude.ai |
| Gear Lever | https://gearlever.mijorus.it |
| Google Chrome | https://www.google.com/chrome/ |
| Mission Center | https://missioncenter.io |
| MongoDB Compass | https://www.mongodb.com/products/compass |
| Obsidian | https://obsidian.md |
| ONLYOFFICE | https://www.onlyoffice.com |
| Postman | https://www.postman.com |
| Prettify | — |
| Slack | https://slack.com |
| SmoothCSV | https://smoothcsv.com |
| Sublime Merge | https://www.sublimemerge.com |
| Sublime Text | https://www.sublimetext.com |
| Typora | https://typora.io |
| Visual Studio Code | https://code.visualstudio.com |

## CLI tools

### Packaged

| Tool | apt (Ubuntu) | dnf (Fedora) |
| --- | --- | --- |
| antidote | `zsh-antidote` | — |
| aria2 | `aria2` | `aria2` |
| autoconf | `autoconf` | `autoconf` |
| automake | `automake` | `automake` |
| bat | `bat` | `bat` |
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
| gh | `gh` | `gh` |
| git | `git` | `git` |
| git-crypt | `git-crypt` | `git-crypt` |
| git-lfs | `git-lfs` | `git-lfs` |
| glances | `glances` | `glances` |
| go | `golang-go` | `golang` |
| gping | `gping` | — |
| hwinfo | `hwinfo` | `hwinfo` |
| hyperfine | `hyperfine` | `hyperfine` |
| iftop | `iftop` | `iftop` |
| intel-gpu-tools | `igt-gpu-tools` | `igt-gpu-tools` |
| inxi | `inxi` | `inxi` |
| iotop | `iotop` | `iotop-c` ² |
| java | `openjdk-25-jdk` | `java-25-openjdk-devel` ³ |
| libdrm-tests | `libdrm-tests` | `drm-utils` |
| libvirt | `libvirt-daemon-system libvirt-clients` | `libvirt` |
| linuxlogo | `linuxlogo` | — |
| lm-sensors | `lm-sensors` | `lm_sensors` |
| mesa-utils | `mesa-utils` | `glx-utils mesa-demos` |
| ncdu | `ncdu` | `ncdu` |
| neovim | `neovim` | `neovim` |
| nethogs | `nethogs` | `nethogs` |
| node | `nodejs` | `nodejs` ⁴ |
| nvme-cli | `nvme-cli` | `nvme-cli` |
| perf | `linux-tools-generic` | `perf` |
| pip | `python3-pip` | `python3-pip` |
| pipes.sh | `pipes-sh` | — |
| pkg-config | `pkgconf` | `pkgconf-pkg-config` |
| powertop | `powertop` | `powertop` |
| procs | `procs` | `procs` |
| qemu | `qemu-system-x86 qemu-utils` | `qemu-system-x86 qemu-img` |
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
| tree | `tree` | `tree` |
| tree-sitter | `tree-sitter-cli` | `tree-sitter-cli` |
| util-linux-extra | `util-linux-extra` | `util-linux` |
| uv | — | `uv` |
| vainfo | `vainfo` | `libva-utils` |
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
| claude code | https://claude.com/claude-code |
| codex | https://developers.openai.com/codex/cli |
| ctop | https://github.com/bcicen/ctop |
| mise | https://mise.jdx.dev |
| mongodb-database-tools | https://www.mongodb.com/try/download/database-tools |
| mongosh | https://www.mongodb.com/products/tools/shell |

## Left out

### GUI

| Item | Why it's left out |
| --- | --- |
| cmatrix, Neovim | Run inside a terminal, so they're listed under CLI |
| WhatsApp Web | Chrome web-app shortcut, not an installed program |
| TeXdoctk | Came in with `texlive-base` as a dependency of `fnt` |
| QEMU | Hidden launcher (`NoDisplay=true`), pulled in as a dependency |
| Helper launchers (VS Code URL handler, SmoothCSV handler, Claude Code URL handler, etc.) | Hidden launchers (`NoDisplay=true`) |

### CLI

| Item | Why it's left out |
| --- | --- |
| `subl`, `smerge`, `kitten`, `code`, `chatgpt`, `obsidian`, `smoothcsv-cli`, etc. | Command-line launchers that come with GUI apps listed above |
| gcc, g++, make | Come with build-essential |
| ruby, texlive | Pulled in as dependencies (by tmuxinator and fnt) |
| cups snap | Added automatically by snapd |
| core18, core20, core26, gnome-3-28-1804 snaps | Runtimes pulled in by other snaps |
| npm | Bundled with node |
| cargo, rustc, rust-analyzer, etc. | Managed by rustup |
| python3-venv | Python module, no command of its own |
| apt-transport-https | Empty transitional package |
| zsh plugins | Managed by antidote |
| Libraries, `-dev` headers, drivers, firmware (`ovmf`), kernel packages, `libfuse2t64` | Not programs you run |

### Already in the default install

- **GUI:** Resources, Sysprof, Papers, Loupe, Ptyxis, Text Editor, Disks, Disk Usage Analyzer,
  Firefox, App Center, Security Center and Firmware Updater.
- **CLI:** jq. It's also managed by mise here, but it ships with 26.10.

## How this list was made

1. **Find GUI apps.** Read every `.desktop` launcher in `/usr/share/applications`,
   `/var/lib/snapd/desktop/applications`, `/var/lib/flatpak/exports/share/applications`
   and `~/.local/share/applications`. Skip entries with `NoDisplay=true` or `Terminal=true`.
2. **Find CLI tools.** Take manually installed apt packages (`apt-mark showmanual`) that ship
   executables, plus tools from mise (`mise ls`), snaps, rustup, global npm packages, `~/.local/bin`
   and `/usr/local/bin`.
3. **Find the default debs.** `/var/log/dpkg.log` starts on the day the install image was
   built (2026-10-13), so any package installed that day shipped with the image. Installer
   extras such as `ubuntu-restricted-addons` show up in `/var/log/apt/history.log` without a
   `Requested-By:` line.
4. **Find the default snaps.** They're listed in `/var/lib/snapd/seed/seed.yaml`.
5. **Look up package names.**
   - **Ubuntu:** `apt-cache policy`, counting only packages served from `archive.ubuntu.com`
     or `security.ubuntu.com`.
   - **Fedora:** `dnf repoquery --whatprovides /usr/bin/<command>` in a `fedora:44` container,
     which finds packages by the command they install even when the package name differs.
