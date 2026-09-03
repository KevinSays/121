# Bastion Security — Teaching Kit

A netrunner/hacker-terminal approach to teaching cybersecurity fundamentals.
Bastion Security is a fictional managed SOC (security operations center)
that protects client companies; the student is a newly hired Tier-1
analyst — effectively the ICE standing between a client network and the
threat actors and attack techniques filed here. Every recurring threat type
gets a dossier; every session's content reads loosely as a case reviewed on
shift. Built for classroom handouts and lecture read-alouds — the
cybersecurity-essentials counterpart to IT131's "OSI Company" kit, though
IT121 uses its own dark cyberpunk visual identity rather than IT131's kraft
paper (changed 2026-09-03, at the user's request).

## Files

- `bastion-threat-board.html` — Dossier board. One card per threat actor
  category from Module 1: MO, tools of the trade, countermeasure, threat
  level, and a cross-reference back to Session 1.
- `bastion-attack-log.html` — Dossier board, same component. One card per
  foundational-protocol attack from Module 3: ARP spoofing, IP spoofing,
  ICMP abuse, TCP SYN flood, DNS cache poisoning, DHCP spoofing/starvation —
  cross-referenced back to Session 2.

## Design system

IT121's own palette — not shared with IT131. Near-black background with a
faint cyan scanline texture; neon-glow borders and shadows instead of paper
shadows; no card rotation (digital panels don't tilt, unlike IT131's pinned
paper posters).

**Palette**
| Token | Hex | Use |
|---|---|---|
| `--paper` | `#0d1619` | Card/panel background |
| `--canvas` | `#070b0d` | Page background |
| `--ink` | `#d8fff2` | Body text, pale-cyan card borders |
| `--kraft` | `#ff2e88` | Dossier field labels (MO, tools, countermeasure) |
| `--blue` | `#2de2e6` | Primary accent — links, card borders, status LEDs |
| `--red` | `#ff4d4d` | Threat-level pips, danger accents |

**Type** (Google Fonts, loaded via `<link>` in each file's `<head>`)
- Display / headers: `Orbitron` (futuristic marquee)
- Body prose: `Rajdhani` (technical HUD feel)
- Data, labels, dossier fields: `IBM Plex Mono`

**Recurring conventions**
- Small glowing status-LED dot (`.pin`) at top-center of each card instead
  of IT131's pushpin; neon box-shadow (`0 0 0 1px rgba(45,226,230,.15), 0 0
  24px rgba(45,226,230,.12)`) instead of offset hard-shadow
- `text-shadow` glow on headers/eyebrows/kickers for the neon-marquee look
- Dashed rules (`1px dashed rgba(45,226,230,.25)`) for section dividers
- `@media print` rules included for handout printing (forces a light
  background so posters actually print legibly)

## Cast reference

**Threat actors (filed on the Threat Board):** Script Kiddie · Hacktivist ·
Organized Crime · Nation-State / APT · Insider Threat.

**Foundational-protocol attacks (filed on the Attack Log):** ARP Spoofing ·
IP Spoofing · ICMP Abuse · TCP SYN Flood · DNS Cache Poisoning · DHCP
Spoofing/Starvation.

**Recurring mentor (not yet introduced):** the Shift Lead — planned for the
first episode script, will walk a case from alert to resolution the way
IT131's NOC character does for ARP spoofing.

## Open threads

- Personnel Directory (Bastion's own SOC roles — Tier 1/2 analyst, threat
  intel, DFIR, GRC) not yet built; natural pairing is once those modules
  (20–22, 24, 27) are filed.
- Episode 01 not yet written — strongest first case is a phishing incident,
  since Session 1 already covers social engineering and threat actors.
