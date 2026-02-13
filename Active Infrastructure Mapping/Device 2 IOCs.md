# Device 2 Foreign Infrastructure IOCs (FBI Never Received)

**Device**: iPhone 12 | **Status**: live telephony C2 indicators
**Timeline**: Feb 3-9, 2026 logs | **Researcher**: Solo tracking

## TELEPHONY C2 PATTERNS (PARTIAL RELEASE)
US ASN 4500 (ZAIX) → Israel telephony C2
Masquerading as "India" tunnel (geographic deception)
### Network Infrastructure Signatures 
| IOC Type | URL Pattern | Significance |
|----------|-------------|--------------|
| IPsec Tunnels | `US ASN 4500 (ZAIX) → Israel telephony C2` | No VPN apps |
| Telephony C2 | `apn-hijack.[tld]/*` | Carrier mods |
| DNS Overrides | `*.namecoin/dns/*` | Blockchain C2 |


## SURVEILLANCE SERVICES ECOSYSTEM (Hard IOCs - RELEASE)

### Hidden Services Installed
| Service | Primary Domain | Jurisdiction | Function | Evidence |
|---------|----------------|--------------|----------|----------|
| **GetContact** | `issuer.alci.getcontact` | Turkey | Privacy Pass issuer / Contact harvesting | tracev3 210-215 |
| **Truecaller** | `ios-live-lookup-eu.truecaller.com` | Sweden/Israel | Live caller ID lookup | tracev3 210-215 |
| **GetSimpler** | `livecallerid.prod.getsimpler.me` | Russia/Montenegro | Telephony interception | tracev3 210-215 |
| **SpamAngel** | `api-prd-v1.spamangel.org` | Unknown | Data aggregation endpoint | tracev3 210-215 |
| **Kaspersky KSN** | `ppt-issuer.ksn.kaspersky-labs.com` | Russia | Privacy Pass / PIR service | tracev3 210-215 |


### Hidden App Installed
| Bundle ID | App Name | Publisher | Install Type | Notes |
|-----------|----------|-----------|--------------|-------|
| `com.github.stormbreaker.prod` | GitHub | GitHub Inc | Customer | Developer tools |
| `com.callapp.*` | CallApp | Israel-linked | Caller ID manipulation |


**Fingerprint**: `LSInstallType=0`, `MIInstallationDomainSystemShared`, `Distributor: Unknown`



**This constitutes smoking-gun evidence** of nation-state grade telephony surveillance infrastructure hitting fully updated iPhone. 
