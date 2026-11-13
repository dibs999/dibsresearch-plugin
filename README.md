# dibsresearch plugin for Claude

Three skills for research on public companies, working with the dibsresearch connector (`https://mcp.dibsresearch.com/mcp`):

- **quarterly-comparison**: one company's KPI or statement line over recent quarters, or several companies on one KPI, as a table with a source link for every figure.
- **segment-development**: segment revenue and margins over time, with the mix shift and where a company changed its segments.
- **earnings-day-brief**: the newest reported quarter against the quarter before and a year earlier, from the company's own release and filings.

Every figure comes from the dibsresearch tools and links to the document it was read from. Only periods the company reported are shown; a quarter it did not report on its own stays "not reported". No share prices, no valuation and no investment advice.

The plugin connects only to the dibsresearch MCP server, which reads public company data and nothing from your dibsresearch account. A free dibsresearch account is needed to connect.

- Connector and help: https://dibsresearch.com/connectors
- Privacy: https://dibsresearch.com/privacy#connected-assistants
- Contact: help@dibsresearch.com

## Install in Claude Code

```
/plugin install dibsresearch --marketplace dibs999/dibsresearch-plugin
```

License: for use with dibsresearch only, see [LICENSE.txt](LICENSE.txt).
