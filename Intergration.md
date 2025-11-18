# Avery Integration Guide  
Multi-Wallet Orchestration and Role-Based Import  
Licensed to the Sovereign Trust  
Trustee: Matthew David Palmer ($MADMONEY42)  
Beneficiaries: Trustee and Mother

---

## Overview

Avery is not a wallet. She’s a cold cockpit that integrates all your wallets under one sovereign roof.  
Once connected, Avery pulls extended public keys (xpubs), derives addresses by role, and enforces your doctrine automatically.  
No seed exposure. No manual entry. No fragmentation.

---

## Supported Wallets

Avery integrates with any hardware wallet or cold vault that supports xpub export:

- Ledger Nano / Ledger Stax  
- Trezor Model T / Trezor One  
- Keystone / Coldcard / BitBox  
- XRP Toolkit / MetaMask (watch-only)  
- Solana Phantom (via xpub or address import)  
- BTC, ETH, XRP, SOL, ADA, LTC, BCH, DOGE, ZEC, XLM

---

## Integration Steps

1. **Connect your hardware wallet**  
   Avery detects the device and requests xpubs only.  
   Mnemonic stays sealed in hardware custody.

2. **Import xpubs by chain**  
   Avery auto-detects chain type and derives addresses using standard paths:  
   - BTC: `m/84'/0'/0'/0/i`  
   - ETH: `m/44'/60'/0'/0/i`  
   - XRP: `m/44'/144'/0'/0/i`  
   - SOL: `m/44'/501'/0'/0/i`

3. **Assign roles by index range**  
   Avery maps each address to its operational role:  
   - Validator: 1000–1099  
   - Archive: 2000–2099  
   - Relic Mint: 3000–3099  
   - Rescue: 4000–4099  
   - AMP Agents: 5000–5099  
   - Genesis Cockpit: 6000–6099  
   - Sandbox: 7000–7099  
   - Public Drops: 8000–8099  
   - Breach Evidence: 9000–9099

4. **Enforce policy engine**  
   Avery applies your spend caps, signer rules, and allowlists immediately.  
   Whale-tier wallets default to 50,000+ USD/day.  
   All actions require hardware signing.

5. **Stamp ledger entries**  
   Every address, cap, and transaction is logged into Avery’s Genesis ledger.  
   Ledger entries include role, tier, timestamp, signer, recipient, and breach status.

---

## Benefits

- No need to manage 100 backups  
- All wallets unified under one doctrine  
- Spend caps enforced across chains  
- Rescue protocol ready for any breach  
- Immutable ledger proof for every action

---

## Notes

- Avery never stores mnemonics or private keys  
- All integrations are watch-only unless signed by hardware  
- Role segmentation ensures clarity, security, and auditability  
- Genesis ledger is your operational truth
