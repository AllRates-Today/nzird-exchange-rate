# New Zealand Inland Revenue Exchange Rates API — nzird-exchange-rate

[![npm version](https://img.shields.io/npm/v/nzird-exchange-rate.svg)](https://www.npmjs.com/package/nzird-exchange-rate)
[![license](https://img.shields.io/npm/l/nzird-exchange-rate.svg)](https://github.com/AllRates-Today/nzird-exchange-rate/blob/main/LICENSE)
[![zero dependencies](https://img.shields.io/badge/dependencies-0-brightgreen.svg)](https://www.npmjs.com/package/nzird-exchange-rate)
[![TypeScript](https://img.shields.io/badge/TypeScript-types%20included-3178C6.svg)](https://www.typescriptlang.org/)
[![NZD/USD today](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fallratestoday.com%2Fapi%2Fopen%2Fcentral-bank%2Fnzird%3Fsource%3DNZD%26target%3DUSD&query=%24.rate&label=NZD%2FUSD%20official%2C%20New%20Zealand%20Inland%20Revenue&color=0A7E8C&cacheSeconds=3600)](https://allratestoday.com/tax-authority-rates-api/nzird/)
[![rate date](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fallratestoday.com%2Fapi%2Fopen%2Fcentral-bank%2Fnzird%3Fsource%3DNZD%26target%3DUSD&query=%24.rate_date&label=rate%20date&color=555&cacheSeconds=3600)](https://allratestoday.com/tax-authority-rates-api/nzird/)

**Official New Zealand Inland Revenue (New Zealand) monthly exchange rates for Node.js and TypeScript. The published tax authority rates behind tax filings, customs valuations, audits, and compliant invoicing — not market estimates, but the numbers New Zealand Inland Revenue itself prints, every month.**

## 🚀 Why this client?

- 🏛️ **Official rates** — New Zealand Inland Revenue's own table, with the publisher's own `rate_date` on every response
- 📅 **History back to 2020** — point-in-time tables and daily series for any past date
- 🔀 **Official vs derived, always flagged** — computed inverse/cross pairs carry `derived: true`, never mixed with official prints
- ⚡ **Zero dependencies** — pure ESM + CJS over global `fetch`; Node 18+, Bun, Deno, and edge runtimes
- 🔷 **Type-safe** — full TypeScript definitions shipped with the package
- 🧾 **Compliance-grade metadata** — `rate_type`, publication date, and source disclaimer on every response

> **Official rate, not mid-market:** every value here is a number New Zealand Inland Revenue itself published, fixed once printed and carrying the tax authority's own `rate_date` — what filings and audits require. Need the live mid-market rate for pricing or display instead? Use the [mid-market API](https://allratestoday.com/docs/) or [`@allratestoday/sdk`](https://www.npmjs.com/package/@allratestoday/sdk). The two can diverge by several percent.

## 🔑 Get your API key

Get a free API key at [allratestoday.com/register](https://allratestoday.com/register) — no credit card required. Latest rates are on every plan, including free.

## 📈 Latest official table

[![Latest New Zealand Inland Revenue table](https://allratestoday.com/api/open/central-bank/nzird/table.svg)](https://allratestoday.com/tax-authority-rates-api/nzird/)

The image is rendered live from the keyless endpoint, so it follows the tax authority's publications on npm and on GitHub alike without a new release. The same table as text is folded below for search and copy-paste: on GitHub [a daily Action](.github/workflows/daily-table.yml) refreshes it whenever the tax authority publishes a new table; on npm it is as of the package's publish date.

<!-- daily-table:start -->
<details>
<summary>Table as text: published 2026-10-31 by New Zealand Inland Revenue — 51 rates. Updated 2026-11-25.</summary>

| Base | Quote | Type | Rate |
| --- | --- | --- | ---: |
| NZD | AUD | end_of_month | 0.8013 |
| NZD | AUD | mid_month | 0.8061 |
| NZD | AUD | rolling_12m_average | 0.8362 |
| NZD | CAD | end_of_month | 0.7864 |
| NZD | CAD | mid_month | 0.7966 |
| NZD | CAD | rolling_12m_average | 0.8068 |
| NZD | CNY | end_of_month | 3.7498 |
| NZD | CNY | mid_month | 3.7515 |
| NZD | CNY | rolling_12m_average | 3.9846 |
| NZD | EUR | end_of_month | 0.5027 |
| NZD | EUR | mid_month | 0.5007 |
| NZD | EUR | rolling_12m_average | 0.5018 |
| NZD | GBP | end_of_month | 0.4202 |
| NZD | GBP | mid_month | 0.4236 |
| NZD | GBP | rolling_12m_average | 0.4336 |
| NZD | HKD | end_of_month | 4.4151 |
| NZD | HKD | mid_month | 4.3988 |
| NZD | HKD | rolling_12m_average | 4.5492 |
| NZD | IDR | end_of_month | 10204.47 |
| NZD | IDR | mid_month | 10033.85 |
| NZD | IDR | rolling_12m_average | 10068.11 |
| NZD | INR | end_of_month | 53.615 |
| NZD | INR | mid_month | 53.3385 |
| NZD | INR | rolling_12m_average | 54.2366 |
| NZD | JPY | end_of_month | 88.58 |
| NZD | JPY | mid_month | 88.49 |
| NZD | JPY | rolling_12m_average | 91.73 |
| NZD | KRW | end_of_month | 753.6 |
| NZD | KRW | mid_month | 755.4 |
| NZD | KRW | rolling_12m_average | 844.66 |
| NZD | MYR | end_of_month | 2.277 |
| NZD | MYR | mid_month | 2.2887 |
| NZD | MYR | rolling_12m_average | 2.3435 |
| NZD | PHP | end_of_month | 35.8198 |
| NZD | PHP | mid_month | 35.2586 |
| NZD | PHP | rolling_12m_average | 35.1977 |
| NZD | SGD | end_of_month | 0.7197 |
| NZD | SGD | mid_month | 0.7193 |
| NZD | SGD | rolling_12m_average | 0.7451 |
| NZD | THB | end_of_month | 18.9709 |
| NZD | THB | mid_month | 18.8149 |
| NZD | THB | rolling_12m_average | 18.8722 |
| NZD | TWD | end_of_month | 18.3399 |
| NZD | TWD | mid_month | 17.9973 |
| NZD | TWD | rolling_12m_average | 18.4179 |
| NZD | USD | end_of_month | 0.5629 |
| NZD | USD | mid_month | 0.5606 |
| NZD | USD | rolling_12m_average | 0.5815 |
| NZD | VND | end_of_month | 14538.98 |
| NZD | VND | mid_month | 14516.56 |
| NZD | VND | rolling_12m_average | 15241.01 |

</details>

Source: [Official rates published by NZIRD, served by AllRatesToday](https://allratestoday.com/tax-authority-rates-api/nzird/). Rates are as printed by the tax authority; AllRatesToday is not affiliated with it.
<!-- daily-table:end -->

## 📦 Installation

```bash
npm install nzird-exchange-rate
```

```bash
yarn add nzird-exchange-rate
```

```bash
pnpm add nzird-exchange-rate
```

Requires Node 18+ (global `fetch`); also runs on Bun, Deno and edge runtimes. Also published under the org scope as [`@allratestoday/nzird-exchange-rate`](https://www.npmjs.com/package/@allratestoday/nzird-exchange-rate) — same code, same versions.

## 🏁 Quick start

```js
import { getRate } from 'nzird-exchange-rate';

const pair = await getRate('USD', 'NZD', { apiKey: 'art_live_...' });
console.log(pair.rate, pair.rate_date); // the official New Zealand Inland Revenue rate, on the tax authority's own date
```

## 📚 API reference

- [Latest pair rate](#latest-pair-rate) — one pair from the latest official table
- [Full official table](#full-official-table) — everything the tax authority printed, in one call
- [Table for a date](#table-for-a-date) — the official table for an invoice or filing date
- [Daily time series](#daily-time-series) — one pair across a date range

---

### Latest pair rate

Free plan and up. Pairs the tax authority does not print directly are resolved from its table and flagged (see *Official vs derived rates* below).

```js
const pair = await getRate('USD', 'NZD', { apiKey: 'art_live_...' });
```

**Response:**

```javascript
{
  bank: 'nzird',
  name: 'New Zealand Inland Revenue',
  rate_date: '2026-10-31',   // New Zealand Inland Revenue's own publication date
  source: 'USD',
  target: 'NZD',
  rate: 1.77651,
  rate_type: 'end_of_month',
  derived: true,
  method: 'inverse',  // computed from the published NZD/USD print
  disclaimer: 'Official rates as published by the named central bank. On weekends/holidays the most recent published rate_date is returned.'
}
```

### Full official table

Free plan and up. The complete table for the latest publication date.

```js
import { getLatestRates } from 'nzird-exchange-rate';

const table = await getLatestRates({ apiKey: 'art_live_...' });
console.log(table.rate_date, table.rates.length);
```

**Response:**

```javascript
{
  bank: 'nzird',
  name: 'New Zealand Inland Revenue',
  rate_date: '2026-10-31',
  rates: [
    { "base": "NZD", "quote": "USD", "type": "end_of_month", "value": 0.5629 },
    { "base": "NZD", "quote": "USD", "type": "mid_month", "value": 0.5606 },
    { "base": "NZD", "quote": "USD", "type": "rolling_12m_average", "value": 0.5815 },
    // … the rest of the official table (17 currencies vs NZD)
  ],
  disclaimer: '…'
}
```

### Table for a date

Paid plans. The official table for any date since 2020 — weekends and holidays return the most recent published date, flagged via `published_on_requested_date`, which is exactly the in-force rate a filing needs.

```js
import { getRatesForDate } from 'nzird-exchange-rate';

const day = await getRatesForDate('2026-06-30', { apiKey: 'art_live_...' });
// Optionally narrow to one pair:
const one = await getRatesForDate('2026-06-30', { apiKey: 'art_live_...', source: 'USD', target: 'NZD' });
```

**Response:**

```javascript
{
  bank: 'nzird',
  requested_date: '2026-06-30',
  rate_date: '2026-06-30',                // the date actually published
  published_on_requested_date: true,      // false when a weekend/holiday fell back
  rates: [ /* the full table for that date */ ],
  disclaimer: '…'
}
```

### Daily time series

Paid plans. One resolved rate per publication date — ready for charting, revaluation runs, or audit workpapers.

```js
import { getHistory } from 'nzird-exchange-rate';

const series = await getHistory(
  { source: 'USD', target: 'NZD', from: '2026-01-01', to: '2026-10-31' },
  { apiKey: 'art_live_...' }
);
```

**Response:**

```javascript
{
  bank: 'nzird',
  source: 'USD',
  target: 'NZD',
  from: '2026-01-01',
  to: '2026-10-31',
  count: 152,
  rates: [
    // one entry per publication date
    { date: '2026-10-31', rate: 1.77651, rate_type: 'end_of_month', derived: true, method: 'inverse' },
    // …
  ],
  disclaimer: '…'
}
```

Pass `{ symbol: 'USD' }` instead of `source`/`target` to get the raw published rows for one currency (all rate types, no pair resolution).

---

## 🗺️ Currencies covered

New Zealand Inland Revenue currently publishes rates covering **17 currencies** against the NZD (as of the latest table):

🇦🇺 `AUD` · 🇨🇦 `CAD` · 🇨🇳 `CNY` · 🇪🇺 `EUR` · 🇬🇧 `GBP` · 🇭🇰 `HKD` · 🇮🇩 `IDR` · 🇮🇳 `INR` · 🇯🇵 `JPY` · 🇰🇷 `KRW` · 🇲🇾 `MYR` · 🇵🇭 `PHP` · 🇸🇬 `SGD` · 🇹🇭 `THB` · 🇹🇼 `TWD` · 🇺🇸 `USD` · 🇻🇳 `VND`

## 🏛️ Source

Overseas currency rates Inland Revenue gives for converting foreign amounts to New Zealand dollars for income tax and GST, including the foreign investment fund and controlled foreign company rules: a mid-month rate (accepted as the rate for any day of that month), an end-of-month rate (for market values and balances at the start or end of the tax year) and a rolling 12-month average of the mid-month rates (for repeated transactions and FIF income). They come as yearly tables per tax year (April to March), re-issued each month with one more column.

- Publisher's own page: [Overseas currency rates for tax](https://www.ird.govt.nz/managing-my-tax/overseas-currency-conversion-to-nz-dollars) · [www.ird.govt.nz](https://www.ird.govt.nz/)
- Publication: every month; the exact schedule, freshness status and any current delay are on the [New Zealand Inland Revenue rates page](https://allratestoday.com/tax-authority-rates-api/nzird/)
- Values are stored unmodified, with the publisher's own `rate_date` on every row — see the [methodology](https://allratestoday.com/official-rates-methodology/)

## 🧭 Reading the numbers

- `value` is always **quote currency per 1 unit of base currency** (`base: "EUR", quote: "USD", value: 1.15` means 1 EUR = 1.15 USD).
- New Zealand Inland Revenue quotes **foreign currency per 1 NZD** (e.g. `base: "NZD", quote: "USD"` means USD per one NZD).
- Need the other way round? Ask `getRate(target, source)` and the API inverts or crosses for you, flagged `derived: true` — never divide a published rate yourself in a compliance workflow.
- `rate_type` tells you which of the tax authority's series a row belongs to (`end_of_month` here); some publishers print buy/sell or several fixings for the same pair.

## 🧩 ERP & accounting systems

Loading the official New Zealand Inland Revenue rate into an accounting system is a supported workflow, not a hack. Step-by-step guides with the direction each system expects:

- [Dynamics 365 Business Central](https://allratestoday.com/docs/integrations/business-central/) — built-in Currency Exchange Rate Service, no code
- [Xero](https://allratestoday.com/docs/integrations/xero/) · [QuickBooks Online](https://allratestoday.com/docs/integrations/quickbooks/) · [SAP S/4HANA and ECC](https://allratestoday.com/docs/integrations/sap/) · [Odoo](https://allratestoday.com/docs/integrations/odoo/)

The same keyed endpoints return `?format=csv`, `?format=xml` and `?format=xlsx`, and accept the key as `?api_key=` on the URL for importers that cannot send headers:

```bash
curl "https://allratestoday.com/api/v1/central-bank/nzird/latest?format=xml&api_key=art_live_..."
```

## 🤖 AI agents

- MCP server: `npx -y @allratestoday/central-bank-mcp` (stdio) or the hosted endpoint `https://allratestoday.com/api/mcp` — tools for official rates, history, cross-bank comparison and publication calendars
- Already using the general SDK or MCP server? Since 2026-10-01 [`@allratestoday/sdk`](https://www.npmjs.com/package/@allratestoday/sdk) 1.4+ has `officialRates('nzird')` and [`@allratestoday/mcp-server`](https://www.npmjs.com/package/@allratestoday/mcp-server) 0.6+ has a `get_official_rates` tool — both return this source's latest table with no key, so you can add it without a second dependency
- Claude Code plugin (no key): `/plugin marketplace add AllRates-Today/claude-code-plugin` then `/plugin install allratestoday@allratestoday` — bundles both MCP servers plus an `/official-rate nzird ...` command
- Evaluating? Agents can self-issue a trial key with no signup: `POST https://allratestoday.com/api/agent/keys` (send `Content-Type: application/json`) returns a 100-call key valid 7 days that covers the free-plan methods (latest table, pairs); dated tables and history need a [paid plan](https://allratestoday.com/pricing/). The MCP servers expose it as `request_trial_key`
- Machine-readable site guide: [llms.txt](https://allratestoday.com/llms.txt) · [for-ai-agents](https://allratestoday.com/for-ai-agents/)

## ⚖️ Official vs derived rates

If New Zealand Inland Revenue does not print a pair directly, the API resolves it from the tax authority's own table and says so — official and computed values are never confused:

| `method` | `derived` | Meaning |
| --- | --- | --- |
| `published` | `false` | The tax authority printed this pair directly |
| `inverse` | `true` | Computed as 1 ÷ the published opposite direction |
| `cross` | `true` | Computed via NZD from two published rates |

## 🛡️ Error handling

Errors are thrown as `Error` with `status` (HTTP code) and `body` (the API's JSON error) attached:

```js
try {
  const pair = await getRate('USD', 'XXX', { apiKey: 'art_live_...' });
} catch (err) {
  console.log(err.message); // human-readable reason
  console.log(err.status);  // e.g. 404
}
```

| Status | Meaning |
| ------ | ------- |
| — | Missing `apiKey` (thrown before any request) |
| `400` | Malformed date or parameters |
| `401` | Invalid API key |
| `403` | Endpoint needs a [paid plan](https://allratestoday.com/pricing/) (historical dates & series) |
| `404` | Pair or date range not covered by New Zealand Inland Revenue |
| `429` | Monthly quota exceeded |

## 🔷 TypeScript

Full definitions ship with the package — no `@types` install:

```ts
import type { LatestRates, PairRate, DatedRates, RateEntry, HistoryQuery, RequestOptions } from 'nzird-exchange-rate';
```

## 📦 CommonJS

```javascript
const { getRate } = require('nzird-exchange-rate');

getRate('USD', 'NZD', { apiKey: 'art_live_...' }).then((pair) => console.log(pair.rate));
```

## 💡 Quota tips

- Rates change once a month — cache the official table locally and a small monthly quota goes a long way.
- Every request counts toward your AllRatesToday quota, shared across all AllRatesToday endpoints on your key.

## 📖 Methods reference

| Method | Plan | Description |
| ------ | ---- | ----------- |
| `getRate(source, target, { apiKey })` | Free | Latest rate for one pair, resolved from the official table |
| `getLatestRates({ apiKey })` | Free | The tax authority's full latest official table |
| `getRatesForDate(date, { apiKey, source?, target? })` | Paid | The official table (or one pair) for a YYYY-MM-DD date |
| `getHistory({ symbol \| source+target, from?, to? }, { apiKey })` | Paid | Daily series since 2020 |

## 📥 Bulk data (no key)

Need the whole archive rather than an API call? The same official tables are mirrored daily as open data:

- Hugging Face: [AllRatesToday/central-bank-exchange-rates](https://huggingface.co/datasets/AllRatesToday/central-bank-exchange-rates) — one CSV per institution (`rates/nzird.csv`)
- Kaggle: [allratestoday/central-bank-exchange-rates](https://www.kaggle.com/datasets/allratestoday/central-bank-exchange-rates)
- Raw JSON on GitHub: `https://raw.githubusercontent.com/AllRates-Today/central-bank-exchange-rates/main/data/nzird/latest.json`

## 🔗 Links

- **Website:** [allratestoday.com](https://allratestoday.com)
- [New Zealand Inland Revenue rates page](https://allratestoday.com/tax-authority-rates-api/nzird/) — live table, publication cadence, FAQ
- [All tax authority sources](https://allratestoday.com/tax-authority-rates-api/) · [Full list of 120+ central banks and 50+ tax authorities](https://allratestoday.com/central-bank-rates-api/institutions/) — one API, the same response shape for every source
- [Download central bank rates](https://allratestoday.com/download-central-bank-rates/) — every bank's latest table and history as Excel, CSV or JSON
- [Bank Exchange Rate API](https://allratestoday.com/bank-exchange-rate-api/) — live buy and sell rates from 1,200+ commercial banks in 120+ countries · [npm](https://www.npmjs.com/package/bank-exchange-rates) · [GitHub](https://github.com/AllRates-Today/bank-exchange-rates)
- [Package docs on the site](https://allratestoday.com/docs/sdk/nzird-exchange-rate/) · [ERP integration guides](https://allratestoday.com/docs/integrations/)
- [API documentation](https://allratestoday.com/docs/#central-bank) · [Interactive reference](https://allratestoday.com/api-reference/) · [Methodology](https://allratestoday.com/official-rates-methodology/)
- [Register (Free)](https://allratestoday.com/register) · [Dashboard](https://allratestoday.com/profile) · [Pricing](https://allratestoday.com/pricing/)
- [Status](https://allratestoday.com/status)
- [Postman collection](https://allratestoday.com/postman/)
- [ChatGPT app](https://chatgpt.com/plugins/plugin_asdk_app_6ae1e76098f48191a285ac3f5ab7a83b) — ask ChatGPT for live and official central bank rates
- [OpenAPI reference on Bump.sh](https://bump.sh/allratestoday/doc/allratestoday-api) — also on [SwaggerHub](https://app.swaggerhub.com/apis-docs/allratestoday/allratestoday-exchange-rate-central-bank-rates-api/2.2.0)
- [GitHub](https://github.com/AllRates-Today/nzird-exchange-rate)

## 📜 License

MIT
