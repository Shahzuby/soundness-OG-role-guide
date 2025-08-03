# Soundness Codes - Installation & Wallet Management Guide

Official Discords:
- Main: [https://discord.gg/soundnesslabs](https://discord.gg/soundnesslabs)

---

### 🚀 **Quick Start Guide**

1️⃣ Type `/8queens` to play your first puzzle

2️⃣ Win and hit **"Generate Ligero Proof"** in your game channel keep your proof safe 

<img width="456" height="472" alt="image" src="https://github.com/user-attachments/assets/6019d6d0-71d4-495e-9281-a17baab1b8cb" />

---

## 🧑‍💻 Run Inside GitHub Codespace (Recommended)

You can run all commands directly in GitHub using **Codespaces** without needing a local Linux machine.

### ➕ How to Create a Codespace

1. Go to the codespace on this repo
2. Click the green **Code** button > Select **"Open with Codespaces"** > **New codespace**
3. Wait for the environment to load (1–2 mins)
4. Now, run the below commands inside the terminal panel

---

## 🔧 System Preparation

Update your system before proceeding:

```bash
sudo apt update && sudo apt upgrade -y
```

---

## ⚙️ Install Soundness CLI

```bash
curl -sSL https://raw.githubusercontent.com/soundnesslabs/soundness-layer/main/soundnessup/install | bash
```

---

## 🛠 Install Rust (if not already installed)

```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs/ | sh
```

After installing Rust, reload the shell:

```bash
source ~/.bashrc
```

---

## 📦 Setup Soundness CLI

```bash
soundnessup install
soundnessup update
```

---

## 🔐 Wallet Management

### 🔁 Import Existing Wallet

```bash
soundness-cli import-key --name my-key --mnemonic "<your-mnemonic-words>"
```

---

### 🧠 Generate New Wallet

```bash
soundness-cli generate-key --name my-key
```

Send this key to the team on the Discord `#soundness-cockpit` channel if you create new key 

---

### 📤 Export Wallet

```bash
soundness-cli export-key --name my-key
```

Expected output:

```
✅ Imported key pair 'my-key'
🔑 Public key:
```

---

### 📜 List All Stored Keys

```bash
soundness-cli list-keys
```

### 📜 paste your game proof 
done

---

## 📌 Notes

- Keep your mnemonic phrase safe and backed up.
- Use GitHub Codespace for easiest setup with zero local dependency.
- Join the Discord server for any support or issues.
