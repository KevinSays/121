# Bastion Security — Teaching Kit

An Edo-period castle-town approach to teaching cybersecurity fundamentals.
Bastion Security is a fictional managed SOC (security operations center)
that protects client organizations. The student is a newly hired Tier-1
analyst, a new guard on the watch. A *bastion* is a fortification, so concepts
are explained through one world: a castle town of Edo-period Japan
(1603–1868), with its walls, checkpoints, watchtowers, couriers, and the
shinobi who try to get past them. The clients and systems are modern. The
castle town is only the lens. Every recurring threat type gets a dossier, and
every session's content reads loosely as a case reviewed on shift. Built for
classroom handouts and lecture read-alouds. It's the cybersecurity-essentials
counterpart to IT131's "OSI Company" kit. (Visual identity changed from a dark
cyberpunk look to washi paper on 2026-10-01, at the user's request.)

## Files

- `bastion-threat-board.html` — Dossier board. One card per threat actor
  category from Module 1: MO, tools of the trade, countermeasure, threat
  level, and a cross-reference back to Session 1.
- `bastion-attack-log.html` — Dossier board, same component. Six cards:
  Module 3 (IP spoofing, ICMP abuse, TCP SYN flood, cross-referenced to
  Session 2) plus Module 4 (ARP cache poisoning, DNS cache poisoning, DHCP
  spoofing/starvation, cross-referenced to Session 3, filed once that
  session existed — don't add a module's dossiers before its session is
  actually built).

## Design system

Washi paper: sumi-ink text on cream paper, vermilion and gold accents, and a
faint *seigaiha* (wave) texture. It's light like IT131's kraft paper, but IT121 is set apart
by its Japanese typefaces, the wave texture, and the vermilion/gold palette.
No card rotation.

**Palette** (all colors pass WCAG AA on the paper tones)
| Token | Hex | Use |
|---|---|---|
| `--paper` | `#fbf8f0` | Card/panel background |
| `--canvas` | `#f4eee1` | Page background (washi) |
| `--ink` | `#2b2420` | Body text, card borders (sumi) |
| `--kraft` | `#7d590d` | Dossier field labels (MO, tools, countermeasure), gold |
| `--blue` | `#b23a1e` | Primary accent: links, card borders, status dots (vermilion; token name kept for compatibility) |
| `--red` | `#b0213d` | Threat-level pips, danger accents (crimson) |

**Type** (Google Fonts, loaded via `<link>` in each file's `<head>`)
- Display / headers: `Shippori Mincho B1` (Japanese Mincho serif with Latin)
- Body prose: `Zen Kaku Gothic New`
- Data, labels, dossier fields: `IBM Plex Mono`

**Recurring conventions**
- Small vermilion dot (`.pin`) at top-center of each card instead of IT131's
  pushpin; soft warm shadows, no glow
- Dashed rules for section dividers
- `@media print` rules included for handout printing

## Cast reference

**Threat actors (filed on the Threat Board):** Script Kiddie · Hacktivist ·
Organized Crime · Nation-State / APT · Insider Threat.

**Attack techniques (filed on the Attack Log):** Module 3 — IP Spoofing ·
ICMP Abuse · TCP SYN Flood. Module 4 — ARP Cache Poisoning · DNS Cache
Poisoning · DHCP Spoofing/Starvation.

**Clients (Bastion protects these; examples and labs use them):**
Kiriyama General Hospital (regional hospital: EHR, imaging, 24/7 ops) ·
Tsukimi Sweets (small family confectionery: website, POS, shop Wi-Fi) ·
Kaidō Freight (mid-size logistics: Windows domain, Linux servers, warehouse
Wi-Fi, VPN). The Threat Board is styled as a *kōsatsu* (public notice board),
the Attack Log as a guardhouse ledger.

**Recurring mentor (not yet introduced):** the Shift Lead — planned for the
first episode script, will walk a case from alert to resolution the way
IT131's NOC character does for ARP spoofing.

## Open threads

- Personnel Directory (Bastion's own SOC roles — Tier 1/2 analyst, threat
  intel, DFIR, GRC) not yet built; natural pairing is once those modules
  (20–22, 24, 27) are filed.
- Episode 01 not yet written — strongest first case is a phishing incident,
  since Session 1 already covers social engineering and threat actors. Note
  `../labs/phishing-triage.html` covers similar ground as a worksheet, not
  a narrative episode — the two aren't a substitute for each other.
