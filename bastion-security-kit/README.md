# Bastion Security — Teaching Kit

A case-file approach to teaching cybersecurity fundamentals. Bastion
Security is a fictional managed SOC (security operations center) that
protects client companies; the student is a newly hired Tier-1 analyst.
Every recurring threat type gets a dossier; every session's content reads
loosely as a case file reviewed on shift. Built for classroom handouts and
lecture read-alouds — the cybersecurity-essentials counterpart to IT131's
"OSI Company" kit.

## Files

- `bastion-threat-board.html` — Wanted-poster board. One dossier per threat
  actor category from Module 1: MO, tools of the trade, countermeasure,
  threat level, and a cross-reference back to Session 1.

## Design system

Shared with the IT131 site — reuse these if you extend the set.

**Palette**
| Token | Hex | Use |
|---|---|---|
| `--paper` | `#EDE8DD` | Card/document background |
| `--canvas` | `#D9D2C3` | Page background |
| `--ink` | `#1F2421` | Body text, borders |
| `--kraft` | `#B08554` | Folder tabs, stat labels |
| `--blue` | `#2F4858` | "Analyst" stamps, teaching notes |
| `--red` | `#A23A2E` | Incident stamps, threat accents |

**Type** (Google Fonts, loaded via `<link>` in each file's `<head>`)
- Display / stamps / headers: `Special Elite` (typewriter)
- Body prose: `IBM Plex Sans`
- Data, labels, dossier fields: `IBM Plex Mono`

**Recurring conventions**
- Folder-tab / pin / stamp elements for card headers, offset hard-shadow
  (`5px 5px 0 rgba(31,36,33,0.16)`) instead of soft blur shadows
- Dashed rules (`2px dashed`) for tear-off / perforated sections
- `@media print` rules included for handout printing

## Cast reference

**Threat actors (filed on the Threat Board):** Script Kiddie · Hacktivist ·
Organized Crime · Nation-State / APT · Insider Threat.

**Recurring mentor (not yet introduced):** the Shift Lead — planned for the
first episode script, will walk a case from alert to resolution the way
IT131's NOC character does for ARP spoofing.

## Open threads

- Personnel Directory (Bastion's own SOC roles — Tier 1/2 analyst, threat
  intel, DFIR, GRC) not yet built; natural pairing is once those modules
  (20–22, 24, 27) are filed.
- Episode 01 not yet written — strongest first case is a phishing incident,
  since Session 1 already covers social engineering and threat actors.
