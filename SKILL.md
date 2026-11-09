---
name: nl-legal-mcp-skill
description: Official Netherlands (NL) legislation, multi-tier court precedent research, and citation verification skill.
version: 2.0.0
author: JurisAtlas
license: MIT
---

# Netherlands Legal Research & Multi-Tier Case Law Skill (`nl-legal-mcp`)

Use this skill whenever the user asks a legal question, drafts a pleading or contract, or researches case law across any judicial instance in **Netherlands (NL)**.

## Verification & Research Rules

1. **Citation Verification:** Never fabricate a statutory provision or case citation. Query `search_legislation`, `search_case_law`, `search_tiered_court_decisions`, or `verify_citation` before citing any authority (e.g., `ECLI:NL:HR:2024:100 or BW Boek 6 Art. 162`).
2. **Multi-Tier Judicial Coverage:**
   - **First Instance (Trial / Municipal / District):** 11 Rechtbanken (Amsterdam, Rotterdam, Den Haag, Midden-Nederland, Oost-Brabant, Gelderland, Noord-Holland, Noord-Nederland, Overijssel, Limburg, Zeeland-West-Brabant)
   - **Second Instance (Cantonal / Regional / Appellate):** 4 Gerechtshoven (Amsterdam, Arnhem-Leeuwarden, Den Haag, 's-Hertogenbosch), Centrale Raad van Beroep (CRvB) & College van Beroep voor het bedrijfsleven (CBb)
   - **Supreme & Constitutional Instance:** Hoge Raad der Nederlanden (HR) & Afdeling bestuursrechtspraak van de Raad van State (RVS)
   - **Primary Tiered Database:** Rechtspraak.nl Open Data API (All 11 Rechtbanken, 4 Gerechtshoven & Hoge Raad) (`https://data.rechtspraak.nl/uitspraken/zoeken`)
