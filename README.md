# SPCDE — Spark Desktop Environment

**A lightweight, classic desktop environment for Linux, powered by Sparks.**

![License](https://img.shields.io/badge/License-GPLv3-blue.svg)

SPCDE is an experimental desktop environment focused on simplicity, performance, customization and low memory usage.

Inspired by classic Linux desktops, SPCDE aims to provide a familiar and responsive experience without unnecessary services or excessive resource consumption.

SPCDE is built using **Sparks**, a custom programming language, alongside native Linux and X11 bindings.

## Features

- Lightweight desktop and window manager.
- Classic window decorations and taskbar.
- Custom right-click menus.
- Desktop file management.
- File-specific icons and external icon themes.
- Custom wallpapers and gradient backgrounds.
- Four included wallpapers.
- Copy, cut and paste support.
- Experimental file drag-and-drop.
- Efficient desktop rendering.
- Emergency Disable DE button.
- Independent desktop settings.

## Memory Usage

Previous measurements on Debian:

| Component | RAM usage |
|---|---:|
| SPCDE | ~2 MB |
| Xorg | ~102 MB |
| Combined | ~104 MB |

Memory usage may vary depending on hardware and running applications.

Our goal is to make SPCDE even lighter without sacrificing usability.

## Installation

### Debian and Debian-based distributions

Install the required dependencies:

```bash
sudo apt install build-essential libx11-dev \
    feh zenity xterm thunar xclip \
    xfce4-clipman python3-gi gir1.2-gtk-3.0
```

Extract the SPCDE archive, open its directory and run:

```bash
sudo bash install-session.sh
```

Log out and select SPCDE from your login screen.

## Customization

Make your desktop look the way you want.

Right-click the desktop to access wallpapers, icon styles, applications and other settings.

SPCDE supports installed Linux icon themes, custom images, gradients and multiple wallpaper display modes.

## Keyboard Shortcuts

| Shortcut | Action |
|---|---|
| Ctrl+C | Copy |
| Ctrl+X | Cut |
| Ctrl+V | Paste |
| Ctrl+Shift+C | Terminal copy |
| Ctrl+Shift+V | Terminal paste |
| Super+Shift+Esc | Emergency exit |

## The Anti-Yandere System

SPCDE once had a bug where it refused to let users switch to another desktop environment.

We called it the **Yandere Bug**.

SPCDE now includes an emergency Disable DE feature to help users safely switch back to their preferred desktop.

You can also disable SPCDE manually:

```bash
sudo /opt/spcde/disable-session.sh
```

And enable it again:

```bash
sudo /opt/spcde/enable-session.sh
```

## Future Plans

- [x] Sparks-powered desktop
- [x] Window management
- [x] Wallpaper customization
- [x] Custom desktop menus
- [x] External icon themes
- [x] Efficient desktop rendering
- [x] Emergency desktop exit
- [ ] Improved clipboard compatibility
- [ ] Full drag-and-drop support
- [ ] Optimized independent Xorg
- [ ] Xorg memory usage below 40 MB
- [ ] Spark Server (SPS)
- [ ] Spark Rendering (SPR)
- [ ] Independent graphics system without X11 or Wayland
- [ ] SPCDE Linux distribution

## Our Philosophy

SPCDE is built around a few simple ideas:

- Your desktop should not consume unnecessary resources.
- Simplicity should not limit functionality.
- Users should have control over their systems.
- Classic desktop designs are still worth preserving.
- Other installed desktop environments should remain untouched.

## Development Status

SPCDE is currently experimental and actively being developed.

Bugs and incomplete features are expected. Testing in a virtual machine is recommended.

Contributions, suggestions, bug reports and performance tests are always welcome.

## License

SPCDE is free and open-source software licensed under the **GNU General Public License v3.0 (GPLv3)**.

You are free to use, modify and redistribute SPCDE under the terms of this license.

Third-party components and artwork remain subject to their respective licenses.

See the [LICENSE](LICENSE) file for more information.

---

**SPCDE — Your desktop, your rules.**

*Lightweight by design. Independent by ambition.*
