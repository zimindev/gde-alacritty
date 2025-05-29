## 🧭 Alacritty Setup Guide

### ✅ What is Alacritty?

Alacritty is a fast, GPU-accelerated terminal emulator focused on simplicity and performance. It runs on Linux, macOS, and Windows and uses a YAML file for configuration.

---

### 🖥️ Step 1: Install Alacritty

#### **Linux (Debian/Ubuntu):**

```bash
sudo apt install alacritty
```

#### **Arch Linux:**

```bash
sudo pacman -S alacritty
```

#### **Fedora:**

```bash
sudo dnf install alacritty
```

#### **Windows:**

* Download the latest Alacritty release from [GitHub](https://github.com/alacritty/alacritty/releases).
* Extract the zip and run `alacritty.exe`.

#### **macOS:**

```bash
brew install alacritty
```

---

### 🚀 Step 2: Run Alacritty

* Open a terminal and type:

```bash
alacritty
```

---

### ⚙️ Step 3: Configure Alacritty

* Configuration is done via a YAML file located at:

```bash
~/.config/alacritty/alacritty.yml
```

* If the file doesn’t exist, copy the example config from the repo or create your own.

---

### ✍️ Step 4: Basic Configuration Example

Create or edit `~/.config/alacritty/alacritty.yml` with:

```yaml
font:
  normal:
    family: "JetBrainsMono Nerd Font"
  size: 12.0

colors:
  primary:
    background: '0x1e1e2e'
    foreground: '0xcdd6f4'

cursor:
  style: Beam
```

---

### 🔑 Step 5: Customize Keybindings (Optional)

You can add or override keybindings in the config file. For example:

```yaml
key_bindings:
  - { key: V,        mods: Control|Shift, action: Paste        }
  - { key: C,        mods: Control|Shift, action: Copy         }
```

---

### 🔄 Step 6: Make Alacritty Your Default Terminal (Optional)

#### On Linux (example with GNOME Terminal alternatives):

```bash
sudo update-alternatives --install /usr/bin/x-terminal-emulator x-terminal-emulator /usr/bin/alacritty 50
sudo update-alternatives --config x-terminal-emulator
```

---

### 📚 Additional Resources

* Official GitHub: [https://github.com/alacritty/alacritty](https://github.com/alacritty/alacritty)
* Configuration examples: [https://github.com/alacritty/alacritty/blob/master/alacritty.yml](https://github.com/alacritty/alacritty/blob/master/alacritty.yml)
* Nerd Fonts for better glyph support: [https://www.nerdfonts.com/](https://www.nerdfonts.com/)
