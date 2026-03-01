# NK Sprint 2026 — Live Klassement

Live sprintvierkamp tracker voor het Daikin NK Sprint 2026 in Thialf, Heerenveen.  
Haalt automatisch resultaten op van [liveresults.schaatsen.nl](https://liveresults.schaatsen.nl).

## Afstanden & Puntentelling

| Volgorde | Afstand | Divisor | Comp ♀ | Comp ♂ |
|----------|---------|---------|--------|--------|
| 1 | 1e 500m | 1 | C1 | C2 |
| 2 | 1e 1000m | 2 | C3 | C4 |
| 3 | 2e 500m | 1 | C5 | C6 |
| 4 | 2e 1000m | 2 | C7 | C8 |

**Punten** = tijd (seconden) ÷ divisor, afgekapt op 3 decimalen.  
**Tijden** worden afgekapt op 2 decimalen (37,087 → 37,08).  
**Totaal** = som van afstandspunten (geen extra afronding).  
**Verschil in seconden** = puntenverschil × divisor, afgerond op 2 decimalen.

## Klassement sortering

1. Meeste afstanden gereden → altijd bovenaan
2. Daarna: laagste puntentotaal

## Modules

- **Klassement** — Live stand met delta in seconden per afstand
- **Afstandsviews** — Per afstand: uitslag + live klassement sidebar met benodigde tijd voor P1
- **Head to Head** — Vergelijk twee rijders + 4 tiles: benodigde tijden voor P1 en target
- **Deelnemers** — Actief/inactief toggle (20 per gender)
- **WK Tickets** — Wie kwalificeert zich voor WK Sprint (♀ 2 tickets, ♂ 1 ticket)

## WK Sprint startbewijzen

Aangewezen: Femke Kok (♀), Jenning de Boo (♂), Joep Wennemars (♂).  
Te verdienen via NK: 2× vrouwen, 1× mannen (winnaar).

## Technisch

- **Data:** Jina Reader proxy → liveresults.schaatsen.nl
- **Poll:** elke 10 seconden
- **Event ID:** `2026_NED_0003`
- **Mobiel:** hamburger menu, responsive tabellen en tiles
- **Geen dependencies** — vanilla JS, HTML, CSS

## Deployen

Push `index.html`, `app.js` en `styles.css` naar GitHub Pages.
