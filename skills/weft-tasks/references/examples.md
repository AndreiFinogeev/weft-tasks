# Worked examples — non-code work

Read this when a request is far from software and the shape of "done" isn't
obvious. Each example shows the request as it arrives, what to ask (or not), and
the card that results.

---

## Investor update

> **User:** I should send an update to investors.

**Ask nothing.** The artifact names itself, the format is known, and a wrong
guess costs one edit. Write it, mark the guesses.

> **Title:** Send October investor update to the 6 angels
>
> **Why:** They last heard from us in July; the next raise starts from their
> warm intros.
>
> **Done when**
> - [ ] Draft under 400 words in the shared drive, named "Investor update — October"
> - [ ] States MRR, month-over-month change, and months of runway, each a number
> - [ ] Contains exactly one ask, addressed to the reader
> - [ ] Sent to all 6 addresses on the angels list; thread link on this task
>
> **Not this time:** Deck refresh, financial model, new investor outreach.
>
> **Assumed:** Monthly cadence, plain email, no attachments.

The trap: "write a good investor update". Length, the three numbers, the single
ask and the send are each checkable by someone who wasn't there. "Good" is not.

---

## Pricing change

> **User:** Our pricing is wrong, fix it.

**Ask** — this is irreversible for existing customers and public.

1. Change prices for new customers only, or existing ones too? *(default: new only)*
2. Is the current tier structure staying, or is that in scope? *(default: staying)*
3. Anything that must not break — annual plans, promised discounts, the free
   tier? *(default: free tier and existing annual plans untouched)*

> **Title:** New pricing live at /pricing, existing customers grandfathered
>
> **Why:** The top tier is under-priced for the support it consumes; new revenue
> per customer has to rise before the next hire.
>
> **Done when**
> - [ ] /pricing shows three tiers, each with a USD number and its stated limit
> - [ ] Checkout completes a test purchase on each tier
> - [ ] Every current customer maps to exactly one tier, listed in the pricing doc
> - [ ] Existing subscriptions still bill the old amount on the next invoice
> - [ ] Effective date and the two rejected structures written in the pricing doc
>
> **Not this time:** Usage-based billing, annual discount changes, a migration email.
>
> **Assumed:** New customers only; tier structure stays.

The trap: "prices are competitive". Competitive against whom, measured when? If
that matters, make it a criterion with names: "each tier is within 20% of
<competitor A> and <competitor B> for the same seat count, table in the doc".

---

## Hiring a contractor

> **User:** I need to find someone to do our SEO.

**Ask** — money leaves the account and the wrong hire costs weeks.

1. Budget ceiling for the first engagement? *(default: $2k for a one-month trial)*
2. What has to improve, in one sentence? *(default: organic signups)*
3. Decide by when? *(default: end of next week)*

> **Title:** Sign an SEO contractor for a one-month paid trial, decide by Friday
>
> **Done when**
> - [ ] 3+ candidates replied with a fixed quote and links to comparable past work,
>       all in the hiring folder
> - [ ] Each candidate scored against the same 4 questions, in one table
> - [ ] One selected; the others told no
> - [ ] Signed SOW in the shared drive with start date, fixed price, and the one
>       metric the trial is judged on
>
> **Constraints:** ≤$2k for the trial, no long-term commitment.
> **Not this time:** Content production, backlink buying, a full audit.

The trap: "find a good contractor". Nothing to look at. The receipt here is the
signed SOW, and the comparison table is what makes the choice reviewable later.

---

## Personal and admin

> **User:** Sort out the business insurance thing.

**Ask nothing** if you know the deadline; otherwise one question.

> **Title:** Business liability insurance active before the 1st
>
> **Done when**
> - [ ] Policy purchased, policy number recorded on this task
> - [ ] Certificate PDF filed in the admin folder
> - [ ] Coverage start date is on or before the 1st
> - [ ] Renewal date in the calendar with a 2-week reminder
>
> **Assumed:** Minimum coverage that satisfies the client contract, cheapest
> provider that meets it.

Admin tasks almost always close on a number someone issued you — policy,
invoice, confirmation, booking reference. Ask for that number, not for a report.

---

## Recurring work

> **User:** I keep forgetting to invoice clients.

Weft tasks do not recur. Make the procedure durable and the cards cheap:

> **Title:** Send invoices — October
>
> **Done when**
> - [ ] Hours pulled from the tracker for each active client
> - [ ] Invoice issued in the billing tool for each, numbers recorded here
> - [ ] All sent; any client with no hours noted as skipped
>
> Repeat monthly: copy this card, change the month.

Create the next three months in one batch call, not one card at a time.

---

## Splitting an oversized ask

> **User:** Launch on Product Hunt next month.

That is a program, not a task. Split by outcome, and stop at about five cards:

1. **Launch assets ready** — thumbnail, gallery, tagline, first comment, all in
   the launch folder.
2. **Landing page handles a traffic spike** — page live, load-tested at N
   concurrent, analytics recording signups.
3. **Hunter and 20 supporters confirmed** — names in a list, each replied yes.
4. **Launch day executed** — posted before 00:05 PT, first comment posted,
   replies answered until 18:00.
5. **Result recorded** — upvotes, signups and top-5 placement written on the card
   the day after.

Not "prepare launch → do launch → follow up". Phases close on opinion; outcomes
close on artifacts.
