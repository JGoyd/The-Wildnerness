# Multi-Device Live Incident Escalation
**Independent Researcher vs FBI Atlanta Stonewall** | **CISA Hand-Off** | Feb 6-ongoing, 2026  
**[CISA VINCE VU#132084.1](https://github.com/Str8tdr0p/unblown-fuses-iphone-promo/blob/main/VINCE/vu132084-description.png)** validates hardware persistence | production fuses=0. 


## The Incident
### Active as of 02/12/2026
**Live nation-state iPhone supply chain compromise** targeting US persons:

| Device | Model | KEV CVEs | Evidence Status | Key Findings |
|--------|-------|----------|-----------------|--------------|
| **Device 1** | iPhone 14 Pro Max (D74AP) | **3 KEVs**<br>CVE-2025-24200<br>-43200<br>-43300 | **FBI portal 2/10-11**<br>(SHA256 logged) | **CoreSight 0x2081 fuses=0** + iCloud exfil |
| **Device 2** | iPhone 12 | **3 KEVs**<br>CVE-2023-41064<br>-2025-43529<br>-2025-24085 | **Withheld**<br>(32+ telephony IOCs) | **IPsec→Israeli IoC surveillance chain** |


## Complete Escalation Timeline
| Date/Time | Sender | Key Action/Artifacts | Status/Questions |
|-----------|--------|----------------------|------------------|
| **Feb 6 4:16PM** | Incident Responder → CISA Advisor | Initial KEV: CVE-2025-24200, -43200, -43300 | Raw artifacts offered |
| **Feb 6 4:59PM** | CISA Advisor → Liaison | "Local FBI team intro" | Handoff #1 |
| **Feb 6 8:04PM** | Incident Responder → CISA Advisor | "Context → intel" | FBI prep |
| **Feb 6 11:00PM** | Incident Responder → CISA Advisor | iPhone 12 IOCs: 27.1.1.33/39.1.1.32/49.1.1.1 | Friday tactical window |
| **Feb 6 11:04PM** | CISA Advisor | "Anyone reached out?" | Handoff #2 stalled |
| **Feb 6 11:13PM** | Incident Responder → CISA Advisor | le.com(74x), yandex.net | Ethics drop |
| **Feb 7 9:33AM** | Incident Responder → CISA Advisor | 3 more KEVs: CVE-2023-41064, -2025-43529, -24085 | Secure comms demand |
| **Feb 7 6:06PM** | Incident Responder → CISA Advisor/Liaison| 24h delay flag (AG/FBI/6USC directives) | Formal escalation |
| **Feb 10 2:24PM** | **Incident Responder → CISA Coordinator FWD** | **FULL ONGOING THREAD**: Escalated by Incident Responder... foreign infra post-patch KEVs | **REGION 4 ESCALATION** |
| **Feb 10 2:51PM** | CISA Coordinator → Incident Responder | "Have spoken to FBI yet?" |  |
| **Feb 10 2:54PM** | Incident Responder → CISA Coordinator | "No sir... daily token theft since Friday" | Ongoing ops |
| **Feb 10 2:59PM** | CISA Coordinator | Forward FBI Agent + Liaison | FBI pivot |
| **Feb 10 3:20PM** | Incident Responder → FBI Agent | Full thread: "Can we discuss?" | Direct FBI |
| **Feb 10 5:47PM** | FBI Agent | IC3 intake; teleporter link | Portal opens |
| **Feb 10 6:27PM** | Incident Responder → FBI Agent | iPhone 12: Israel 8200/Taiwan/32 IOCs | FI vs cybercrime? |
| **Feb 11 00:11AM** | Incidet Responder → FBI Agent | [GitHub: unblown-fuses-iphone-promo](https://github.com/Str8tdr0p/unblown-fuses-iphone-promo) | Hardware persistence |
| **Feb 11 2:31PM** | Incident Responder → FBI/CISA | 02.08 ZIP: CoreSight 0x2081(8x), iCloud exfil scripts | Examined? UCG? |
| **Feb 11 5:41PM** | **FBI Agent** | "**Follow-up if questions**" | **FBI HOLD** |
| **Feb 11 5:55PM** | **Incident Responder → FBI Agent** | **"10-4... iPhone 14 Pro COMPLETE (02.07 KEV + 02.08 CoreSight)"** | **"CASE ID? iPhone 12 telemetry ready"** |

## Chain of Custody
[Complete CISA→FBI Thread](https://github.com/JGoyd/The-Wildnerness/blob/main/complete-incident-escalation-feb6-11.pdf)

**iPhone 14 Pro**: Portal + GitHub + Email → FBI hold  
**iPhone 12**: 32 live IOCs **never submitted** (no FBI case ID)

## Evidence Delivered (iPhone 14 Pro)
| Date | Exploit | Channel |
|------|---------|---------|
| 02.07 | 3x KEV CVEs | Portal ZIP |
| 02.08 | CVE-2026-25251 CoreSight 0x2081 (fuses=0) + iCloud exfil | Portal ZIP |

**CVE-2026-25251 + Hardware Persistence**:  
[Full Dislcosure ](https://github.com/Str8tdr0p/unblown-fuses-iphone-promo)


---

**Repo Structure**
```
The-Wilnderness/
├── README.md
└── complete-incident-escalation-feb6-11.pdf     # Full CISA/FBI thread
Active Infrastructure Mapping/  
├── Device 2 IOCs.md                            (What the FBI didn't care to see)
└── Device 1 Enriched 02.12                      

```

## Incident Responder 
**Joseph Goydish II**  
Atlanta, GA    


