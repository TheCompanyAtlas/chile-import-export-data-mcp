# Chile Import Export Data MCP

**Chile Customs Data: Importers, Suppliers & HS Codes.** Chile import export data for your AI assistant. Search Chile customs shipment records, find importers and foreign suppliers, and break down trade by HS code, partner country and counterparty company, through the Model Context Protocol.

An AI-native alternative to Chile trade data from Panjiva, ImportGenius, Volza, Seair, TradeInt and ExportGenius: ask in plain language instead of exporting spreadsheets.

The MCP connection is provided by [The Company Atlas](https://thecompanyatlas.com). This repository does not run a separate server.

## Connect

```
https://thecompanyatlas.com/mcp/trade/chile
```

Add this URL as a custom MCP connector in Claude, ChatGPT, Cursor, or any MCP-compatible client. Sign in with Google when prompted.

- Transport: Streamable HTTP
- Auth: Google OAuth (sign in once, stays authorized)
- Free accounts get 50 credits per calendar month
- Defaults to Chile: the server tells your AI to filter on `CL` unless you ask about another country

## Chile data coverage

- **Years:** 2019–2026
- **Records:** Import declarations: Chilean importer, foreign supplier, origin country, HS code, goods description, value, quantity, port and date.
- **Country code:** `CL` (use `buyerCountry: "CL"` for imports into Chile)
- **Common products:** mining and earth-moving machinery (HS 8429), refined fuel (HS 2710), cars (HS 8703), phones (HS 8517)

## Notable traders in the data

Companies that appear most often in recent Chile records (by number of declaration lines, not value):

**Importers**

- Copec
- ENAP Refinerías
- Komatsu Chile
- Finning Chile
- Apple Chile
- Derco

## Example prompts

- *"Who are the top importers of mining machinery (HS 8429) into Chile?"*
- *"What does Komatsu Chile import, by HS code?"*
- *"List Chilean importers of cars (HS 8703) in 2025"*
- *"Which suppliers ship fuel to ENAP Refinerías?"*
- *"Show recent import shipments for Apple Chile"*

## Tools

### Trade search

| Tool | Description |
|---|---|
| `Trade_search_trades` | Paginated customs shipment search: filter by HS code, buyer, seller, country, port, value and date range |
| `Trade_company_trade_volume_by_year` | Rank importers or exporters by declared value and line counts per year, with HS code and country filters |

### Trade analytics

| Tool | Description |
|---|---|
| `Trade_hs_code_breakdown` | For one company, import and export value by HS chapter, heading or subheading |
| `Trade_year_country_breakdown` | For one company, trade value by year and counterparty country |
| `Trade_partner_breakdown` | For one company, trade value by year and matched counterparty company |

### Company registry

| Tool | Description |
|---|---|
| `Company_search` | Search the global company registry by name or id, with optional country filter |
| `Company_get_by_id` | Full company profile by id |

## Keywords

Chile import data, Chile export data, Chile customs data, Chile shipment data, importers in Chile, Chile buyers and suppliers, HS code search, datos de importación Chile, importadores de Chile, comercio exterior, Aduana, código arancelario
