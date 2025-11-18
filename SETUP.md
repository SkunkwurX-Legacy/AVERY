# Avery Setup Guide  
Sovereign Cold Wallet Initialization  
Licensed to the Sovereign Trust  
Trustee: Matthew David Palmer ($MADMONEY42)  
Beneficiaries: Trustee and Mother

---

## Step 1: Connect Your Cold Wallet

Start by plugging in your hardware wallet — Ledger, Trezor, Keystone, or any device holding your seed.  
Avery will detect the device and request only the extended public keys (xpubs).  
Your mnemonic stays sealed inside the hardware. Avery never touches it.

---

## Step 2: Mnemonic Orchestration

Avery uses your master seed to derive wallet addresses by role.  
Each role has a dedicated index range:

| Role                  | Index Range  | Purpose                        |
|-----------------------|--------------|--------------------------------|
| Validator             | 1000–1099    | Core operational addresses     |
| Archive               | 2000–2099    | Long-term storage              |
| Relic Mint            | 3000–3099    | NFT/XFT minting                |
| Rescue                | 4000–4099    | Recovery from breach           |
| Delegated Agents (AMP)| 5000–5099    | Smart contract workflows       |
| Genesis Cockpit       | 6000–6099    | Origin ledger entries          |
| Experimental/Sandbox  | 7000–7099    | Testing and dev deployments    |
| Public Drops          | 8000
