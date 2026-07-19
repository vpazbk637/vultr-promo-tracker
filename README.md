# How to Use Vultr Promo Code: A Step-by-Step Walkthrough to Redeem $300/$250/$200 Free Credit, the VULTRMATCH Deposit Bonus, Hidden Expiry Rules & Best Plans to Spend Credit On

Last Tuesday a friend texted me at 11 p.m.: "I just signed up at Vultr, pasted `FLY300VULTR` into the box, hit Apply, and nothing showed up in my balance." The code was fine. He'd skipped the step where you link a card first, so the eligibility check silently rejected it. That small mess is what this walkthrough is built to prevent.

A **Vultr promo code** is a short alphanumeric string — think `FLY300VULTR`, `250VULTRFLY`, `FLYTWOHUNDRED`, or `VULTRMATCH` — that, when applied through the **Billing → Gift Code** section of the Vultr Console, drops promotional credit into a brand-new account in exchange for meeting a few eligibility checks: a linked credit card or PayPal, and for some codes an initial deposit. The credit is real and spendable on Cloud Compute and Optimized Cloud Compute products, but it carries a 30-day expiry on the free-credit codes and a 12-month expiry on the VULTRMATCH match bonus, per Vultr's own match page FAQ.

So if you arrived here searching "how to use vultr promo code," the short version is: register, link a real payment method, open Billing, paste the code into Gift Code, watch the credit land — then deploy something within 30 days before it evaporates. The rest of this guide fills in every pothole I hit on the way.

## The 4 Vultr Promo Codes You Can Actually Use Right Now

Pull up the official [coupons page](https://www.vultr.com/coupons/?ref=9738262-9J) and you'll see a wall of nearly identical-looking offers. They are not identical. The match deal behaves nothing like the free-credit deals, and picking the wrong one is the most common mistake I see in the r/Vultr threads.

| Promo Code | What You Get | Expiry | Eligibility | Best For |
|---|---|---|---|---|
| `FLY300VULTR` | $300 free credit | 30 days from activation | New accounts only, valid card or PayPal linked | Big benchmark run, AI inference test, multi-region demo |
| `250VULTRFLY` | $250 free credit | 30 days from activation | New accounts only | Mid-size web app trial, staging environment |
| `FLYTWOHUNDRED` | $200 free credit | 30 days from activation | New accounts only | Single-server POC, blog migration test |
| `VULTRMATCH` | Vultr matches your first deposit 1:1, up to $100 extra | 12 months from issuance | New accounts only, requires an actual deposit | Anyone who plans to keep using Vultr past a month |

> 👉 [Claim the active Vultr promo codes on the official coupons page](https://www.vultr.com/coupons/?ref=9738262-9J)

The free-credit codes are trial fuel — burn bright, burn fast. The match code is the only one that behaves like a real long-term discount, because the matched $100 lasts a full year and gets applied 50/50 against your real funds on every hourly accrual (Vultr's own match page spells out the 50/50 split). If you're going to keep paying Vultr after the trial, `VULTRMATCH` is mathematically the better deal even though the headline number is smaller.

## How to Apply a Vultr Promo Code: Numbered Steps, Start to Finish

The official Vultr docs page titled "How Can I Add a Promotional Code?" confirms the eligibility rules: a valid Credit Card or PayPal linked, one code per user, promotional credits are non-transferable. Here is the exact sequence that has worked every time I tested it.

1. **Register a fresh account** through the [Vultr signup page](https://www.vultr.com/?ref=9738262-9J) using an email you have never used on Vultr before — duplicate accounts are explicitly disqualified from promotions.
2. **Verify your email** and complete any phone verification prompt; do not skip these, the Gift Code box stays greyed out until identity checks pass.
3. **Link a real Credit Card or PayPal** under Billing → Payment Methods. A prepaid card or a virtual card with $0 balance will fail the $5–$10 authorization hold that Vultr runs to confirm the method is live.
4. **Open Billing → Gift Code** in the left-hand navigation of the Vultr Console — not the "Make a payment" flow, which is for topping up real funds.
5. **Paste the code** exactly as written (they are case-insensitive but spaces will break them) and click **Apply**.
6. **Watch the credit appear** under Billing → Overview as a separate "Promotional Balance" line, distinct from your real funds. Note the expiry date stamped next to it.
7. **Deploy something within 30 days** (for the FLY codes) or within 12 months (for VULTRMATCH). Unused promotional credit disappears silently on the expiry date — there is no warning email.

If step 5 throws a "code invalid" error and you're certain the code is current, the cause is almost always one of three things: no payment method linked, an account flagged for the standard 24-hour Trust & Safety review on new signups, or a code that has already been used on a different account under the same identity. Open a support ticket referencing the code and the ticket queue moves faster than the live chat for billing-specific issues.

> 👉 [Start the signup flow and grab your promo code in one go](https://www.vultr.com/?ref=9738262-9J)

## The Hidden Conditions Nobody Puts on the Coupon Page

Here is the part most "Vultr promo code 2026" articles glide over, and it's the part that actually costs people money.

A Reddit user on r/Vultr (post "What are the hidden conditions for the Vultr coupon codes?", January 2026) tested the $300 promo and reported that the credit added on April 16 expired on May 17 — roughly 30 days, not a year. The top reply in the same thread states plainly: "They last 30 days unless it states longer. I don't think it matters which you pick. Go with the highest." That matches Vultr's own match-page FAQ, which reserves the 12-month window exclusively for the VULTRMATCH deposit bonus.

Then there's the deposit escalation issue. Several Trustpilot reviews from mid-2026 describe the same pattern: sign up, deposit $10 to unlock the $250 credit, then hit a "Monthly Fee Limit Reached" or "additional verification required" wall when trying to deploy anything bigger than a $5/month node. One reviewer trying to rent a `vbm-8c-64gb-amd` bare-metal box was told to spend $250 on other services over 30 days before being allowed to rent the hardware they came for. GPU access is even more locked down — a user who deposited $1,000 to rent GPUs was told to wait 60 days, with spending capped to a few small compute nodes in the meantime.

Vultr's official response on Trustpilot confirms the policy without denying the experience: "Access to certain high-demand resources, including GPUs, may be subject to account reviews, spending limits, or eligibility requirements designed to protect the platform." So the headline "$300 free credit" is real, but it's a credit you can only spend on the lower-tier SKUs until your account ages and passes review.

**Plain-language summary:** The free-credit codes are 30-day trial fuel for Cloud Compute and Optimized Cloud Compute, not a year of free hosting. The VULTRMATCH deposit bonus is the only long-tail discount, and it requires you to actually spend real money first.

## Where to Spend the Credit: Vultr's Full Plan Lineup

Vultr organizes compute into four buckets: Cloud Compute (shared vCPU, the cheap tier), Optimized Cloud Compute (dedicated vCPU, the serious tier), Cloud GPU (accelerated), and a handful of bare-metal and storage specialized SKUs. Promotional credit applies to "select products" — in practice the Cloud Compute and Optimized Cloud Compute lines work without issue; bare metal and most GPU SKUs sit behind the spending-limit gate described above.

Below is the full plan list pulled from the [official pricing page](https://www.vultr.com/pricing/?ref=9738262-9J), with monthly and hourly rates. Use the buy link to jump straight to the relevant product page (affiliate-tagged).

### Cloud Compute — Regular Performance

| Plan | vCPU | RAM | Storage | Bandwidth | Monthly | Hourly | Buy |
|---|---|---|---|---|---|---|---|
| IPv6 Only | 1 | 0.5 GB | 10 GB | 0.50 TB | $2.50 | $0.004 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| Starter | 1 | 0.5 GB | 10 GB | 0.50 TB | $3.50 | $0.005 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 1 vCPU | 1 | 1 GB | 25 GB | 1.00 TB | $5 | $0.007 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 1 vCPU | 1 | 2 GB | 55 GB | 2.00 TB | $10 | $0.015 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 2 vCPU | 2 | 2 GB | 65 GB | 3.00 TB | $15 | $0.022 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 2 vCPU | 2 | 4 GB | 80 GB | 3.00 TB | $20 | $0.030 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 4 vCPU | 4 | 8 GB | 160 GB | 4.00 TB | $40 | $0.060 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 6 vCPU | 6 | 16 GB | 320 GB | 5.00 TB | $80 | $0.119 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 8 vCPU | 8 | 32 GB | 640 GB | 6.00 TB | $160 | $0.238 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 16 vCPU | 16 | 64 GB | 1280 GB | 10.00 TB | $320 | $0.476 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 24 vCPU | 24 | 96 GB | 1600 GB | 15.00 TB | $640 | $0.952 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |

### Cloud Compute — High Performance (AMD EPYC / Intel Xeon, NVMe)

| Plan | vCPU | RAM | Storage | Bandwidth | Monthly | Hourly | Buy |
|---|---|---|---|---|---|---|---|
| 1 vCPU | 1 | 1 GB | 25 GB | 2.00 TB | $6 | $0.009 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 1 vCPU | 1 | 2 GB | 50 GB | 3.00 TB | $12 | $0.018 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 2 vCPU | 2 | 2 GB | 60 GB | 4.00 TB | $18 | $0.027 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 2 vCPU | 2 | 4 GB | 100 GB | 5.00 TB | $24 | $0.036 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 4 vCPU | 4 | 8 GB | 180 GB | 6.00 TB | $48 | $0.071 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 4 vCPU | 4 | 12 GB | 260 GB | 7.00 TB | $72 | $0.107 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 8 vCPU | 8 | 16 GB | 350 GB | 8.00 TB | $96 | $0.143 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |
| 12 vCPU | 12 | 24 GB | 500 GB | 12.00 TB | $144 | $0.214 |  [Choose this plan](https://www.vultr.com/products/cloud-compute/?ref=9738262-9J) |

### Cloud Compute — High Frequency (3 GHz+ Intel Xeon, NVMe)

| Plan | vCPU | RAM | Storage | Bandwidth | Monthly | Hourly | Buy |
|---|---|---|---|---|---|---|---|
| 1 vCPU | 1 | 1 GB | 32 GB | 1.00 TB | $6 | $0.009 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 1 vCPU | 1 | 2 GB | 64 GB | 2.00 TB | $12 | $0.018 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 2 vCPU | 2 | 2 GB | 80 GB | 3.00 TB | $18 | $0.027 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 2 vCPU | 2 | 4 GB | 128 GB | 3.00 TB | $24 | $0.036 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 3 vCPU | 3 | 8 GB | 256 GB | 4.00 TB | $48 | $0.071 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 4 vCPU | 4 | 16 GB | 384 GB | 5.00 TB | $96 | $0.143 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 6 vCPU | 6 | 24 GB | 448 GB | 6.00 TB | $144 | $0.214 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 8 vCPU | 8 | 32 GB | 512 GB | 7.00 TB | $192 | $0.286 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 12 vCPU | 12 | 48 GB | 768 GB | 8.00 TB | $256 | $0.381 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |

### Optimized Cloud Compute — General Purpose (Dedicated AMD EPYC vCPU)

| Plan | vCPU | RAM | Storage | Bandwidth | Monthly | Hourly | Buy |
|---|---|---|---|---|---|---|---|
| 1 vCPU | 1 | 4 GB | 30 GB | 4.00 TB | $30 | $0.045 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 2 vCPU | 2 | 8 GB | 50 GB | 5.00 TB | $60 | $0.089 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 4 vCPU | 4 | 16 GB | 80 GB | 6.00 TB | $120 | $0.179 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 8 vCPU | 8 | 32 GB | 160 GB | 7.00 TB | $240 | $0.357 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 16 vCPU | 16 | 64 GB | 320 GB | 8.00 TB | $480 | $0.714 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 24 vCPU | 24 | 96 GB | 480 GB | 9.00 TB | $720 | $1.071 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 32 vCPU | 32 | 128 GB | 640 GB | 9.00 TB | $960 | $1.429 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 40 vCPU | 40 | 160 GB | 768 GB | 10.00 TB | $1,200 | $1.786 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 64 vCPU | 64 | 192 GB | 960 GB | 11.00 TB | $1,920 | $2.857 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 96 vCPU | 96 | 256 GB | 1280 GB | 12.00 TB | $3,840 | $5.714 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |

### Optimized Cloud Compute — CPU Optimized

| Plan | vCPU | RAM | Storage | Bandwidth | Monthly | Hourly | Buy |
|---|---|---|---|---|---|---|---|
| 1 vCPU | 1 | 2 GB | 25 GB | 4.00 TB | $28 | $0.042 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 2 vCPU | 2 | 4 GB | 50 GB | 5.00 TB | $40 | $0.060 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 2 vCPU | 2 | 4 GB | 75 GB | 5.00 TB | $45 | $0.067 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 4 vCPU | 4 | 8 GB | 75 GB | 6.00 TB | $80 | $0.119 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 4 vCPU | 4 | 8 GB | 150 GB | 6.00 TB | $90 | $0.134 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 8 vCPU | 8 | 16 GB | 150 GB | 7.00 TB | $160 | $0.238 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 8 vCPU | 8 | 16 GB | 300 GB | 7.00 TB | $180 | $0.268 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 16 vCPU | 16 | 32 GB | 300 GB | 8.00 TB | $320 | $0.476 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 16 vCPU | 16 | 32 GB | 500 GB | 8.00 TB | $360 | $0.536 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 32 vCPU | 32 | 64 GB | 500 GB | 9.00 TB | $640 | $0.952 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 32 vCPU | 32 | 64 GB | 1000 GB | 10.00 TB | $720 | $1.071 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |

### Optimized Cloud Compute — Memory Optimized

| Plan | vCPU | RAM | Storage | Bandwidth | Monthly | Hourly | Buy |
|---|---|---|---|---|---|---|---|
| 1 vCPU | 1 | 8 GB | 50 GB | 5.00 TB | $40 | $0.060 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 2 vCPU | 2 | 16 GB | 100 GB | 6.00 TB | $80 | $0.119 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 2 vCPU | 2 | 16 GB | 200 GB | 6.00 TB | $100 | $0.149 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 2 vCPU | 2 | 16 GB | 400 GB | 6.00 TB | $125 | $0.186 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 4 vCPU | 4 | 32 GB | 200 GB | 8.00 TB | $160 | $0.238 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 4 vCPU | 4 | 32 GB | 400 GB | 8.00 TB | $195 | $0.290 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 4 vCPU | 4 | 32 GB | 800 GB | 8.00 TB | $250 | $0.372 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 8 vCPU | 8 | 64 GB | 400 GB | 9.00 TB | $320 | $0.476 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 8 vCPU | 8 | 64 GB | 800 GB | 9.00 TB | $390 | $0.580 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 8 vCPU | 8 | 64 GB | 1600 GB | 9.00 TB | $500 | $0.744 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 16 vCPU | 16 | 128 GB | 800 GB | 10.00 TB | $640 | $0.952 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 16 vCPU | 16 | 128 GB | 1600 GB | 10.00 TB | $785 | $1.168 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 16 vCPU | 16 | 128 GB | 3200 GB | 10.00 TB | $1,000 | $1.488 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 24 vCPU | 24 | 192 GB | 1200 GB | 11.00 TB | $960 | $1.429 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 24 vCPU | 24 | 192 GB | 2400 GB | 11.00 TB | $1,175 | $1.749 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 24 vCPU | 24 | 192 GB | 4800 GB | 11.00 TB | $1,500 | $2.232 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 32 vCPU | 32 | 256 GB | 1600 GB | 12.00 TB | $1,280 | $1.905 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 32 vCPU | 32 | 256 GB | 3200 GB | 12.00 TB | $1,565 | $2.329 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |

### Optimized Cloud Compute — Storage Optimized

| Plan | vCPU | RAM | Storage | Bandwidth | Monthly | Hourly | Buy |
|---|---|---|---|---|---|---|---|
| 1 vCPU | 1 | 8 GB | 150 GB | 4.00 TB | $75 | $0.112 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 2 vCPU | 2 | 16 GB | 320 GB | 6.00 TB | $125 | $0.186 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 2 vCPU | 2 | 16 GB | 480 GB | 6.00 TB | $155 | $0.231 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 4 vCPU | 4 | 32 GB | 640 GB | 7.00 TB | $250 | $0.372 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 4 vCPU | 4 | 32 GB | 960 GB | 7.00 TB | $310 | $0.461 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 8 vCPU | 8 | 64 GB | 1280 GB | 8.00 TB | $500 | $0.744 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 8 vCPU | 8 | 64 GB | 1920 GB | 8.00 TB | $620 | $0.923 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 16 vCPU | 16 | 128 GB | 2560 GB | 9.00 TB | $1,000 | $1.488 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 16 vCPU | 16 | 128 GB | 3840 GB | 9.00 TB | $1,240 | $1.845 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 24 vCPU | 24 | 192 GB | 3840 GB | 10.00 TB | $1,500 | $2.232 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 24 vCPU | 24 | 192 GB | 5760 GB | 10.00 TB | $1,850 | $2.753 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| 32 vCPU | 32 | 256 GB | 5760 GB | 12.00 TB | $2,000 | $2.976 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |

### Cloud GPU (Generally Gated Behind Account Review)

| GPU Model | GPUs | GPU RAM | vCPUs | RAM | Storage | Monthly | Hourly | Buy |
|---|---|---|---|---|---|---|---|---|
| NVIDIA GH200 (36-mo reserved) | 1 | 96 GB | 72 | 480 GB | 4800 GB | $2,913 | $4.335 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |
| NVIDIA H100 (36-mo reserved) | 8 | 640 GB | 224 | 2048 GB | 32640 GB | $13,432 | $19.988 |  [Choose this plan](https://www.vultr.com/pricing/?ref=9738262-9J) |

For a $300 promo balance, the sweet spot is the High Performance AMD line at $6/mo or High Frequency at $6/mo — both let you run roughly 50 instance-months of testing within the 30-day window if you stack a few small nodes, or one beefy 8 vCPU / 16 GB node flat-out for the entire month. The Optimized Cloud Compute General Purpose at $30/mo is the next step up if you want dedicated vCPU for a database benchmark.

> 👉 [Compare every Vultr plan on the official pricing page](https://www.vultr.com/pricing/?ref=9738262-9J)

## Is Vultr Actually Any Good? What Real Users Say

Here is where most affiliate articles slap a five-star badge and call it a day. The real picture is messier.

On the positive side, a July 2026 Trustpilot review praised Vultr as "actually better than most big providers like GCP, AWS, Azure — prices are competitive and support is really good, they have never let me down," specifically calling out that BGP is included free. Another reviewer in June 2026 highlighted "outstanding technical support… professional, fast, and remarkably flexible," crediting a billing and snapshot issue resolved quickly. Gartner Peer Insights lists Vultr at a 4.0/5 rating with the summary "Affordable performance stands out, though advanced features feel limited."

On the negative side, the same Trustpilot feed is heavy with billing and account-lock complaints. A May 2026 review describes the $300 credit being pulled mid-trial and the service suspended without access to data. Multiple reviews from April–June 2026 describe the same deposit-escalation pattern around bare metal and GPU access, with one user reporting "they told me I need to deposit, so I deposited $1000. Then they told me I still can't rent GPUs and I need to wait 60 days." Vultr's official responses on Trustpilot do not deny the policy — they restate it as fraud-prevention.

The pattern: small Cloud Compute workloads run reliably and the promo credit flows through cleanly. The friction shows up when you try to spend promotional credit on GPU or bare-metal SKUs, or when a new account gets flagged for KYC review. Treat the $300 as trial fuel for ordinary VMs and the experience is generally smooth.

> 👉 [Read the full Trustpilot feed before you sign up](https://www.trustpilot.com/review/vultr.com)

## Common Failure Modes (and the Fix)

**Code says "invalid" on apply.** You almost certainly haven't linked a real card or PayPal yet, or the account is still in the 24-hour Trust & Safety review window. Link a card, wait, retry.

**Credit appeared but the deploy button is greyed out.** Your account hit the "Monthly Fee Limit Reached" wall that gates high-tier SKUs on new accounts. Drop down to a Cloud Compute Regular Performance or High Performance plan and the deploy goes through. Bigger SKUs unlock as the account ages and accrues real spend.

**Promotional credit vanished before you used it.** The 30-day clock starts the moment the code is applied, not the moment you first deploy. If you're not ready to spin something up, do not redeem the code yet.

**Account suspended mid-trial for KYC.** This one has no clean workaround — Vultr's Trust & Safety team can lock a new account for verification with little warning, and reviewers report 8+ hour waits with only generic copy-paste replies. Keep critical data backed up off-Vultr from day one, even during a trial.

**Charges keep accruing after you stopped using it.** Vultr bills for any resource that is *deployed*, not just running — a stopped instance still costs storage and IP charges. Delete the instance entirely, snapshot it first if you want to keep the data.

## FAQ: How to Use Vultr Promo Code

**Q: Where do I enter the Vultr promo code?**
A: In the Vultr Console, go to Billing → Gift Code (not "Make a payment"), paste the code, and click Apply. You need a linked Credit Card or PayPal first, otherwise the apply button rejects the code silently.

**Q: Which Vultr promo code gives the most free credit?**
A: `FLY300VULTR` gives $300, the largest single free-credit offer on the official coupons page. `250VULTRFLY` gives $250 and `FLYTWOHUNDRED` gives $200. All three expire 30 days after activation.

**Q: Does the Vultr $300 free credit expire?**
A: Yes — 30 days from the moment the code is applied, per multiple Reddit user reports and Vultr's match-page FAQ. Only the VULTRMATCH deposit-match credit lasts 12 months.

**Q: Can existing Vultr customers use a promo code?**
A: No. Vultr's match page states explicitly that "the match promotion is available to anyone new to the Vultr cloud. Existing customers are not eligible," and the same restriction applies to the FLY free-credit codes. Duplicate accounts are also disqualified.

**Q: Do I need to deposit money to use the free credit?**
A: Not for the FLY codes — a linked card or PayPal is enough. For VULTRMATCH you must make an actual deposit, which Vultr matches 1:1 up to $100, applied on a 50/50 basis against your real funds on every hourly charge.

**Q: Can I use the $300 credit on GPU instances?**
A: In practice, no — at least not on a fresh account. Multiple Trustpilot reviews from 2026 report that GPU and bare-metal access is gated behind account-age and additional-deposit requirements, even when the promotional balance shows as available. Cloud Compute and Optimized Cloud Compute work without issue.

## The Short Version

A Vultr promo code is redeemed through Billing → Gift Code after a real card or PayPal is linked, drops $200–$300 of trial credit (30-day expiry) or a $100 deposit match (12-month expiry) into a new account, and is best spent on Cloud Compute or Optimized Cloud Compute plans starting at $2.50/mo. The credit is real but the marketing headlines skip three things: the 30-day clock, the spending-limit wall on GPU/bare-metal, and the KYC suspension risk on new accounts. Treat the promo as a one-month test drive of the lower-tier SKUs, keep backups off-Vultr, and you'll get the full value out of it.

> 👉 [Head to Vultr now, link a card, and apply your promo code](https://www.vultr.com/?ref=9738262-9J)
