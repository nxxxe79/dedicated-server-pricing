# Rent dedicated servers: what $55 to $679 a month actually buys, whether a 36-month contract pays off, and when a VPS is the smarter call (with a verified price benchmark)

US hosts advertise dedicated servers from $35.75 a month, but the cheapest configuration with a published spec that I could verify starts around $56. European hosts go lower on paper (€4.99) and much higher at the top (€297 and beyond), and the gap between those numbers is mostly contract length and bandwidth caps, not silicon. SpinServers sits in the middle of the US market at **$79 a month** for a 4-core Xeon E3-1280 v5, 32GB of RAM, a 1TB NVMe drive, 30TB of transfer and dual 10Gbps ports on month-to-month billing.

Below is what each price tier really contains, how the commitment discounts work out in actual dollars, and the five things worth confirming before you pay anyone.

> **Quick pick.** If you need dual 10Gbps ports, 30TB of traffic and no annual contract, the SpinServers E3-1280 v5 at $79/month is the least expensive machine of that shape in this comparison, and it auto-provisions from stock in Dallas or San Jose.
> 👉 [See the current SpinServers configurations and stock](https://bit.ly/Spinservers)

## SpinServers plans: $79 to $679 a month, month to month

SpinServers sells bare metal in Dallas, TX and San Jose, CA with no setup fee and no long-term commitment. Every plan includes root access, IPMI/iKVM console access, a DDoS-protected network, Linux/Windows/ESXi auto-install, free Layer 2 VPC networking between your own servers, and at least one dedicated IPv4 address. In-stock inventory provisions automatically, typically within about half an hour.

| Plan | CPU · RAM · storage | Network | Price & term | Order |
| --- | --- | --- | --- | --- |
| Intel Xeon E3-1280 v5 | 4c/8t @ 3.7GHz · 32GB DDR4 ECC · 1TB M.2 NVMe | 30TB on 10Gbps, dual 10G ports | **$79/mo**, month-to-month | [E3-1280 v5 listing](https://bit.ly/Spinservers) |
| Starter Package | 32GB DDR4 · 1TB NVMe | 10TB on 10Gbps | **$99/mo**, month-to-month | [Starter Package listing](https://bit.ly/Spinservers) |
| Growth Package | 2× Xeon E5-2630L v3 · 256GB DDR4 · 2× 1.6TB SSD (RAID-1) | 20TB on 10Gbps | **$149/mo**, month-to-month | [Growth Package listing](https://bit.ly/Spinservers) |
| High Performance Package | 4× Xeon E5-4640 v2 · 768GB DDR3 · 8× 2TB SSD (RAID-10) | 40TB on 10Gbps | **$679/mo**, month-to-month | [High Performance listing](https://bit.ly/Spinservers) |

Those are the listed rates; SpinServers states that pricing varies by location, hardware and availability, so the cart is the number that counts. The site also lists larger builds without public prices, including a dual Xeon Gold 6148 (40 cores/80 threads, 256GB RAM, 2× 1.92TB SSD, 2× 10Gbps LACP) and a dual Xeon Platinum 8173M (56 cores/112 threads, 512GB RAM, 4× 1.92TB SSD), both in Dallas.

The $99 Starter is worth a second look before you buy it. It doubles the price of the entry server while cutting monthly transfer from 30TB to 10TB. Unless something in that build matters to you specifically, the $79 plan is the better buy.

## The benchmark: what other hosts charge

These are published rates from three other providers, collected to give you a reference range. No plan-level pricing was available for HOSTKEY, only its stated band of roughly €25 at entry, €100 average and €600+ for high-performance builds.

| Provider | Configuration | Bandwidth | Price & commitment |
| --- | --- | --- | --- |
| Dedicated.com | Xeon E3-1270 v5/v6 · 64GB DDR4 · 2× 1TB HDD | 1Gbps | $55.99/mo; $591.25 prepaid for 12 months |
| Dedicated.com | 2× Xeon E5-2640 v4 · 128GB DDR4 · 2× 2TB SSD | 1Gbps, 50TB | $134.99/mo; $1,376.90 prepaid for 12 months |
| Dedicated.com | Xeon Gold 6140 · 36c/72t · 256GB DDR4 · 2× 2TB SSD | 10Gbps, 100TB | $183.99/mo; $1,942.93 prepaid for 12 months |
| Scaleway | Start-2-S-SSD · C2350 2c/2t · 4GB · 120GB SSD | up to 1Gbps | €4.99/mo |
| Scaleway | Start-9-M · Ryzen 5 PRO 3600 6c/12t · 32GB · 2× 1TB NVMe | up to 1Gbps | €33.99/mo with 36-month term |
| Scaleway | Pro-5-S · Xeon E3-1240 v6 · 32GB · 3× 250GB SSD | up to 1Gbps | €37.99/mo with 12-month term |
| Scaleway | Core-10-XS · EPYC 8024P 8c/16t · 64GB · 2× 960GB NVMe | up to 25Gbps | €114.74/mo with 36-month term |
| Scaleway | Core-7-M-A · EPYC 7302P 16c/32t · 256GB · 2× 1.92TB NVMe | up to 25Gbps | €297.49/mo with 36-month term |

Two things stand out. US pricing clusters between roughly $56 and $184 for single and dual Xeon machines with 64GB to 256GB of RAM. European pricing spreads much wider, from €4.99 to €297, and almost every attractive number in the middle carries a 12- or 36-month commitment.

## Do long commitments actually save money?

Dedicated.com discounts prepayment by 3% for three months, 6% for six and 12% for twelve. On the $183.99 Xeon Gold 6140, twelve months at the monthly rate costs $2,207.88; prepaid it's $1,942.93, a saving of **$264.95**. On the $55.99 E3 box, twelve months runs $671.88 monthly versus $591.25 prepaid, a saving of **$80.63**.

So the discount is real, and small. You are handing a host roughly $1,900 up front to save about 12%. If the machine turns out to be wrong for your workload in month three, that money is already gone.

Scaleway's structure is stricter. The €33.99 Ryzen 5 PRO 3600 requires a 36-month term. The €37.99 Pro-5-S requires 12 months. HOSTKEY advertises up to 25% off for terms of six months or more. None of these are bad deals if you know what you need, but each one converts a monthly decision into a multi-year one.

A month-to-month plan costs more per month and buys you the right to leave. SpinServers' entire lineup is billed that way with no setup fee, which makes it a cheap way to find out whether a given CPU and bandwidth profile actually fits before you sign anything longer.

👉 [Check SpinServers' month-to-month rates before committing to a year elsewhere](https://bit.ly/Spinservers)

## What the cheap end of the market leaves out

The €4.99 Scaleway Start-2-S-SSD is a 2-core, 2-thread Avoton C2350 with 4GB of RAM and a single 120GB SSD. It runs a DNS resolver, a small VPN or a backup target. It will not run a database with any traffic on it.

The next rung up has its own traps. Scaleway's Start-1-L at €19.99 gives you 16GB of RAM and 2TB of spinning disk, but caps public bandwidth at 200Mbps. And the Pro-5-S and Pro-5-S-LE cost the same €37.99 with the same Xeon E3-1240 v6 and 32GB of RAM, except the LE version caps you at 300Mbps instead of 1Gbps. Same price, one-third the network.

Port speed is the specification most often used in marketing and least often the thing that limits you. A 10Gbps port with a 10TB monthly allowance gets you further into the month than a 1Gbps port with 30TB. Compare the transfer allowance first, the port speed second.

## Five things to confirm before you pay

**1. Whether the server is actually in stock.** Dedicated.com lists 43 configurations, 37 of them marked in stock, but several of the most attractive ones are annotated "sold out everywhere," and availability concentrates in Los Angeles across its ATL, CHI, DAL, LA, MTL, NYC and SEA locations. Picking a plan by price and discovering it's unavailable is the most common friction in this market.

**2. How long provisioning takes.** Dedicated.com deploys on payment and states the OS install takes about 20 minutes, with credentials emailed automatically. HOSTKEY says preconfigured servers go online minutes after payment. SpinServers auto-provisions in-stock configurations, generally within half an hour. Custom builds at any of these providers take longer.

**3. Whether remote management is included or an add-on.** It should be included. Dedicated.com puts IPMI/iKVM on every server, Scaleway provides hardware IPMI/KVM, HOSTKEY provides IPMI 2.0, iDRAC and iKVM, and SpinServers includes IPMI/iKVM access. Without it, a broken bootloader means a support ticket instead of a five-minute fix.

**4. Whether DDoS filtering costs extra.** Dedicated.com includes it free on every port, Scaleway includes it, HOSTKEY includes basic protection free in Europe. Ask specifically what size of attack is mitigated before scrubbing kicks in.

**5. How many IPv4 addresses you get.** Dedicated.com allocates a /29, which is five usable addresses. SpinServers includes one IPv4 per server, with an IPv6 /64 on listed configurations. If you are hosting multiple sites with separate TLS certificates or running mail, count the addresses before you order.

👉 [View live SpinServers inventory and provisioning status](https://bit.ly/Spinservers)

## Dedicated server or VPS?

A VPS shares physical hardware with other tenants. A dedicated server gives you the whole machine, with no hypervisor layer and no resource throttling from neighbouring workloads. That distinction matters in three situations: heavy databases where disk I/O consistency decides query times, custom virtualization where you need to run your own hypervisor, and production workloads where a noisy neighbour taking CPU steal would show up in your latency graphs.

It does not matter for a low-traffic site, a staging environment or someone learning Linux administration. A €5 to €15 VPS handles those, and paying $79 a month for a bare-metal box to host a brochure site is money spent on nothing.

There is a middle case worth naming. If your VPS bill has grown because you keep adding instances, or you've hit the point where you need custom RAID, custom ISO installs or 10Gbps, that's the signal to move.

## Which one fits your situation

- **Under €40, Europe, light workload:** Scaleway Start-2-S-SSD at €4.99, or the Start-9-M at €33.99 if you need 6 cores, 32GB and NVMe and can accept a 36-month term.
- **US, 10Gbps, no contract, 30TB of traffic:** SpinServers Xeon E3-1280 v5 at $79/month.
- **256GB of RAM and 36 cores in the US:** Dedicated.com's Xeon Gold 6140 at $183.99/month, subject to stock.
- **25Gbps and 256GB in Europe:** Scaleway Core-7-M-A at €297.49 on a 36-month term.
- **Storage-heavy, 144TB of disk:** Scaleway Store-2-L-144TB at €254.99 on a 36-month term.

Before you check out anywhere, confirm three things: that the specific configuration is in stock at the location you want, whether the price quoted is tied to a term you can live with, and what the refund position is. SpinServers bills month to month with no setup fee and no advertised refund window, so treat the first month as the trial and test the disk throughput and network you actually paid for.

👉 [Check current SpinServers availability and pricing](https://bit.ly/Spinservers)
