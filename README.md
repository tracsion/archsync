# archsync

`archsync` is a simple, fast CLI tool written in Rust for Arch Linux that helps you **save** and **restore** all your installed packages.  
It tracks both official repo packages and AUR packages, so you can easily replicate your setup on a fresh Arch install.

---

## ✨ Features

✅ Saves all explicitly installed packages into a clean TOML file  
✅ Distinguishes between official repo packages (pacman) and AUR packages (yay/paru)  
✅ Restores your entire package list automatically  
✅ Colorful, user-friendly output  
✅ Small and blazing fast (built with Rust)

---

## 🚀 Usage

### Save your current packages
Generates a `archpkglist.toml` file with all explicitly installed packages.


archsync save

Restore on a new system

Reads the archpkglist.toml file and reinstalls everything, using pacman for repo packages and yay (or paru) for AUR.

archsync restore

⚙️ Build

You need Rust installed.

git clone https://github.com/yourusername/archsync.git
cd archsync
cargo build --release

Then copy the binary:

sudo cp target/release/archsync /usr/local/bin/

🔗 Dependencies

    🐧 Arch Linux

    pacman (default on Arch)

    yay or paru for AUR support

If you don’t have yay, install it:

git clone https://aur.archlinux.org/yay.git
cd yay
makepkg -si

📝 License

MIT License.
See LICENSE for details.
💻 Screenshot

    Optional: You could paste an example CLI run here later.

Enjoy your fast Arch package snapshot & restore tool! 🎉


---

✅ If you’d like, I can also make:
- a **LICENSE file** for you (MIT with your name/year),
- or a **badges section** (with Rust version, license, etc).

Just tell me! 🚀
