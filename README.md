# The Mine Works for Gemini CLI

A Gemini CLI extension that connects nine remote MCP servers from
The Mine Works, 80 tools in total. Each server runs on Apify and is
reached over streamable HTTP. Nothing runs locally.

Pricing: pay per call on Apify, billed to your own Apify account. Current
prices for each tool are on the server's Apify Store page.

## Install

```
gemini extensions install https://github.com/themineworks/gemini-cli-extension
```

Gemini CLI asks for your Apify API token during install and stores it in
the system keychain. Get a token at
https://console.apify.com/account/integrations.

## Servers

| Server | Tools | What it covers |
|---|---|---|
| `india-jobs-mcp` | 14 | India job market data: Naukri, Indeed India, Foundit, Shine, Apna, CutShort, Hirist, Instahyre and Internshala, plus LinkedIn candidate sourcing and AmbitionBox employer snapshots. |
| `company-diligence-mcp` | 13 | Company diligence from official sources: SEC EDGAR, GLEIF LEI, EU VIES VAT, US state registries, UK Companies House, CourtListener, USAspending, SAM.gov and FEC, plus Trustpilot and news. |
| `recruiting-jobs-mcp` | 10 | Job and candidate data for recruiting: ATS postings (Greenhouse, Lever, Workday, Ashby), LinkedIn, Indeed, SimplyHired, Naukri and CutShort, plus candidate sourcing and employer snapshots. |
| `social-research-mcp` | 8 | Social listening: Reddit, X, Threads, LinkedIn posts, YouTube transcripts, Google News and Google Trends. |
| `ecommerce-intel-mcp` | 8 | Product research: Amazon products and reviews, AliExpress prices, Shopify catalogs, TikTok Shop, Meta Ad Library and Google Trends. |
| `real-estate-mcp` | 8 | US property data: Zillow listings, sales, rentals and property details, plus Redfin, Realtor.com and Airbnb rental supply. |
| `lead-generation-mcp` | 8 | B2B and local leads: people with work emails, email verification, website contacts, Google Maps, Yellow Pages and Trustpilot. |
| `academic-research-mcp` | 6 | Scholarly search: OpenAlex, Crossref, arXiv, OpenCitations and PubMed. |
| `india-real-estate-mcp` | 5 | India property listings: 99acres, MagicBricks, NoBroker and Housing.com. Rent and sale, residential and commercial. |

Store pages, with tool prices: `https://apify.com/themineworks/<server>`.
Full tool lists: https://github.com/themineworks/mcp-servers

## Using one server elsewhere

Every server also works through Apify's MCP gateway, which signs you in
with your Apify account instead of a token:

```
https://mcp.apify.com/?tools=themineworks/india-jobs-mcp
```

## Licence

MIT for this repository. The servers themselves run on Apify and are not
included here.
