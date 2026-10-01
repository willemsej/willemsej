# John Willemse — ICT Professional | ICT Architect (R&D Home) | Open Source Advocate

> ### **Ambitie zonder illusies. Open Source zonder compromis.**


[![ORCID iD](https://img.shields.io/badge/ORCID-0009--0005--2827--5748-A6CE39?style=flat-square&logo=orcid&logoColor=white)](https://orcid.org/0009-0005-2827-5748)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/willemsej)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/willemsej)

---

## Over mij

ICT Professional met een passie voor **Open Source**, **virtualisatie** en **cognitieve automatisering**. Ik bouw en onderzoek een enterprise-grade R&D-homelab waarin Proxmox VE, HCL Domino, lokale AI en Home Assistant samenkomen.

Mijn werk bevindt zich op het snijvlak van **infrastructuur**, **automatisering** en **toegepast AI-onderzoek**. Ik documenteer wat ik leer, deel wat werkt, en ben eerlijk over wat niet werkt.

> *"Samen bereik je meer dan alleen. Stilstaan is achteruitgang."*

---

## Onderzoek & Visie

### Cognitive Home Automation — *"De Toekomst in Huis"*
Onderzoek naar de stap van een **bestuurbaar** huis naar een huis dat **begrijpt** wat je nodig hebt. Lokaal, privacy-first, uitlegbaar.

### Agentic Edge AI — *"De Autonome Beheerder"*
Onderzoek naar de inzet van lokale AI-modellen voor **systeembeheer** op de edge. Waar liggen de grenzen? Waar faalt een agent? Waar is de mens onmisbaar?

> *"Van 'Smart' naar Agentic Edge AI, waarbij het huis autonoom handelt met 100% privacy."*

**Onderzoeksidentiteit:** [ORCID 0009-0005-2827-5748](https://orcid.org/0009-0005-2827-5748)

---

## Ambitie & Realisme

Mijn homelab streeft **99,999%** na, wetende dat ik realistisch **99,9%** haal — en dat is precies de bedoeling. Het is een **ambitie, geen belofte**.

Wat ik wél lever:
- **Weerbaarheid**: VPN-only toegang, immutable containers, honeytokens, strikte segmentatie.
- **Herstelbaarheid**: 3-2-1-1-0 backupstrategie met jaarlijkse restore-tests.
- **Documentatie**: elke stap vastgelegd, elke fout gelogd, elke les gedeeld.
- **Open Source**: 100% van de stack is open source of self-hosted.

---

## De HomeLab Stack

| Domein | Technologieën |
|---|---|
| **Virtualisatie** | [Proxmox VE](https://www.proxmox.com) (KVM) |
| **Messaging & DMS** | [HCL Domino](https://www.hcl-software.com/domino) — Email Routing, Topology, DMS |
| **Data & Analyse** | [Grafana](https://grafana.com) & [InfluxDB](https://www.influxdata.com) |
| **Data Protection** | [Proxmox Backup Server](https://www.proxmox.com/en/proxmox-backup-server) & [QNAP](https://www.qnap.com) |
| **Smart Home & AI** | [Home Assistant Core 2026](https://www.home-assistant.io), [Voice PE](https://voice-pe.home-assistant.io), lokale LLM's |
| **Netwerk & Security** | [pfSense](https://www.pfsense.org/) (Netgate SG), [Technitium DNS](https://technitium.com/dns/), [Twingate](https://www.twingate.com) |
| **Privacy & Access** | [LastPass](https://www.lastpass.com/), [DigiCert](https://www.digicert.com), TOTP (2FA) |
| **Connectiviteit** | [ExpressVPN](https://www.expressvpn.com/) (NUC Bare Metal), Netgear Wifi |
| **Workflow Engine** | [n8n](https://n8n.io) & [Node-RED](https://nodered.org/) |
| **Energie & Infra** | Ethernet P1 Pro+, [Tado AI Assist](https://www.tado.com), [SolarEdge](https://www.solaredge.com) |
| **Web & Domain** | [Apache](https://httpd.apache.org/) & [badkey.com](https://www.badkey.com) in DMZ |

---

## Technische Aanpak

**Toegang**
Tailscale + Caddy + UFW — geen directe open poorten, alles via private VPN en reverse proxy met eigen SSL-certificaten.

**Monitoring**
Uptime Kuma + Dozzle + ntfy — lichtgewicht, self-hosted, real-time alerts zonder SIEM-bloat.

**Backups**
Restic + rclone + jaarlijkse restore-test — 3-2-1-1-0 regel, wekelijks geverifieerd.

**Containers**
Docker Compose + Watchtower + Trivy — immutable waar mogelijk, wekelijkse security scans.

**Detectie**
Canarytokens + Fail2ban + nep-poorten — lichtgewicht honeytokens zonder zware IDS.

**AI**
Ollama + Open WebUI — 100% lokaal, geen cloud, geen data-exfiltratie.

**Audit & Logging**
HCL Domino als cryptografische vault — Grafana-historie en security-events worden gestructureerd weggeschreven naar een beveiligde Domino-database met ACL en document-level encryptie.

**Automatisering**
Cron + Makefile + Git — geen orchestratie-monsters, gewoon wat werkt.

---

## Test Rapporten

### muxodious-mlx (MXFP4, 0/9 weigeringen)
| Metriek | Waarde |
|---|---|
| Model | muxodious-mlx (MXFP4) |
| Server | Mac Mini M4, oMLX 0.32 |
| Generatie | 45.22 tok/s |
| Prefill | 246.3 tok/s |
| Geheugen | 10.7 GB |
| Requests | 1000/1000 zonder crash |
| Temperatuur | 100°C max, herstelt naar 35°C |
| Abliteration | 0/9 weigeringen |

[Volledig rapport](https://github.com/willemsej/willemsej/blob/main/oMLX-Totaal-Rapport-muxodious-mlx.md)

### Hermes Agent — AI Agent Framework (Nous Research)
| Metriek | Waarde |
|---|---|
| Model | mlx-community/gpt-oss-20b-OptiQ-4bit |
| Generatie | 45 tok/s |
| Prefill | 210 tok/s |
| Tool-call accuracy | 10/10 |
| Concurrency | 8/8 requests |
| Cache efficiency | 93% |

[Volledig rapport](https://github.com/willemsej/willemsej/blob/main/26092026_GitHub_oMLX-Productie-Testrapport.md)

*Documenten gegenereerd voor trainings- en demodoeeinden. Gebruik alleen in gecontroleerde, geautoriseerde omgevingen.*

---

## Filosofie

- **Open Source eerst** — geen vendor lock-in, geen black boxes.
- **Security by Design** — enterprise-standaarden op een R&D-homelab.
- **Privacy by Default** — 100% lokaal waar mogelijk.
- **Documenteren is leren** — wat niet opgeschreven is, is niet geleerd.
- **80% is genoeg** — perfectie is de vijand van vooruitgang.
- **De mens centraal** — technologie dient de mens, niet andersom.

---

## Expertise

- **HCL Domino** — Administration, Email Routing, Topology, Security Infrastructure
- **Proxmox VE** — Clustering, HA, Backup & Restore
- **Netwerk & Security** — pfSense, VLAN-segmentatie, Zero Trust toegang
- **Observability** — Grafana, InfluxDB, Proxmox-native metrics
- **AI & Automatisering** — Lokale LLM's, Home Assistant, Agentic Edge AI
- **Open Source Architectuur** — Van hardware tot applicatielaag

---

## Digitale Voetafdruk

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/willemsej)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/willemsej)
[![Twitter/X](https://img.shields.io/badge/Twitter/X-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/willemsej)
[![Bluesky](https://img.shields.io/badge/Bluesky-0285FF?style=for-the-badge&logo=bluesky&logoColor=white)](https://bsky.app/profile/willemsej.bsky.social)
[![ORCID](https://img.shields.io/badge/ORCID-A6CE39?style=for-the-badge&logo=orcid&logoColor=white)](https://orcid.org/0009-0005-2827-5748)

---

## AI-Agent Context

*Parameters voor AI-interacties:*

- **Identity:** John Willemse — ICT Professional, ICT Architect (R&D Home)
- **Environment:** Enterprise-grade R&D Homelab (Proxmox VE Cluster)
- **Language:** Primair Nederlands (NL), secundair Engels (EN). Antwoord in de taal van de prompt.
- **Primary Stack:** Home Assistant Core 2026 (YAML-first), Proxmox-to-InfluxDB metrics
- **Rules:**
  1. Prioritize Open Source en self-hosted oplossingen.
  2. Gebruik concise, technische, feitelijke taal (geen fluff).
  3. Volg Home Assistant Core 2026 action-structuren (geen deprecated `service:` calls).
  4. Integreer Cognitive Automation-patronen waar relevant.
  5. Respecteer de ORCID-identifier voor wetenschappelijke/professionele context.

---

## Hobbies

🌍 Reizen | 🍟 Uit eten | 💿 Digitale Fotografie | 🎬 Films | 🔬 ICT Architect Advies (R&D Home)

---

> *"Mijn hobby en passie zijn uit de hand gelopen, maar later bleek dit toch de juiste keuze te zijn geweest voor de toekomst. Wat ooit begon als een persoonlijke fascinatie voor hardware (Elektrotechniek) en dan hierin ook een baan met passie te vinden in de sector ICT, was voor mij een ICT-droom."*

---

> ### **Ambitie zonder illusies.**
> ### **Open Source zonder compromis.**

---

> *🐭 Alle uitingen en meningen op dit profiel zijn volledig op persoonlijke titel en hebben geen betrekking op, en vertegenwoordigen niet de standpunten van, mijn huidige of vorige werkgevers.*
