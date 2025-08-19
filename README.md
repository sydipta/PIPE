# 🚀 Pipe Firestarter Storage Node Guide

This guide explains how to set up and use the **Pipe Firestarter CLI** to upload files/folders, earn rewards, and become part of the decentralized storage network.  

---

## ⚡ What is Pipe?  
Pipe is a decentralized storage and delivery network — a blockchain-powered alternative to services like Google Drive or Cloudflare.  

- Built on **Solana**  
- Hosts **1 PB+** of blockchain history, reducing validator sync time by ~30%  
- Users can upload files/folders, encrypt them, and share via public links  
- Payments are made in **$PIPE tokens**  

---

## 🛠 Prerequisites  

Update & install dependencies:  
```bash
sudo apt update && sudo apt upgrade -y
sudo apt install curl iptables build-essential git wget lz4 jq make gcc postgresql-client nano automake autoconf tmux htop nvme-cli libgbm1 pkg-config libssl-dev tar clang bsdmainutils ncdu unzip libleveldb-dev libclang-dev ninja-build -y
```

Install Rust:  
```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
source $HOME/.cargo/env
```

---

## ⚙️ Installation  

Clone the repo and install CLI:  
```bash
git clone https://github.com/PipeNetwork/pipe.git
cd pipe
cargo install --path .
pipe -h
```

Create user & set password:  
```bash
pipe new-user <your_username>
pipe set-password
nano ~/.pipe-cli.json
```

Login later with:  
```bash
pipe login <your_username>
```

---

## 🎁 Referral Program  

You can earn extra **PIPE tokens** by applying a referral code before you start.  

👉 Use my referral code:  
```bash
pipe referral apply SYDIPTA-DYVL
```

Check status:  
```bash
pipe referral show
```

Generate your own referral code:  
```bash
pipe referral generate
```

---

## 💰 Token Swap (Devnet)  

Request SOL from faucet: [https://faucet.solana.com](https://faucet.solana.com)  

Swap SOL → PIPE:  
```bash
pipe swap-sol-for-pipe <AMOUNT_SOL>
```

---

## 📤 Uploading Files & Folders  

**Upload a file:**  
```bash
pipe upload-file <FILE_PATH> <FILE_NAME>
```

**Upload a directory:**  
```bash
pipe upload-directory <DIRECTORY_PATH>
```

**Make it public:**  
```bash
pipe create-public-link <NAME>
```

**List uploads:**  
```bash
pipe list-files
```

---

## 🔥 Become a Firestarter  

1. Upload at least one file  
2. Create a public link  
3. Join the [Pipe Discord](https://discord.gg/pipe) and share your contribution  

---

✨ You are now part of the Pipe decentralized storage movement!  
