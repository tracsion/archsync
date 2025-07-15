archsync
---------

archsync is a simple, fast CLI tool written in Rust for Arch Linux.
It lets you SAVE and RESTORE all your installed packages, including
official repo packages (via pacman) and AUR packages (via yay or paru).

This makes it easy to quickly replicate your Arch setup on a fresh install.

------------------------------------------
Features
------------------------------------------
- Saves all explicitly installed packages into a clean TOML file
- Separates official repo packages vs AUR packages
- Automatically restores your entire package list
- Colorful, user-friendly output
- Small and fast (written in Rust)

------------------------------------------
Usage
------------------------------------------

Save your current packages:

    archsync save

This creates a file called 'archpkglist.toml' listing all your packages.

Restore on a new system:

    archsync restore

This reads 'archpkglist.toml' and reinstalls everything using pacman for
repo packages and yay (or paru) for AUR packages.

------------------------------------------
Build
------------------------------------------

You need Rust installed. Then run:

    git clone https://github.com/yourusername/archsync.git
    cd archsync
    cargo build --release

------------------------------------------
Dependencies
------------------------------------------

- Arch Linux
- pacman (standard on Arch)
- yay or paru for AUR support

If you don’t have yay:

    git clone https://aur.archlinux.org/yay.git
    cd yay
    makepkg -si

------------------------------------------
License
------------------------------------------

MIT License. See LICENSE file for details.

------------------------------------------

Enjoy your fast Arch package snapshot & restore tool!
