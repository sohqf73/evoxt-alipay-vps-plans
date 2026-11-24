# Buy VPS with Alipay: Can You Pay Evoxt Without a Credit Card, What Do the Plans Cost, and Which One Fits? (Fees, Locations, Refunds)

Evoxt accepts Alipay at checkout, so an order can be completed from the Alipay app without an international Visa or Mastercard. The entry plan on the current price list is VM-0.5 at **$2.99/month** for 1 vCPU, 512 MB of RAM, 5 GB of SSD and 500 GB of transfer. Invoices are issued in US dollars and Alipay converts the amount at the rate shown on its confirmation screen before you approve the payment. Provisioning is automatic once the invoice is marked paid.

What follows covers every plan with its specs and price, where the Alipay option sits in the cart, what Evoxt's network does and does not do for mainland China, and the two costs that decide whether a cheap Alipay VPS stays cheap: payment-channel surcharges and what you pay on renewal.

> **Most readers should start with VM-1.** At $5.99/month you get 1 vCPU, 2 GB of RAM, 20 GB of SSD and 1 TB of transfer. That's the cheapest tier where a normal stack (web server plus database plus a couple of background jobs) isn't fighting over memory, and it's enough for a small site, a bot, a build box or a personal proxy. 👉 [Check VM-1 pricing and pick a location](https://bit.ly/EvoXt)

## Every Evoxt plan, side by side

Prices below are the standard-network monthly rates in USD. Some locations are priced as premium network and run higher; the cart shows the exact figure for the location you select before you pay.

| Plan | vCPU · RAM · SSD | Transfer | Price (USD/month) | Order |
| --- | --- | --- | --- | --- |
| VM-0.5 | 1 core · 512 MB · 5 GB | 500 GB | $2.99 | [Order VM-0.5](https://bit.ly/EvoXt) |
| VM-0.75 | 1 core · 1 GB · 10 GB | 750 GB | $4.99 | [Order VM-0.75](https://bit.ly/EvoXt) |
| VM-1 | 1 core · 2 GB · 20 GB | 1 TB | $5.99 | [Order VM-1](https://bit.ly/EvoXt) |
| VM-2 | 2 cores · 4 GB · 30 GB | 2 TB | $11.99 | [Order VM-2](https://bit.ly/EvoXt) |
| VM-3 | 4 cores · 8 GB · 60 GB | 3 TB | $23.99 | [Order VM-3](https://bit.ly/EvoXt) |
| VM-4 | 8 cores · 16 GB · 80 GB | 4 TB | $47.99 | [Order VM-4](https://bit.ly/EvoXt) |
| VM-8 | 16 cores · 32 GB · 100 GB | 5 TB | $95.99 | [Order VM-8](https://bit.ly/EvoXt) |

The jump from VM-0.5 to VM-1 is $3 a month and quadruples the RAM. Below VM-1 you're shopping on price alone; a 512 MB or 1 GB box runs a static site, a small proxy or a monitoring agent, and not much else once a database and a package manager are installed. VM-2 is the first plan where two cores help, which matters if you're compiling code or running anything with a worker process. VM-3 and above are for multiple sites, heavier databases or a handful of containers, and the per-gigabyte cost flattens out as you climb.

## How the Alipay payment actually works

Pick a plan and a location from the order form, then choose Alipay in the payment-method list on the checkout page. The invoice total appears in USD. Confirming in the Alipay app (or scanning the QR code on the payment page) converts that total to CNY at Alipay's cross-border rate, and the CNY figure is displayed before you approve. The invoice is marked paid within seconds of confirmation, the server is created, and the IP address, root password and control-panel login arrive by email.

Two details are worth knowing before you scan.

**Check the invoice total against the plan price.** Some hosts pass the cost of the Alipay channel on to you: Infrawire, for instance, adds 3% to Alipay invoices and shows the fee on the invoice before you confirm, while cards, PayPal and crypto stay fee-free there. If Evoxt's invoice total equals the plan price shown on the price list, no surcharge has been applied; if it's a few percent higher, that's the channel fee and you should decide whether it's worth switching payment method.

**Alipay accounts are real-name verified.** The payment is tied to your verified identity even though the host itself may never ask for ID. That's fine for most buyers, and it's the reason some people pay with crypto instead. If the purchase needs to stay unlinked from your real name, ask support which alternatives they accept before you order rather than after.

One more practical point: the conversion rate you get on day one is not the rate you'll get at renewal. Budget in USD and treat the CNY amount as an estimate.

## Where the servers sit, and what that means from mainland China

Evoxt's order form offers locations across Asia, Europe and North America, including Malaysia, Japan, Australia, the United States, the United Kingdom, Germany, the Netherlands and Poland. The list changes as capacity is added, so confirm the specific city in the cart before paying.

Here's the part most "buy VPS with Alipay" pages skip: **Alipay support says nothing about routing to China.** Evoxt's published plan information does not advertise a China-optimized route such as CN2 GIA or China Unicom VIP. Japan and Malaysia are the shortest hops from most of mainland China, and European or US locations will add distance on top of whatever transit your ISP uses.

If your users are in mainland China and latency decides whether the project works, expect to test rather than assume. Order the smallest plan on a monthly cycle, measure ping and traceroute from the provinces and ISPs you care about, and only then commit to a bigger box or a longer term. Providers that do sell China-optimized lines say so explicitly in their plan names; this one doesn't.

## What the first year actually costs

Monthly billing on VM-1 is $5.99, or $71.88 across twelve months. VM-0.5 comes to $35.88 a year. Evoxt lets you choose the billing cycle in the cart, and any cycle discount is applied there and shown on the invoice before payment, so the annual total is the number to compare rather than the monthly headline multiplied by twelve.

The figure that matters more is the renewal rate. Evoxt's listed prices are recurring rates for the cycle you pick, not a discounted first term that jumps later, which is unusual in this market and worth confirming on your own renewal invoice. Where the cost does move is the exchange rate: a $5.99 renewal is a fixed dollar amount, but the CNY you pay for it in eighteen months is not.

If you're testing whether a location works for you, pay monthly for the first order. The difference between monthly and annual on VM-1 is small enough that flexibility is worth more than the discount in month one.

## Who shouldn't buy Evoxt

**You need a China-optimized line.** No amount of plan comparison fixes transit. rdp.monster states plainly that its European and US datacenters have no CN2 GIA-style routes; Evoxt doesn't market one either. If mainland latency is the whole point of the project, buy from a provider that sells CN2 GIA as a named product and accept the higher price.

**You need a Windows licence included.** Evoxt's plans are Linux-first self-managed VPS. rdp.monster sells Windows RDP from $8.99/month with 2 dedicated cores, 6 GB of DDR4 ECC and 40 GB of NVMe, and its high-performance line on Ryzen 9 7950X starts at $13.99/month. That's a different product at a different price, and the licence question is why.

**You need a specific city Evoxt doesn't cover.** LightNode lists Alipay VPS in more than 40 countries starting at $7.71/month for 2 GB of RAM, 1 vCPU, 50 GB of NVMe and 1 TB of transfer, with hourly billing. Infrawire starts at €8.30/month with an Alipay option and a Hong Kong presence at Equinix HK1, and charges the 3% Alipay fee mentioned earlier.

**You want managed operations.** All of the above are self-managed. Nobody is going to tune your MySQL config or patch your kernel for you.

## FAQ

**Do I need an international credit card to order?**
No. Alipay is offered as a payment method at checkout, and the order completes entirely inside the Alipay app. That's the reason this payment route exists for buyers in mainland China.

**Does Evoxt add a surcharge for Alipay?**
Compare the invoice total with the plan price on the price list. If they match, there's no surcharge; if the invoice is higher by a small percentage, the channel fee has been passed through. Some hosts do this openly, which is why the check is worth thirty seconds.

**How long until the server is ready?**
Provisioning is automatic after the invoice is marked paid, so the wait is measured in minutes rather than hours. Watch for the welcome email with the IP and root password; if it hasn't arrived within a reasonable window, check the client area before opening a ticket.

**Can I change the location after ordering?**
Treat location as a decision made at order time. Changing it normally means deploying a new server in the target location and migrating your data, so if the city matters, confirm it's available in the cart before you pay.

**What's the refund situation?**
Evoxt's terms of service set out the conditions and the window; read them before ordering rather than after something breaks. For a first order, monthly billing keeps your exposure to one month, which is usually cheaper than any refund argument.

## Picking a plan in one line each

A static site, a proxy or a monitoring agent: VM-0.5 at $2.99. A small site with a database, a bot, or a build server: VM-1 at $5.99, and it's the plan most people should buy. Multiple sites or containers with real traffic: VM-2 at $11.99. Anything with heavy concurrent workloads: VM-3 or above, where you're buying cores rather than disk.

Before you pay, confirm two things: the invoice total matches the plan price after Alipay conversion, and the location in your cart is the one you actually tested or intended. 👉 [Start with VM-1 on a monthly cycle and test the location yourself](https://bit.ly/EvoXt)
