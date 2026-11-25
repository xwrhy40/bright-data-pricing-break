# Bright Data Pricing: Is $8/GB, $1.50 per 1,000 Records, or the $499 Monthly Plan the Right Buy? (Full Plan Table and Break-Even Math)

Bright Data charges **$8 per GB** for residential proxy traffic on pay-as-you-go, **$1.50 per 1,000 records or requests** across its scraper APIs, and **$499 a month** for the cheapest commitment plan. A coupon on the residential page halves the gigabyte rate to $4 for the opening months, and then it goes back to $8.

Three billing units, three sets of rules, and one number that settles most purchases: **332,667 records a month** is where the $499 API plan starts beating pay-as-you-go. Below that, you are paying for capacity you won't use.

> **Buying raw proxy bandwidth?** Bright Data is the purchase, and the $8/GB rate plus a KYC check is the entry cost.
> **Scraping 330,000+ records a month from hard targets?** The $499 Scale plan, with $1.30 per 1,000 beyond the included 384,000, is the cheapest flat rate Bright Data sells.
> **Under 300,000 standard pages a month and no proxy needs?** A credit-based API costs a fraction of that. ScraperAPI's Hobby plan is $49 for 100,000 credits. 👉 [See ScraperAPI's plan table with credits, threads and prices](https://www.scraperapi.com/pricing/?fp_ref=coupons)

## Bright Data pricing at a glance: every product on the price list

Bright Data sells four things: proxy bandwidth, scraper APIs, datasets, and a fully managed service. Each has its own unit, so comparing them to each other is meaningless. Here is the whole list, split by type.

### Proxy and network pricing

| Product | Free allowance | Pay as you go | Entry commitment |
| --- | --- | --- | --- |
| Residential proxies | One-time $2 trial credit, 7 days | $8/GB, or $4/GB with coupon | $499 for 71 GB ($7/GB) |
| Datacenter proxies | One-time $2 trial credit | $0.60/GB | $499 for 1 TB listed, or 10 IPs for $14 |
| ISP proxies (static residential) | One-time $2 trial credit | $8/GB | $499 for 71 GB, or 10 shared IPs at $1.80 each |
| Dedicated ISP IPs | None | $3.50 per IP | $2.50 per IP at volume |

Residential bandwidth gets cheaper as the commitment grows: $499 buys 71 GB at $7/GB, $999 buys 166 GB at $6/GB, and $1,999 buys 399 GB at $5/GB. Shared ISP IPs drop from $1.80 each at 10 IPs to $1.30 each at 1,000.

### Scraper API and dataset pricing

| Product | Free allowance | Pay as you go | $499 Scale plan | Overage |
| --- | --- | --- | --- | --- |
| Web Scraper API | 5,000 records/month | $1.50/1,000 records | 384,000 records | $1.30/1,000 |
| Web Unlocker API | 5,000 requests/month | $1.50/1,000 requests | 383,000 requests | $1.30/1,000 |
| SERP API | 5,000 requests/month | $1.50/1,000 requests | 380,000 requests | $1.30/1,000 |
| Browser API | 5,000 credits (1 GB) | $8/GB | 71 GB | Standard GB rate |
| Datasets | Free samples | From $2.50/1,000 records | 100,000 records for $250, one-time | n/a |

The 5,000 monthly credits are shared across Web Unlocker, SERP, Web Scraper, Browser API and Scraper Studio. One credit equals one request or one record. They don't carry over, and they stop once you move onto a pre-commit plan.

### Managed data services

Bright Data will run the collection for you if you don't want to touch an API. A Standard project starts at **$1,000/month** plus a **$500** one-time setup per scraper and **$250/scraper** maintenance from month two, covering one scraper, 250,000 records and 24/7 support. A Strategic annual project starts at **$2,000/month** with 500,000 records, a dedicated Data Concierge and daily project reporting. Both deliver JSON, NDJSON or CSV by webhook or API. Every figure is billed in USD; local currency amounts on the page are estimates only.

## What a Bright Data bill actually looks like

The list price is the starting point, not the invoice. Three worked examples using the published rates:

**1. The $999 plan at 300 GB works out to $3.33/GB.** That tier lists $6/GB for 166 GB, but the 50% coupon doubles the effective allowance for the first months, and 300 GB consumed against a $999 charge is $3.33 per gigabyte. Fill the allowance and the tier rate is real. Use half of it and the effective rate doubles.

**2. The $499 plan with 50 GB used still costs $499.** That's **$9.98/GB**, more than the $8/GB you'd pay with no commitment at all. Fifty gigabytes on pay-as-you-go is $400. The commitment only pays off when you consistently use most of what it includes.

**3. The coupon expires in the fourth month.** At a steady 100 GB/month, half price for three months saves $1,200 in year one and nothing after that. Budget the full $8/GB from month four or your second-year costs will surprise you.

## Five costs the headline rate doesn't include

This is where most budget plans go wrong, because none of it appears on the pricing table.

**KYC before you touch residential or mobile.** Bright Data's FAQ says a representative will ask you to go through a compliance process, known as KYC, which can include a video call. Days of lead time before your first proxy request, not minutes.

**Bandwidth is billed in both directions.** Request headers, request data, response headers and response data all count against your GB. Your real consumption per page is higher than the page size.

**Commitments don't roll over.** The monthly commitment is charged automatically on the 1st, and unused volume does not carry into the next month. A slow January still costs $499.

**Zone spend limits lag by 15 minutes.** You can cap a proxy zone's daily spend, but the limit is recalculated every 15 minutes, so any zone can overshoot by a quarter hour of traffic before the cap bites.

**The account suspends at zero balance.** You get an email at 85%, and at 100% the account stops until you add funds. Auto-recharge is the only way to avoid a pipeline that dies mid-crawl.

One more exclusion that catches people: **proxies are not in the free tier.** The 5,000 monthly credits cover the scraper APIs only. Proxy users get a one-time $2 trial credit valid for seven days, plus $5 when a payment method is added. If you want to test proxy throughput before committing, that is the whole free window. 👉 [See the free plan and trial allowance on ScraperAPI's pricing page](https://www.scraperapi.com/pricing/?fp_ref=coupons)

## The break-even point: when $1.50 per 1,000 records stops being the cheap option

Do the division once and you'll never guess again. $499 ÷ $1.50 × 1,000 = **332,667 records**. Add the 5,000 free monthly credits and the crossover sits at roughly **337,700 records a month**. Above that, the Scale plan's $1.30 overage rate makes it cheaper than paying per record. Below it, pay-as-you-go wins and the commitment loses.

The flat $1.50 is also unusual in one useful way: Bright Data charges the same per 1,000 records whether the target is a plain blog or a Cloudflare-protected retail site, and only successful results are billed. On hard targets, that flat rate is the reason its numbers look good. In Scrape.do's 2026 benchmark across seven difficult targets including Amazon, Indeed, Zillow, Google and X, Bright Data completed 98.87% of requests against Zyte's 91.43%. Over 100,000 requests that gap is 1,130 failures versus 8,570.

## What the alternative costs, translated into the same unit

Credit-based APIs publish a number that isn't comparable to Bright Data's until you convert it. ScraperAPI's Hobby plan is **$49 for 100,000 credits**, which is $0.49 per 1,000 credits. A standard page costs one credit, so a standard page costs $0.49 per 1,000 against Bright Data's $1.50. Startup is $149 for 1,000,000 credits, or $0.149 per 1,000 standard pages.

Then the multipliers arrive, and they change the answer:

| Request type | Credits per request | Hobby ($0.49/1K credits) | Startup ($0.149/1K credits) | Bright Data |
| --- | --- | --- | --- | --- |
| Standard page | 1 | $0.49/1K | $0.15/1K | $1.50/1K |
| Amazon, Walmart, eBay | 5 | $2.45/1K | $0.75/1K | $1.50/1K |
| Google or Bing | 25 | $12.25/1K | $3.73/1K | $1.50/1K |
| JS rendering added | +10 | $5.39/1K | $1.64/1K | $1.50/1K |

Standard pages at any volume: the credit model wins by a wide margin. Google SERP work at low volume: Bright Data's flat $1.50 is roughly a fifth of ScraperAPI's Hobby cost and still beats Startup. Amazon-heavy scraping is close, and the cheaper option flips depending on which tier you're on. Estimate your target mix before you pick a plan, because a headline credit price tells you nothing about a Google request.

### ScraperAPI's plans

| Plan | Included | Geotargeting | Price per month | Start |
| --- | --- | --- | --- | --- |
| Hobby | 100,000 credits, 20 threads | US & EU | $49 | [Open Hobby](https://www.scraperapi.com/pricing/?fp_ref=coupons) |
| Startup | 1,000,000 credits, 50 threads | US & EU | $149, or $134.10 on annual billing | [Open Startup](https://www.scraperapi.com/pricing/?fp_ref=coupons) |
| Business | 3,000,000 credits, 100 threads | Country-level | Between $149 and $1,975 | [Open Business](https://www.scraperapi.com/pricing/?fp_ref=coupons) |
| Scaling | 5,000,000 credits, 200 threads | Country-level | Between $149 and $1,975 | [Open Scaling](https://www.scraperapi.com/pricing/?fp_ref=coupons) |
| Professional | 10,500,000 credits, 300 threads | Country-level | Between $149 and $1,975 | [Open Professional](https://www.scraperapi.com/pricing/?fp_ref=coupons) |
| Advanced | 21,500,000 credits, 500 threads | Country-level | $1,975 | [Open Advanced](https://www.scraperapi.com/pricing/?fp_ref=coupons) |
| Enterprise | 22,000,000+ credits, 500+ threads | Country-level | Custom quote | [Open Enterprise](https://www.scraperapi.com/pricing/?fp_ref=coupons) |

Hobby, Startup and Advanced have published list prices; the three middle tiers sit between Startup and Advanced and the checkout page shows the exact figure for each. Startup billed annually is $1,609.20 a year, a $178.80 saving. The 7-day trial gives 5,000 credits with no card, and a free plan keeps 1,000 credits a month afterwards. Only successful 200 and 404 responses are charged, so failed 500s cost nothing. Pay-as-you-go overflow is available on Scaling and above; auto-upgrade to the next tier is available on Hobby through Professional.

Two limits to weigh before switching. ScraperAPI sells no standalone proxies, so it cannot replace Bright Data's proxy network at any price. And geotargeting below the Business tier is US and EU only. 👉 [Match your monthly request count to a ScraperAPI plan](https://www.scraperapi.com/pricing/?fp_ref=coupons)

## Where Bright Data still wins, and who should not switch

Raw proxy bandwidth has no substitute here. A 400M+ residential IP pool across 195 locations, ISP and datacenter networks, and city/ZIP/ASN targeting is a different product from a scraping API, and ScraperAPI doesn't sell it. If your job needs sticky sessions, your own proxy rotation logic, or Playwright scripts pointed at managed infrastructure, Bright Data is the purchase.

Pre-built datasets and AI tooling are the second reason. Datasets across 100+ domains, a filter API that returned 100 LinkedIn company records in 46.5 seconds in one published test, and an MCP server that plugs into LangChain, CrewAI and LlamaIndex are things a plain scraping API doesn't offer. ISO 27001, GDPR and CCPA compliance matter if procurement asks.

Price-wise, Bright Data is not the cheapest place to buy gigabytes. Evomi lists residential traffic at $0.49/GB on its 100 GB plan and $0.99/GB pay-as-you-go; Scrape.ly's Business plan reaches $2/GB. Bright Data's $5/GB floor on the $1,999 commitment is a premium for network size and success rate, and for large sustained proxy volume that premium is real money.

## FAQ

**How long does the RESIGB50 coupon last?** It takes 50% off residential proxies, which is confirmed. Bright Data's own blog has advertised six months while the current residential pricing page describes three. Treat the number at checkout as final and budget the full $8/GB from the month the discount ends.

**Do the free credits include proxies?** No. The 5,000 monthly credits cover Web Unlocker, SERP, Web Scraper, Browser API and Scraper Studio. Proxies get a one-time $2 trial credit for seven days, plus $5 when you add a payment method.

**Is there a refund or a real trial?** Bright Data offers no permanent free plan. The API side has a genuine free monthly allowance with no card required, and the proxy side has the $2 trial credit. The pricing pages don't publish a refund window, and the monthly commitment is charged on the 1st without rollover, so run your test on the free credits before signing anything.

**Does the plan renew automatically?** Yes. The monthly commitment is charged automatically each month. Pay-as-you-go accounts run on prepaid balance, with a $10 minimum deposit and a first-deposit match up to $500, and the account suspends when the balance hits zero.

## Which one to buy

Match the tool to the unit you actually pay in.

- **Need residential, ISP or datacenter bandwidth** → Bright Data, at $8/GB pay-as-you-go or $499 for 71 GB. Start on the trial credit, expect the KYC step, and don't sign a commitment until you've measured two full months of GB usage.
- **Scraping 330,000+ records a month from protected sites** → Bright Data's $499 Scale plan, where the $1.30 overage rate holds the unit cost down and flat per-record pricing survives a change in target difficulty.
- **Scraping under 300,000 standard pages a month** → ScraperAPI Hobby at $49 or Startup at $149, with no KYC, no monthly minimum above the plan, and free failed requests.
- **Google or Amazon heavy, under 300,000 requests a month** → do the credit multiplication first. Bright Data's flat $1.50 often wins there, and it's worth checking before you assume the cheaper sticker price is the cheaper bill.

Two things to confirm before you enter a card anywhere: whether your monthly volume clears the 332,667-record break-even with room to spare, and whether your targets cost one credit or twenty-five. Get those two numbers right and the plan choice makes itself. 👉 [Start on ScraperAPI's pricing page before you commit to a $499 month](https://www.scraperapi.com/pricing/?fp_ref=coupons)
