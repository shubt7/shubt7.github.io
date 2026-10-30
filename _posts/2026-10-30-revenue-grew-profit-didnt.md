---
layout: post
title: "Revenue Grew Every Year. Profit Didn't Keep Up."
date: 2026-10-30
---

Most of my week in analytics goes to one question: is the number on the slide telling the whole story? A revenue chart that climbs every quarter is easy to celebrate. It's also the chart that gets the least scrutiny, because it looks like good news.

So I built a small sales KPI dashboard on a synthetic dataset of 6,000 orders from 2023 to 2025, to practise the workflow I use at work: start with the stakeholder question, define the KPI, prepare the data, calculate it, then check whether the chart answers the question. This post is about what the dashboard showed when I looked past the headline.

## The headline hides the margin

Revenue grew from $4.83M in 2023 to $6.13M in 2025, with 15.9% growth in 2024 and 9.4% in 2025. Profit margin moved the other way, down from 72.6% to 71.8% to 71.2%. Sales were rising, but each dollar kept slightly less profit.

A drop of under two points looks like noise on a slide. Over a few years of compounding growth, it's real money. In analytics, I'd treat "revenue is up" as the start of a question, not the answer. The next question is what it cost to get there.

## Revenue and profit can point in different directions

The clearest finding came from breaking revenue down by product:

| Product | Share of revenue | Share of profit (calculated) | Profit margin |
|---|---|---|---|
| Software Licence | 55.5% | ~60% | 78.2% |
| Hardware Device | 17.6% | ~13% | 51.9% |
| Support Plan | 7.8% | ~9% | 85.1% |
| Consulting Hour | 7.5% | ~6% | 60.0% |
| Training Course | 11.5% | ~11% | 70.0% |

Hardware is almost a fifth of revenue but roughly an eighth of profit. If a team is measured on revenue alone, hardware looks like a strong contributor. Measured on profit, it's the weakest line here. A revenue-only report would hide that completely.

This is the kind of gap I look for when I set up a dashboard. A bar chart of revenue by product is standard. Placing profit margin next to each product's share of revenue and profit makes the trade-off visible.

## Volume and value are different views

Northeast is the largest region at 27.9% of revenue, and Online is the largest channel at 45.2%. Margin hardly changes across either split. Region and channel show where the volume is, not where the value is. When I build reports for a commercial team, I keep those two views separate so one doesn't get mistaken for the other.

## The discount question

The obvious follow-up is whether deeper discounts erode margin. In this dataset, they don't. Margin stays between 71.4% and 72.0% in every band, from 0–5% up to 20–30%.

I wouldn't trust that result without checking it. The data is synthetic, so it reflects how I generated it, not how a real sales floor behaves. In a live business I'd expect margin to fall as discounts deepen, and I'd test that against actual transactions before drawing conclusions. The value of the dashboard is in asking the question clearly. Answering it takes real data.

## What I'd put on the dashboard

If I were rebuilding this for a real stakeholder group, I'd make three changes:

1. **Show profit beside revenue on every chart.** Revenue alone rewards volume at any price.
2. **Break down margin by product and discount band.** That's where the real differences show up.
3. **Add a margin trend line.** It's one number, and it's the one that moved quietly.

## The takeaway

Revenue is the easy number to report, and profit is the one that shows whether the growth was worth it. In analytics, the work is making sure both appear on the same screen, so the hard question gets asked before the meeting ends.
