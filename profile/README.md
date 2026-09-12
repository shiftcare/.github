# What is ShiftCare?

ShiftCare is one system for care and disability providers — NDIS, aged care, home care and
allied health — across Australia, the US, Canada and the UK. Every referral, shift, note,
claim and dollar runs through the same record: rostering, care delivery, documentation,
compliance, billing and margin.

The award engine checks each shift as it is rostered, while the roster is still editable —
SCHADS and enterprise agreements in Australia, FLSA and California overtime in the US. Shift
costing shows what a shift costs, earns and returns before it is worked.

This organisation is the developer side of that: what an AI agent, and the person wiring one
up, needs to work against a real ShiftCare account.

## Roster, timesheet, invoice — one record

A coordinator rosters a shift. The hours worked land on a timesheet against that same shift.
The invoice is built from it. Nothing gets re-typed between three systems, because there
aren't three systems.

The MCP server exposes those objects directly — shifts and recurring series, timesheets,
invoiceable items, invoices, invoice runs and payments — so an agent works on the record
itself rather than a copy of it.

**Integrations.** Your HR, payroll and accounting systems connect to the same record.

* **Payroll** — Xero, QuickBooks Online, MYOB AccountRight, Employment Hero, ADP, Paychex,
  Viventium
* **Accounting** — Xero, QuickBooks Online, MYOB AccountRight
* **Award interpretation** — PayCat Connect

Availability varies by region. Shift costing is built in for the US, Canada and the UK, and
draws from Xero AU or PayCat Connect in Australia.

## What's here

**[ai-skills](https://github.com/shiftcare/ai-skills)** — eleven skills that teach AI coding
agents how to work with ShiftCare through the ShiftCare MCP server. Tested with Claude Code
and Codex.

```
npx skills add shiftcare/ai-skills
```

**The ShiftCare MCP server** — regional endpoints for Australia, the US, Canada and the UK.
On by default for accounts created from 24 August 2026; older accounts switch it on under
**Account → AI Settings**.
[Start here](https://help.shiftcare.com/en/articles/14649246-introduction-to-the-shiftcare-mcp-server)
· [Claude setup](https://help.shiftcare.com/en/articles/14612387-connecting-shiftcare-mcp-to-claude)
· [ChatGPT setup](https://help.shiftcare.com/en/articles/14630405-connecting-shiftcare-mcp-to-chatgpt)

## What you can do with it

* Sweep staff credentials for expired, expiring, missing and unverified records — before an
  audit finds them.
* Get yesterday's and today's shifts back grouped by urgency, with the next step on each.
* Create or cancel a shift from a plain-language request. Every write is confirmed first, and
  a cancellation asks the question that matters: charge the client, or don't pay the carer.
* Write a client note or a shift progress note, routed to the right one.
* Lodge a complaint, route a related incident, and assign the corrective action off the back
  of it.
* Score a new account's setup and get the help article for each gap.

Access follows the signed-in user's existing ShiftCare permissions. Reads are read-only.
Writes stop and ask.

## Try it

Once MCP is on and the skills are installed, that's the interface:

```
What needs my attention today?
```

Yesterday's and today's shifts come back grouped by urgency, with a next step on each finding.

## Explore ShiftCare

* [See the product](https://shiftcare.com)
* [Help centre](https://help.shiftcare.com)
* [Connecting an AI assistant to your care data](https://shiftcare.com/blog/connecting-ai-assistant-your-care-data)
* [Turn on MCP for your account](https://help.shiftcare.com/en/articles/14636328-managing-ai-settings)
* [Partner with us](https://shiftcare.com/partners)
* [Report a security issue](mailto:security@shiftcare.com)

<sub>Forked repositories in this organisation are dependency pins, not projects.</sub>
