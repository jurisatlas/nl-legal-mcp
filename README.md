# Netherlands Legal Research MCP Server (`nl-legal-mcp`)

**[Nederlands](#lang-nl) | [English Documentation](#english-documentation)**

---

<a id="lang-nl"></a>
## Juridische MCP-server voor Wetgeving en Rechtspraak (`nl-legal-mcp`) — Nederlands

### Over deze repository

Deze repository bevat een Model Context Protocol (MCP) server die uw AI-assistent (Claude Desktop, Cursor, Windsurf, VS Code / Copilot, Cline, Continue.dev of Antigravity) rechtstreeks verbindt met de officiële wetgevingsportalen en rechtspraakdatabanken voor **Netherlands** (rechtbanken van eerste aanleg, gerechtshoven / hoven van beroep en hoogste rechtscolleges).

### Installatie (Selecteer uw AI-applicatie)

1. **Downloaden:** Klik rechtsboven op **`<> Code` -> `Download ZIP`** en pak de map uit op uw computer.
2. **Starten:** Dubbelklik op **`Click_Here_To_Install_Windows.bat`** (Windows) of **`Click_Here_To_Install_Mac.command`** (macOS).
3. **AI-client kiezen:** Vink de AI-programma's aan die u gebruikt (Claude, Cursor, Windsurf, VS Code, Antigravity), klik op installeren en herstart uw gekozen AI-applicatie.

**Veiligheidsopmerking:** Dit hulpprogramma werkt uitsluitend in alleen-lezen modus en raakt geen persoonlijke bestanden op uw computer aan.

### Rechterlijke hiërarchie en officiële bronnen

| Instantie | Gedekte gerechten |
|:---|:---|
| **Eerste aanleg (Rechtbanken)** | 11 Rechtbanken (Amsterdam, Rotterdam, Den Haag, Midden-Nederland, Oost-Brabant, Gelderland, Noord-Holland, Noord-Nederland, Overijssel, Limburg, Zeeland-West-Brabant) |
| **Hoger beroep (Hoven van beroep / Gerechtshoven)** | 4 Gerechtshoven (Amsterdam, Arnhem-Leeuwarden, Den Haag, 's-Hertogenbosch), Centrale Raad van Beroep (CRvB) & College van Beroep voor het bedrijfsleven (CBb) |
| **Hoogste en Grondwettelijke Gerechtshoven** | Hoge Raad der Nederlanden (HR) & Afdeling bestuursrechtspraak van de Raad van State (RVS) |

- **Wetten.overheid.nl (KOOP Open Data SRU API):** [https://wetten.overheid.nl](https://wetten.overheid.nl) (`wetten.overheid.nl`, `officielebekendmakingen.nl`)
- **Rechtspraak.nl Open Data API (All 11 Rechtbanken, 4 Gerechtshoven & Hoge Raad):** [https://uitspraken.rechtspraak.nl](https://uitspraken.rechtspraak.nl) (`uitspraken.rechtspraak.nl`, `rechtspraak.nl`, `hogeraad.nl`, `raadvanstate.nl`)

---

<a id="english-documentation"></a>
## English Documentation

Model Context Protocol (MCP) server providing live, read-only access to **Netherlands (NL)** legislation, official gazettes, multi-tier judicial decisions (First Instance, Regional/Cantonal/Appellate, and Supreme/Constitutional courts, including HTML and PDF full-text extraction), and statutory citation verification across all major AI clients (**ChatGPT Desktop, OpenAI Codex CLI, Claude Desktop, Claude Code CLI, Cursor, Windsurf, VS Code / GitHub Copilot / Cline / Roo Code, Google Antigravity / Gemini CLI, Perplexity, and Continue.dev**).

---

### Interactive Desktop Setup (Select Your AI Assistant)

This package includes a graphical installer for legal practitioners and non-technical users that lets you select which AI application(s) you use:

1. **Download:** Click **`<> Code`** at the top right of this repository, select **`Download ZIP`**, and extract the folder to your computer.
2. **Run the Setup Utility:**
   - **Windows:** Double-click `Click_Here_To_Install_Windows.bat`
   - **macOS:** Double-click `Click_Here_To_Install_Mac.command`
3. **Select Your AI Client(s) & Connect:** Check the box(es) for the AI assistant(s) installed on your computer (**ChatGPT Desktop & OpenAI Codex CLI**, **Claude Desktop & Claude Code CLI**, **Cursor**, **Windsurf**, **VS Code / GitHub Copilot / Cline / Roo Code**, **Google Antigravity / Gemini CLI**, or **Perplexity / Continue.dev**), click **Install to Selected AI Clients**, and restart your selected AI application.

**System Integrity Note:** The setup utility operates strictly in read-only mode with respect to your personal files and documents. It installs an isolated Python runtime inside the extracted folder and registers the server entry only in the AI client configuration files you select.

---

### Multi-Tier Judicial Hierarchy & Live Indexed National Archives

This server performs live queries across the full judicial hierarchy and official legal archives of **Netherlands**, extracting full text from both HTML pages and official court/gazette PDF judgments:

| Judicial Tier | Covered Courts & Tribunals |
|:---|:---|
| **Tier 1 — First Instance** | 11 Rechtbanken (Amsterdam, Rotterdam, Den Haag, Midden-Nederland, Oost-Brabant, Gelderland, Noord-Holland, Noord-Nederland, Overijssel, Limburg, Zeeland-West-Brabant) |
| **Tier 2 — Regional / Cantonal / Appellate** | 4 Gerechtshoven (Amsterdam, Arnhem-Leeuwarden, Den Haag, 's-Hertogenbosch), Centrale Raad van Beroep (CRvB) & College van Beroep voor het bedrijfsleven (CBb) |
| **Tier 3 — Supreme & Constitutional** | Hoge Raad der Nederlanden (HR) & Afdeling bestuursrechtspraak van de Raad van State (RVS) |

#### Official Portals & Live Indexed Domains

- **National Legislation & Official Gazette:** Wetten.overheid.nl (KOOP Open Data SRU API) — [https://wetten.overheid.nl](https://wetten.overheid.nl)
  - *Indexed Legislation Domains:* `wetten.overheid.nl`, `officielebekendmakingen.nl`
- **Court Decisions & Jurisprudence Archives:** Rechtspraak.nl Open Data API (All 11 Rechtbanken, 4 Gerechtshoven & Hoge Raad) — [https://uitspraken.rechtspraak.nl](https://uitspraken.rechtspraak.nl)
  - *Indexed Judicial & Open Case Law Domains:* `uitspraken.rechtspraak.nl`, `rechtspraak.nl`, `hogeraad.nl`, `raadvanstate.nl`

---

### Available MCP Tools

| Tool | Description |
|:---|:---|
| `search_legislation` | Searches enacted statutes, codes, decrees, and official gazette publications in Netherlands. |
| `search_case_law` | Searches national jurisprudence and open judicial archives for Netherlands. |
| `search_tiered_court_decisions` | Filters case law specifically by judicial instance (`first_instance`, `appellate_regional`, `supreme_constitutional`) or specific regional/cantonal/district court. |
| `list_court_hierarchy` | Returns the complete 3-tier court structure and supported regional court filters for Netherlands. |
| `get_legal_document_markdown` | Retrieves full statutory or judicial texts (both HTML and official `.pdf` court judgments) and converts them into clean Markdown. |
| `verify_citation` | Validates statutory and case law citations against official registries. |

---

<details>
<summary><b>Manual Configuration for Developers (Optional)</b></summary>

```json
{
  "mcpServers": {
    "nl-legal-mcp": {
      "command": "uvx",
      "args": [
        "--from",
        "https://github.com/jurisatlas/nl-legal-mcp/archive/refs/heads/main.zip",
        "nl-legal-mcp"
      ]
    }
  }
}
```
</details>
