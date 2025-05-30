Got it! Here's the optimized and clean `README.md` in **English** for your GitHub Alacritty setup guide, using the **TOML** config format:

````markdown
# 🧭 Alacritty Setup Guide (TOML Config)

## ✅ What is Alacritty?

**Alacritty** is a fast, GPU-accelerated terminal emulator focused on performance and simplicity. As of version **0.12.0**, Alacritty uses **TOML** instead of YAML for configuration.

---

## 🖥️ Installation

### Debian/Ubuntu
```bash
sudo apt install alacritty
````

### Arch Linux

```bash
sudo pacman -S alacritty
```

### Fedora

```bash
sudo dnf install alacritty
```

### macOS

```bash
brew install alacritty
```

### Windows

* Download the latest release: [Alacritty Releases](https://github.com/alacritty/alacritty/releases)
* Extract the `.zip` and run `alacritty.exe`

---

## 🚀 Launch Alacritty

```bash
alacritty
```

---

## ⚙️ Configuration

The main config file is located at:

```
~/.config/alacritty/alacritty.toml
```

If it doesn’t exist, you can create it or copy the official example from [here](https://github.com/alacritty/alacritty/blob/master/alacritty.toml).

---

## ✍️ Basic Configuration Example (`alacritty.toml`)

```toml
[font.normal]
family = "JetBrainsMono Nerd Font"
size = 12.0

[colors.primary]
background = "0x1e1e2e"
foreground = "0xcdd6f4"

[cursor]
style = "Beam"
```

---

## 🔑 Custom Key Bindings (Optional)

```toml
[[key_bindings]]
key = "V"
mods = "Control|Shift"
action = "Paste"

[[key_bindings]]
key = "C"
mods = "Control|Shift"
action = "Copy"
```

---

## 🔄 Set Alacritty as Default Terminal (Linux)

```bash
sudo update-alternatives --install /usr/bin/x-terminal-emulator x-terminal-emulator /usr/bin/alacritty 50
sudo update-alternatives --config x-terminal-emulator
```

---

## 📚 Additional Resources

* 🔗 [Official GitHub](https://github.com/alacritty/alacritty)
* 🔗 [alacritty.toml Example](https://github.com/alacritty/alacritty/blob/master/alacritty.toml)
* 🔗 [Nerd Fonts](https://www.nerdfonts.com/)
* ▶️ [Make Alacritty Amazing (macOS)](https://youtu.be/uOnL4fEnldA)
* ▶️ [Alacritty Overview](https://youtu.be/n3CWYPGjVns)
