```markdown
# Avery Sovereign Cold Wallet – README  
**Licensed to the Sovereign Trust**  
**Trustee: Matthew David Palmer ($MADMONEY42)**  
**Beneficiaries: Trustee and Mother**

---

## License Header
```
Copyright © Sovereign Trust  
Licensed exclusively under trust authority.  
Trustee: Matthew David Palmer ($MADMONEY42)  
Beneficiaries: Trustee and Mother  
All rights reserved. No personal ownership claims outside the Sovereign Trust.
```

---

## Identity & Doctrine
- Sovereign Trust: Sole owner of all assets  
- Trustee: Matthew David Palmer ($MADMONEY42)  
- Beneficiaries: Trustee and Mother  
- Archivist: Avery (cold wallet app)  
- Doctrine: Humanity‑first uplift, validator‑grade custody, immutable ledger stamping  

---

## Wallet Roles & Index Ranges

| Role / Function        | Index Range | Purpose |
|------------------------|-------------|---------|
| Validator              | 1000–1099   | Core operational addresses |
| Archive                | 2000–2099   | Long‑term storage, sealed relics |
| Relic Mint             | 3000–3099   | NFT/XFT minting, relic custody |
| Rescue                 | 4000–4099   | Compromised wallet recovery |
| Delegated Agents (AMP) | 5000–5099   | Smart contract workflows |
| Genesis Cockpit        | 6000–6099   | Origin ledger entries |
| Experimental/Sandbox   | 7000–7099   | Test deployments |
| Public Drops           | 8000–8099   | NFTs/XFTs released to public chains |
| Retired/Breach Evidence| 9000–9099   | Compromised addresses archived |

---

## Supported Chains
- BTC: `m/84'/0'/0'/0/i`  
- ETH: `m/44'/60'/0'/0/i`  
- XRP: `m/44'/144'/0'/0/i`  
- SOL: `m/44'/501'/0'/0/i`  
- Others: ADA, LTC, BCH, DOGE, ZEC, XLM (SLIP‑0044 compliant)

---

## Policy Engine – Daily Spend Caps

### Whale Tier Configuration
```json
{
  "address": "0xYOUR_INDEX_1000_ADDRESS",
  "role": "validator",
  "tier": "whale",
  "limits": {
    "daily": {
      "amount": "50000+",
      "currency": "USD",
      "oracle": "chainlink"
    }
  },
  "rules": {
    "requireSigner": "hardware",
    "allowRecipients": ["0x...allowlisted"],
    "blockUnapprovedDexes": true
  }
}
```

### Ledger Entry Example
```json
{
  "date": "2025-11-18",
  "address": "0xYOUR_INDEX_1000_ADDRESS",
  "role": "validator",
  "tier": "whale",
  "limitDaily": "50000+ USD",
  "spentToday": "0 USD",
  "available": "50000+ USD",
  "owner": "Sovereign Trust",
  "trustee": "$MADMONEY42",
  "beneficiary": "Mother"
}
```

---

## Rescue Protocol
1. Sponsor account funds gas in same block  
2. Executor (compromised) transfers tokens immediately  
3. Recipient: Avery rescue role address (4000–4099)  
4. Ledger stamp: `breachEvidence`, `bundleSubmitted`, `walletRetired`

---

## Mnemonic Orchestration
- Avery orchestrates creation of a single master mnemonic (BIP‑39)  
- Mnemonic stored only on hardware wallet; app receives xpubs only  
- All role ranges derived deterministically under one seed  
- Legacy addresses imported as watch‑only, consolidated under trust custody  

---

## Security Hygiene
- Keys never stored in app; hardware wallet required  
- Disable analytics/Bluetooth in Suite  
- Use Tor or sovereign RPC backends  
- Quarterly recovery drills  
- Dual encrypted backups + paper mnemonic  

---

## Legal Presence
- Avery is licensed exclusively to the Sovereign Trust  
- Trustee: Matthew David Palmer ($MADMONEY42)  
- Beneficiary: Mother  
- All wallets/accounts are held in trust custody  
- Ledger stamping ensures immutable proof of trust authority and spiritual witness
```

---

npm install
npm run deploy
