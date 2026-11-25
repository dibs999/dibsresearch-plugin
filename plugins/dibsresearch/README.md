# dibsresearch

Three research skills for the dibsresearch connector. They make common questions about listed companies run the same
way every time: which tools to call, in which order, and how the answer looks.

## Skills

- **quarterly-comparison**: one company's KPI or statement line over recent quarters, or several companies on one
  figure (a statement line or a KPI; a ratio where the server serves it), as a table with the fiscal quarter and
  every value a link to its place in dibsresearch.
- **segment-development**: segment revenue and segment margins over time and the shift in the revenue mix, every
  figure a link to its place in dibsresearch.
- **earnings-day-brief**: the newest reported quarter against the quarter before and the same quarter a year earlier,
  and the outlook in the company's own words.

## Use it

Install the plugin, then connect the dibsresearch connector from the plugin's Connectors tab and sign in with a free
dibsresearch account. Ask in plain words, for example "Compare the revenue of NVDA, AMD and AVGO over the last
four quarters" or "How did Microsoft's segments develop?". Claude picks the matching skill.

Each skill also works on its own: upload its folder as a zip under Customize > Skills in Claude, or as a skill in
ChatGPT, next to the dibsresearch connector.

## What the answers contain

Only figures the dibsresearch tools return: KPI values read from the companies' filings and earnings releases, and
statements as filed with the SEC. Every figure is itself a link to its place in dibsresearch: a KPI value opens its
table cell, marked, where the reader shows that same number, else the document. A quarter a company did not report on
its own is shown as not reported, never computed. No share prices, no valuation, no estimates and no investment
advice.

## Data

The skills are instructions only: no scripts, nothing runs on your computer. Claude sends your questions' company
names, tickers, KPI names and periods to the dibsresearch MCP server at https://mcp.dibsresearch.com/mcp, which reads
public company data and nothing from your dibsresearch account.

- Privacy: https://dibsresearch.com/privacy#connected-assistants
- Help: https://dibsresearch.com/connectors, help@dibsresearch.com
- License: for use with dibsresearch only, see LICENSE.txt

## Install in Claude Code

```
/plugin install dibsresearch --marketplace dibs999/dibsresearch-plugin
```
