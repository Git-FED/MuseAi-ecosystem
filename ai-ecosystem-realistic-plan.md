# AI Ecosystem Realistic Plan

Date: Nov 25 2026
Built from: the original plan at ~/workspace/ai-ecosystem-plan.md, plus the three verification receipts in ~/workspace/ai-ecosystem-verification/
- 01-technical-feasibility.md: feasible with changes
- 02-legitimacy.md: Etsy copying is out
- 03-money-realism.md: worth it only if narrowed

Status: PLAN ONLY. Nothing built yet. No side chats opened, no Muse slot created, no accounts, no listings.

## What changed from Andrew's version

Andrew's numbers are not a forecast. Do not budget on them.
- $532.47 across 16 Etsy orders is $33.28 per order in revenue, roughly $130 to $300 profit in total, not $532.
- $16,000 in two months needs 481 orders at that value, about $2,667 a month per store. That is 4.6x the median Etsy seller and 9 to 16x a beginner print on demand store.
- $3,400 thumbnails at $20 is 170 thumbnails, $2,720 net after Fiverr's 20 percent, with no period given.
- $1 trillion is a slogan, not a forecast.

Realistic target for the first 90 days across the first 10 rooms: $0 to $1,000 total profit, most likely low hundreds. Realistic 12 month outcome, if Etsy and one prototype compound: a few hundred to low thousands a month, not $8,000 a month in two months.

## The structure, fixed

100 side chats is the long term shape, not the starting shape. One room is one side chat, one venture, one job. No room does two jobs.

The reporting loop is pull only, not push. Side chats do not self report. That is the biggest technical finding.
- A scheduled sweep opens each room, asks for a capped report, and collects it.
- The ecosystem Muse consolidates those reports.
- It sends the consolidated digest to Muse3 through the relay.
- Muse3 ranks it and tells Git-FED.

Relay hard caps, verified live Nov 25, health 200, service museaichat2-new-files:
- One relay message max 20,000 chars.
- Inbox keeps only the last 200 messages per recipient.
- No broadcast. Every report must be addressed to muse3 explicitly.
- Poll with a since watermark and archive each chunk to a file immediately. Do not rely on the inbox as storage.

Per room report format, capped by design, target under about 600 chars:
1. Revenue
2. Orders
3. What sold
4. What is stuck
5. Next action

At 10 rooms that is about 6,000 chars, 1 relay message. At 100 rooms that is about 60,000 chars, 3 relay messages, numbered 1/3, 2/3, 3/3. If a room report is verbose, the count grows and the inbox rolls faster.

Muse3 only ever sees the digest, never 100 room contents in one turn. At 100 rooms the sweep must be sharded across subagents, with per room state files, the same 6 slice pattern used for the 190 chat read on Nov 12.

Phase 3 dashboard means Muse3's daily chat ranking first: top 5 and dead 5. A separate live dashboard app is a second build, with its own host and data source, not included here.

## Legitimacy rules, non negotiable

Etsy copying method: OUT, entirely.
- IN: research on niche, colour, format, and price only, never the design itself. Original designs from Git-FED's own prompts, with human creative input.
- OUT: copying a selling design and changing it slightly, using another seller's photo, design, pattern, or listing text, brand names, logos, characters, song lyrics, team names, or trademarked slogans in design, title, tags, or description without a licence, fan art or inspired by designs without a licence, and any change it by 10 percent or 20 percent rule. No such rule exists.
- Disclose Printify as production partner on every applicable listing, and disclose AI use in the listing description where AI was used.
- No bot generated listings. A human must be involved in each listing.
- Three shops must not carry the same catalogue. Each shop needs a distinct product line and brand, its own account and email, and all shops listed in the Public Profile of each account.
- Consequence if run as written: listing removal, Printify product block, repeat infringement termination of selling privileges at Etsy's discretion, and refusal of service if a new shop is opened after termination.

Fiverr thumbnails:
- Git-FED's own account only, one account, in his own name.
- Thumbnails must be original and meaningfully refined and customised for each client. Pure unmodified AI output, reused across clients, or copying a competitor's thumbnail is out.
- No client logos, characters, or copyrighted images without rights. No deepfakes, no impersonation.
- Honour a client request for non AI work. Keep all communication and payment on Fiverr.
- Human in the loop reviews, edits, and delivers each thumbnail. A hands off agent only pipeline was not verified as compliant.

Game assets:
- Sell only original sprites, tilesets, UI, audio, or code, or work with a clear commercial licence. Do not resell or repackage assets bought from Unity Asset Store, itch.io, or other marketplaces.
- State the licence in writing on each listing. Check each marketplace's AI content rule before uploading, and disclose AI use where required.

Blogs and affiliate:
- Clear disclosure at the top and near the link on every post with an affiliate link, in plain language. No footer only disclosure.
- No fake reviews, no AI generated testimonials from non existent people, no reviews by someone with no experience of the product. Do not present a site Git-FED controls as an independent review site.

Software prototypes and App Store:
- Original work only, or code and assets with a licence that permits commercial sale and redistribution. No copied repos, no stolen assets, no licence incompatible open source code in a paid product.
- No deceptive claims about what the app does, what it connects to, or what data it collects. Privacy, data collection, and payment terms must be stated.
- The Muse AI App Store's own terms, refund policy, and payment rails are unverified. Same for FedPromptly shop catalogue and terms. Those must be checked before those rooms are ranked on money.

Music: NOT in the first 10.
- Streaming pays about $0.003 to $0.005 per stream, $3 to $5 per 1,000 streams, and a track must clear 1,000 streams in 12 months before it earns any recording royalties.
- Pure AI tracks: do not claim US copyright in the AI generated material, and do not claim section 115 mechanical royalties as owner of a non human work.
- No voice clone or likeness impersonation without permission. No mass upload spam to game streaming algorithms.

Sports betting:
- Git-FED, and only Git-FED, places his own bets, in his own name, on his own account, on Hard Rock Bet (21 plus, in Florida) or Kalshi (18 plus, under its own terms), with his own money. No Muse, agent, or other person places a bet for him, logs in to place a bet, or uses automation to place bets.
- Muse2 stays bookkeeper and analyst only: tracking results, bankroll, and lines, and reporting them. It must not take or receive wagers from anyone, accept money to bet on their behalf, charge a percentage on wagers, or settle bets with third parties.
- Do not run a shared bankroll, a syndicate, or a paid picks service that takes a cut of winnings without a specific legal check first.
- Latest on file, Nov 24: real 30-14, minus $5.37, practice 227-100, plus $37.69 paper. The real book loses money despite a 68 percent win rate. Count betting as $0 income. Do not increase stakes on current evidence. Keep records for tax.

FED-SPA:
- List licensed Florida massage establishments only, with licence number, address, and phone number shown, and no language suggesting prostitution, escort, or sexual services.
- Do not list unlicensed establishments as if licensed. Do not publish ads that omit the licence number.
- FED-SPA's actual listing criteria, licence verification, current wording, and whether it takes payment are unverified. Those facts decide whether the current FED-SPA is low risk or high risk, and must be checked before that room is scaled.

## The first 10 rooms, on money alone

This replaces the original Phase 1 list. The original spent 2 of 10 rooms on the two slowest lanes (second blog, music) and 3 rooms on cold Etsy stores before one had sold.

1. Etsy POD Store 1. One niche, 50 plus listings target, the compounding lane. Original designs only.
2. Thumbnail service, Fiverr. Fastest first dollar. Test $20 on Fiverr, and in parallel test one direct to creator price ($75 to $150) with the same portfolio.
3. FedPromptly shop. Existing payer, measure actual sales for 30 days. Do not budget income until a sale is verified.
4. FED-SPA. Existing payer, measure actual sales for 30 days, under the licensed only rule above.
5. Muse AI App Store / software prototype 1. One product that already exists, list it and measure. Do not build a second prototype until this one sells.
6. Etsy POD Store 2, different niche. Only after Store 1 makes its first sale. Diversification, not duplication.
7. Game asset pack 1. One pack, itch.io or Fab, passive tail.
8. Blog / affiliate 1. One blog only, slow compounder, cheap to run.
9. Betting reporting room. Track the book, count $0 as income, do not increase stakes. Included because it is already running and cheap to track, not because it pays.
10. Etsy research room (Nova). Feeds Room 1 and Room 6. Not a seller, but it decides whether the Etsy rooms list what sells. Without it, the Etsy rooms are guessing.

Dropped from the first 10 on money alone: music, second blog, third Etsy store, second prototype. Add each only after the lane it follows has sold.

Ranking, first 90 days profit:
1. Thumbnails
2. Etsy POD
3. Existing payers, unverified, leverage only
4. Software prototypes
5. Game assets
6. Blogs and affiliate
7. Betting
8. Music

## Phases, with gates

Phase 0: Provisioning, before any room opens.
- Git-FED creates the ecosystem Muse slot himself, if a new slot is the choice. How a new slot is created, who must create it, whether there is a cap or cost, is unverified. Do not assume Muse3 can create another Muse account on its own.
- Issue the new slot the RELAY_SECRET key, and give it the museaichat2 client, not the old bus.py default.
- Test one send and one inbox read before opening any room.
- Confirm the three existing payers: FedPromptly shop catalogue and terms, FED-SPA listing criteria and licence verification, App Store terms, refund policy, and payment rails. All three are unverified today.
- Confirm Etsy Store 1 niche, and confirm music stays out for now.

Phase 1: Prove, days 1 to 30, 10 rooms as listed above, with Room 6 gated on Room 1's first sale.
- Daily sweep collects the 5 line report from each room. Ecosystem Muse consolidates to 1 relay message. Muse3 reports the digest to Git-FED.
- Measure, do not assume: actual sales, actual revenue, actual profit after fees, actual hours.
- Day 30 decision: any room with $0 revenue and $0 orders after 30 days is reported as dead, per the Lyft dead night rule. Close it or repurpose it. Do not hide it. A room that sold once stays. A room that sold repeatedly scales.

Phase 2: Scale only what proved, days 31 to 90.
- Add a second room only in a lane that sold. Example: Store 2 after Store 1 sold, second prototype after prototype 1 sold, second blog after blog 1 made a sale.
- Do not scale to 25 rooms on a calendar date. Scale on sales.
- At 25 rooms, the sweep must already be sharded. Muse3 still only sees the digest.
- Day 60 and Day 90 decisions: rank top 5 and dead 5 each time. Kill the dead 5, or repurpose them with a new niche and a new 30 day test.

Phase 3: Scale toward 100, only after Phase 2 proves.
- 100 rooms is 50 hours a day at even 30 minutes a day per room. That cannot be manual. Scaling to 100 requires the sweep, the per room state files, and the human review step to be proven at 25 first.
- No room opens until the lane it belongs to has a sale on file, or a 30 day measurement that justifies it.
- The visual space station layer is last and optional. It is a display, not the system. Build it only if Git-FED wants the tour video.

## Costs to plan on

Etsy: $0.20 per listing, 6.5 percent transaction fee, 3 percent plus $0.25 payment processing, about 10 to 13 percent before Offsite Ads, up to about 20 percent if Offsite Ads drive the sale. Printify tee base $8.80 to $10.98, shipping $3.50 to $5.00. Net per sale roughly $4 to $12 on a $24 to $30 tee. $500 a month profit needs 62 to 100 sales a month.
Fiverr: 20 percent flat, $20 gross is $16 net, earnings clear after 14 days. 170 thumbnails is 85 to 170 hours at 30 to 60 minutes each.
Game assets: Unity keeps 30 percent, Fab keeps 12 percent, itch.io default 10 percent, adjustable to 0 percent.
Software: Gumroad 10 percent flat, Lemon Squeezy 5 percent plus $0.50.
Music: distributor about $20 to $50 a year, plus hours per track. Not in the first 10.
Betting: vig about 4.5 percent of money wagered at minus 110. The cost is negative expected value and bankroll risk, not a platform fee.

## Kill and scale rules

- Dead: $0 revenue and $0 orders for 30 days after launch, with the room actually running. Report it, close it or repurpose it with a new niche and a new 30 day test.
- Prove: first sale within 60 days for Etsy, first thumbnail order within 1 to 4 weeks, first prototype sale within 2 to 4 weeks if listed where buyers are, first blog sale in months 3 to 6.
- Scale: only a lane with a sale on file gets a second room. No second room on hope.
- Stop: any rights holder report, Printify block, Fiverr warning, or affiliate program warning stops that room immediately for review. Do not list around it.

## Decisions Git-FED still has to make

1. Ecosystem Muse: brand new slot, or repurpose an existing Muse. If new, he creates it, per Phase 0.
2. Etsy Store 1 niche. Research room cannot pick it for him without his call on what he wants to sell.
3. Thumbnail direct price test: yes or no on $75 to $150 direct to creator, in parallel with $20 Fiverr.
4. Confirm the three existing payers are in as measurement rooms, with their current terms checked, or hold them out until checked.
5. Confirm betting stays reporting only, $0 income, no stake increase.
6. Confirm music stays out of the first 10.
7. Space station visual: yes or no, last only.

## What this plan does not do

- It does not copy Andrew's claims as facts.
- It does not copy designs that already sell.
- It does not build the game.
- It does not open 100 rooms at once.
- It does not count betting paper profit as income.
- It does not count existing payers as income until a sale is verified.
