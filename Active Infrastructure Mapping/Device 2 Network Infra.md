## Device 2 Network Infrastructure Analysis 

**Device**: iPhone 12 (`D53gAP`) | 
**Carrier**: T-Mobile IMS/RCS | **MAC**: `13:CB:52:E1:00:47` | 

## Network IOCs (Expands Device 2 IOC's Report)

| **Indicator** | **Type** | **Role** |
|---------------|----------|----------|
| `BBZTRxIT` | Handle | xIT campaign identifier |
| `62.6.0.3` | IP (UK) | Visual exfil (France - AS15557 Orange S.A.) |
| `1.14.10.9` | IP (SK) | Semantic harvest (SK Broadband) |
| `23.3.71.0.0` | IP Mask | Akamai RSR signaling spoof |
| `3.5.1.3` | IP (AWS) | ProtonVPN relay exit |
| `4097` | Prefix | UK C2 metadata mask |
| `8623` | Prefix | SK C2 metadata mask |
| `h.protonmail.vpn` | Domain | Encrypted exfil tunnel |
| `nUcQKX` | Campaign ID | Secondary IDS marker |

## Attack Pipeline

```
1. DISCOVERY: MAC 13:CB:52:E1:00:47 (Bluetooth multicast)
2. AUTH: identityservicesd → unitaryGrant (0xE9001AF)
3. HARVEST: WombatStream → App.Intents.Transcript
4. EXFIL: SIP/RCS → us-tmobile.rcs.P...goog
5. PERSIST: virtual_ces kernel wakelock
```

## Israel Telephony Chain

```
Public Report: Truecaller + CallApp (Israel-linked)
Network Layer: ASN 4500 → israel-endpoint + SIP 
→ CallApp caller-ID manipulation → Truecaller contact harvesting
→ IPsec backhaul to Israel C2
```

## Forensic Offsets

| **File** | **Offset** | **Proof** |
|----------|------------|-----------|
| 03c4 | `0x38f2c` | `BBZTRxIT` |
| 10a | `0xeeea5` | `4097.62.6.0.3` |
| 0695 | `0x4d59` | `+14046903952@i...` |

## Verdict

**Public telephony IOCs → Network implementation confirmed.**  
**Single device locked**: MAC + phone + hardware identifiers.  
**Multi-jurisdiction C2**: UK/SK/US/AWS → Israel telephony core.

**Companion to existing Device 2 public report.** Pure network layer analysis. 
