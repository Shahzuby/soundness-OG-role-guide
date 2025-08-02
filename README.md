# Soundness Codes - Installation & Wallet Management Guide

Official Discords:
- Main: [https://discord.gg/soundnesslabs](https://discord.gg/soundnesslabs)

---

### 🚀 **Quick Start Guide**
1️⃣ Type `/8queens` to play your first puzzle
2️⃣ Win and hit **"Generate Ligero Proof"** in your game channel
3️⃣ Earn your first badge + unlock the **Sound OG** role

### ✨ **Game Arena Highlights**
🔐 Real zero-knowledge proofs of your wins --> showing the fact that you won a game while protecting your personal info.
🎮 Modern web-based games — no installs, no friction
🏅 13+ unique achievement badges (You can check them later)
🐋 Walrus storage = your proofs live on-chain for 2 weeks
🧠🐬 The validity of your proofs will be stored as an object on the Sui mainnet.

💬 **Need help or have questions?** Ask in the community — we’re all here to play, learn, and level up together.

🎉 **Ready to play?** Start a game and enter the Arena!
<img width="456" height="472" alt="image" src="https://github.com/user-attachments/assets/6019d6d0-71d4-495e-9281-a17baab1b8cb" />

---

### 🕹️🎪 **Welcome to the Sound Game Arena!** 🎪🕹️

Step into Soundness Labs' playground for Web3 gaming, zero-knowledge puzzles, and friendly competition. Here’s what you can do:
🎯 Play games and generate zero-knowledge proofs
🐋 Directly store your zk proofs to Walrus
🐬  Then interact with Soundness layer for proof attestations

Use the commands below to get started — all games come with interactive guides to help you along the way!

## 🧑‍💻 Run Inside GitHub Codespace (Recommended)

You can run all commands directly in GitHub using **Codespaces** without needing a local Linux machine.

### ➕ How to Create a Codespace

1. Go to the GitHub: create new repo with random name and add readme and created
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
