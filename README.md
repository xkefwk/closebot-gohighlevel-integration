# CloseBot GoHighLevel Integration: Connect Your First Sub-Account, Wire the Tags, and Pick the Right Plan

Most people searching for the CloseBot GoHighLevel integration are standing in one of two places. Either they've got a GHL sub-account full of leads that go cold before anyone replies, or they've been testing HighLevel's native Conversation AI and want to know whether a third-party agent is worth the extra line on the invoice.

Both questions have concrete answers, and neither requires a five-part funnel to explain. Here's how the connection actually works, what breaks when it doesn't, and what each plan costs at the volume you're probably running.

## What the CloseBot GoHighLevel integration actually is

CloseBot isn't a standalone chatbot that talks to Instagram or your SMS provider directly. It connects to your CRM and answers whatever conversations land in that CRM's inbox. In CloseBot's own documentation, that's what a "Source" is: HighLevel, LeadConnector, HubSpot, or a generic webhook.

So the honest version of the setup is this: GoHighLevel carries the channels, CloseBot carries the brain. If Instagram DMs and WhatsApp already flow into your GHL Conversations inbox, a CloseBot agent can reply to them. If you don't run a CRM at all, CloseBot isn't a shortcut around that — you'd be buying a CRM first and layering this on top.

Three things worth knowing before you start connecting anything:

- **It doesn't run your GHL workflows.** CloseBot has its own drag-and-drop flow builder, and if you're migrating from a workflow-based bot, you'll rebuild those flows inside CloseBot. Tags are the bridge back into GoHighLevel automations.
- **One CloseBot account can hold multiple GHL sub-accounts.** The free plan already lists unlimited account connections; the paid difference is about agents, volume, and rebilling.
- **CloseBot calls itself the most-installed lead qualification app in the HighLevel marketplace.** That's a vendor claim, not an audit, but it's consistent with how often the tool comes up in GHL agency discussions.

## Connecting CloseBot to a GoHighLevel sub-account, step by step

You need two things: a CloseBot account (the free tier works for this) and a GHL sub-account you're allowed to authorize.

1. In CloseBot, open **Sources** and click **New Source**.
2. Pick **HighLevel Sub-Account** (there's a separate LeadConnector option) and hit **Connect**. An OAuth popup opens.
3. Sign in to HighLevel if you aren't already, and choose the workspace or account you want to authorize.
4. In the permissions tab, scroll down and approve the CloseBot app permissions, then pick the sub-account you want to connect.
5. Back in the CloseBot tab, tick **Allow CloseBot to create/update fields**. This is the checkbox that lets your agent write to custom contact properties. Skip it and your agents will read but not save.
6. Click **Add Source**. You land on the Sources list with the connection confirmed.

That whole sequence takes minutes, not hours. CloseBot markets a "48 second setup" where a starter agent is auto-created for the industry you picked at signup, and for a basic Q&A bot, that's about right.

The gap between that and a production agent is where the real work lives. Independent reviewers put a proper build at somewhere in the range of 5 to 10 hours once you factor in knowledge base uploads, job flows, and testing. Budget for that, not for the 48 seconds.

👉 [Start with a free CloseBot account and connect your first sub-account](https://app.closebot.com/a?fpr=li87)

## Where GoHighLevel and CloseBot actually hand off

The integration is more interesting in what it hands back to your CRM than in the OAuth dance.

**Tags are the handshake.** CloseBot's "Modify Tags" action adds or removes tags on a contact. Pair that with a GoHighLevel workflow triggered by a tag, and you get internal notifications, pipeline stage moves, invoice triggers, and webhook calls — things CloseBot won't do itself. One detail that trips people up: HighLevel and LeadConnector only allow lowercase tags, and CloseBot auto-formats them to lowercase for you. If your automation is listening for `HotLead`, it will never fire.

**Tags also decide which agent talks to whom.** Source filters let you route conversations to different agents based on tags or channel. A contact tagged as already booked can be pushed out of your qualification flow entirely, and a Spanish-speaking lead can hit a different agent without you duplicating the whole build.

**Custom fields update without the usual cap.** GoHighLevel's own AI opened up to around 20 custom contact fields; CloseBot has updated unlimited fields since its early version, including on the free plan. For anyone qualifying on square footage, property type, or service tier, that difference shows up fast.

**Booking stays conversational.** A single CloseBot agent can offer times across different calendars and handle reschedules and cancellations inside the chat, which is the part that usually forces people into building multiple native bots.

## When the wiring goes wrong

CloseBot has a decent diagnostic habit: if an agent doesn't respond, clicking the contact or conversation tells you why. Still, the failures cluster into a handful of familiar patterns.

| Symptom | Likely cause | Fix |
| --- | --- | --- |
| No message appears in the CloseBot queue at all | Source not added, source already installed on a different CloseBot account, or the connection dropped | Reconnect the source. If it keeps dropping, it's a CRM-side issue, not a CloseBot one |
| Message shows in the queue, agent stays silent | Source filters (tag or channel) exclude that conversation | Check the tag and channel filters on that source |
| A tag-triggered GHL workflow never fires | Tag case mismatch | Use lowercase tag names everywhere |
| Costs climb faster than your message count suggests | Agent Node is running with unlimited potential unlocked | Thinking mode, "intelligence max," and unlimited tools bill by segments or tokens instead of one message |

That last row is the one people miss. A "message" is normally one segment. Turn on the unlocked Agent Node settings and a single reply can consume several segments — still rebillable on the agency plan, but your margin math needs to account for it.

> If a source disconnects, CloseBot's own docs say to raise it with your CRM's support team rather than CloseBot's. That's worth knowing before you spend an afternoon in the wrong queue.

## CloseBot vs GoHighLevel's native Conversation AI

GoHighLevel's built-in AI got better, and plenty of operators say it's fine for simple SMS qualification. Where it still gets called clunky — in GHL's own subreddit, no less — is exactly the SMS back-and-forth that most local businesses live on.

|  | CloseBot | GoHighLevel native AI |
| --- | --- | --- |
| Pricing model | Business from $64/mo with messages included; agency $0.012/message, rebillable | $0.02/message pay-as-you-go, or $97/sub-account/month for AI Employee unlimited |
| Builder | Drag-and-drop job flows with objectives, agent nodes, tools, and exits | Prompt-driven, with a drag-and-drop builder still rolling out |
| Channels | Whatever your CRM carries, including email replies and image handling | Chat and SMS focus; email replies and inbound images are gaps |
| AI providers | OpenAI, Anthropic, Gemini, Grok, DeepSeek, with automatic fallback | OpenAI-based |
| Custom fields | Unlimited (including free plan) | Capped |
| Agents per sub-account | Multiple, split by channel or tag | One bot per sub-account, handoffs get clunky |
| Agency reselling | White-label portal, client seats, rebilling at your markup | Rebillable usage, no white-label portal |

The cost comparison depends entirely on scale. At four sub-accounts, AI Employee unlimited is roughly $388/month. At 102 sub-accounts it's nearly $9,900/month, which is the number that pushes high-volume agencies to a usage-based tool.

None of this makes CloseBot untouchable. Long-time users in GHL communities have complained about reliability and support runarounds, and one recent thread describes an agent confidently making things up over a weekend. If your offer depends on AI handling every inbound lead unsupervised, plan for monitoring and knowledge-base maintenance. Distrust of a single LLM is also why the multi-provider fallback matters — when OpenAI wobbles, the agent can keep answering.

## Full CloseBot plans and pricing

Prices below are from CloseBot's current plans page. Nothing here is discounted by a hidden link trick — the plan tiers are the same however you sign up.

| Plan | Who it's for | What's included | Price | Billing | Get it |
| --- | --- | --- | --- | --- | --- |
| Free | Testing the tool, or very low lead volume | 100 AI replies/month, 1 agent, 1 user seat, 1 MB knowledge storage, unlimited account connections, always free | $0 | No card, no expiry | [Start on the free plan](https://app.closebot.com/a?fpr=li87) |
| Core — Business | Businesses automating their own qualification and booking | Business entry tier includes 500 monthly messages with message costs baked into the base price, 15+ templates, human support; additional agents, seats ($5 each) and storage are add-ons; 50+ extra templates unlock on annual billing. Price scales up with the monthly AI reply volume you select | From $64/mo (annual billing shows $53/mo, billed as $640/yr) | Monthly or annual, month-to-month, cancel anytime | [Pick your business volume](https://app.closebot.com/a?fpr=li87) |
| Core — Agency | Agencies building and reselling AI agents to clients | Unlimited agents across unlimited sources, white-label client portal, rebill all costs, invite additional users at $5/seat, add storage and agents. Messages billed at a flat $0.012 each and fully rebillable at your own markup | $397/mo | Monthly, month-to-month | [Open the agency plan](https://app.closebot.com/a?fpr=li87) |
| Growth | Operations that need contracts, compliance, or serious volume | 50+ templates, HIPAA compliance, quarterly audits, 99.99% priority uptime, priority support, custom scope | Custom — talk to sales | Custom | [Request a Growth quote](https://app.closebot.com/a?fpr=li87) |

A few things the table can't show:

- **Every paid plan includes a 7-day trial, and CloseBot does not issue refunds.** The free plan and the trial are the risk-free windows. Use them.
- **Annual billing is cheaper and unlocks more templates.** The business entry tier drops to a $53/month equivalent when billed yearly.
- **The coupon is real and small.** CloseBot's own blog publishes `CLOSEBOT100OFF` for $100 off your first payment, valid on business and agency plans. Third-party coupon pages recycle codes that may be expired; treat the official one as the safe bet.
- **Your GoHighLevel subscription is separate.** GHL starts around $97/month, so the honest total for a small business on the $64 tier is closer to $161/month before any message overage.
- **No bring-your-own API key.** CloseBot removed that requirement in its November 2025 pricing update. Model spend is inside the plan price now, which means you can't shave costs by plugging in your own Anthropic key.

## Which plan actually fits

If you run inbound conversations for one business and stay under 100 replies a month, the free plan is not a demo — it's a working setup, and it lets you see booked appointments before you pay anything.

Between roughly 500 and a few thousand monthly messages, the business tier at $64 and up is the simpler economics: message costs are included, so your bill doesn't swing with volume.

The agency plan only makes sense if you're charging clients. At $397/month with messages at $0.012 and rebillable, the margin is in what you charge, not in what CloseBot charges you. Polled CloseBot agencies report billing an average of $500 per client per month, a figure CloseBot publishes on its pricing page — and one that makes the base fee look small next to the spread.

Skip both if your only goal is cheap SMS qualification and you're happy with GoHighLevel's native AI. The pay-per-message route there is pennies at low volume, and "good enough" is a legitimate answer.

## FAQ

**Does CloseBot replace GoHighLevel?**
No. It sits on top of your CRM and answers the conversations your CRM already carries. You keep GHL; CloseBot takes over the qualifying and booking.

**How long does the integration take?**
The source connection is a few minutes. A production-ready agent with knowledge, job flows, and tested booking is a multi-hour project.

**Do I need my own OpenAI or Anthropic API key?**
No. Current plans don't allow bring-your-own-key, and model costs are included. Older documentation that mentions API keys is out of date.

**Can I answer Instagram and WhatsApp messages with it?**
Only if those channels are connected to your GoHighLevel inbox. CloseBot has no direct Instagram or WhatsApp connection of its own.

**Can one account manage multiple client sub-accounts?**
Yes, account connections are unlimited across plans. Rebilling and white-labeling are what the agency plan adds.

**Is there a free trial?**
Yes, on any paid plan — 7 days. Combined with the free-forever tier, that's your entire testing window, since refunds aren't offered.

## The short version

The CloseBot GoHighLevel integration is a Source connection, a permissions checkbox, and about ten minutes of clicking. The work that decides whether it pays for itself happens afterward: writing job flows that match how your leads actually talk, keeping the knowledge base current, and watching tags so your GHL automations fire.

Start on the free plan, connect one sub-account, and run it against real leads for a week. You'll know whether the conversation quality clears your bar long before the trial clock runs out.

👉 [Connect CloseBot to your GoHighLevel sub-account for free](https://app.closebot.com/a?fpr=li87)
