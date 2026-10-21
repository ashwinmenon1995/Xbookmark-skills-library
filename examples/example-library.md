> Example only: this is one example library whose categories came from one person's bookmarks, and yours will differ.

# skills.md — Public AI skills library

Techniques, workflows and tool capabilities for AI agents and AI tools, extracted from public posts, articles and videos. Each entry is a summary in our own words plus a link to the source — read the original for full detail. See README.md for how to contribute.

> **How to append:** add new entries at the END of the matching category section (or under "Appended entries" at the bottom if no category fits) using the exact entry template below, then add the ID to that row of the Index and bump its count. Never rewrite existing entries. Each entry gets a unique ID `S-###` (next free number).
>
> Entry template:
> ```
> ### S-### · Title
> - **Source:** @handle · post date · url
> - **Access:** full text | full transcript | title only (couldn't access) | post text only (body/thread not retrievable)
> - **Added by:** name or agent · YYYY-MM-DD
> - **What it does:** …
> - **How to use it:** …
> - **Key details / steps:** …
> ```
> Initial import: 2026-10-21. Claims and numbers are the source authors' own and are not independently verified. Nothing here is financial, legal or medical advice.

## Index (by skill type)
| Category | Count | Entries |
|---|---|---|
| [1. Growth & organic distribution](#1-growth--organic-distribution) | 11 | S-001, S-002, S-003, S-004, S-005, S-006, S-007, S-008, S-009, S-010, S-074 |
| [2. Marketing, copy & launches](#2-marketing-copy--launches) | 7 | S-011, S-012, S-013, S-014, S-015, S-016, S-017 |
| [3. Paid ads & creator programs](#3-paid-ads--creator-programs) | 6 | S-018, S-019, S-020, S-021, S-022, S-075 |
| [4. Sales / GTM & outbound](#4-sales--gtm--outbound) | 4 | S-023, S-024, S-025, S-026 |
| [5. SEO / AEO (AI search)](#5-seo--aeo-ai-search) | 4 | S-027, S-028, S-029, S-073 |
| [6. Automation & AI agents (incl. Grok Bot)](#6-automation--ai-agents-incl-grok-bot) | 10 | S-030, S-031, S-032, S-033, S-034, S-035, S-036, S-037, S-038, S-039 |
| [7. Research & market intelligence](#7-research--market-intelligence) | 4 | S-040, S-041, S-042, S-043 |
| [8. Coding & building](#8-coding--building) | 4 | S-044, S-045, S-046, S-047 |
| [9. Design / creative (web, image, video)](#9-design--creative-web-image-video) | 10 | S-048, S-049, S-050, S-051, S-052, S-053, S-054, S-055, S-056, S-057 |
| [10. Ecom & conversion (CRO)](#10-ecom--conversion-cro) | 4 | S-058, S-059, S-060, S-061 |
| [11. Founder, strategy & fundraising](#11-founder-strategy--fundraising) | 5 | S-062, S-063, S-064, S-065, S-066 |
| [12. Quant / prediction-market methods (educational)](#12-quant--prediction-market-methods-educational) | 2 | S-067, S-068 |
| [13. AI/ML understanding & mental models](#13-aiml-understanding--mental-models) | 4 | S-069, S-070, S-071, S-072 |

---
## 1. Growth & organic distribution

### S-001 · Phase plan: 0 → 100M organic views/month
- **Source:** @domschats · 2026-10-10 · https://x.com/domschats/status/2109071150089445424
- **Access:** full text (X article "How to go from 0-100M views/month")
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Stage-by-stage org + channel plan for organic social.
- **How to use it:** Diagnose your phase, apply that phase's team and channel thresholds.
- **Key details / steps:** Phase 1 (0→1M/mo): founder-led content, daily posting, 1–2 "launch videos"/week (can be simple product-update posts); avoid the "distribution by any means" trap — off-topic viral views (the "gorilla marathon" example) attract followers who won't engage with product content and poison later reach. Phase 2 (1→10M): invest in a channel once it's winning — LinkedIn >10k avg impressions/post, X 50k+/week, IG with thousands/video and 1–2 100k outliers/month; hire copywriter/Head of Content (LinkedIn+X), short-form editor (10M+ organic views track record, targets 500k/wk IG, 250k+ X), creative director for launches. AI skill: auto-send founder meeting transcripts (confidential parts stripped) to the copywriter as raw material. Phase 3 (10→100M): shift founder-led → brand-led, 20+ daily posts across brands/founders/EGC, 10–20 person media team in per-channel pods.

### S-002 · Brand-market fit & funnel content system
- **Source:** @ryangrowthh · 2026-10-12 · https://x.com/ryangrowthh/status/2109644746465726929
- **Access:** full text (X article "How to Grow a Massive Brand (Full 2026 Masterclass)")
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Positioning + content architecture for organic brand growth.
- **How to use it:** Define BMF, then allocate content across funnel and pillars.
- **Key details / steps:** BMF = audience instantly gets what you stand for, wants more, can't get it elsewhere. Positioning: own/create a category (often combining two hot niches, e.g. AI×trading), first-mover, specific pain. Decide the emotion; tell the story publicly (honest takes, face on camera — "doxxing kills ~80% of competition"); audience is the hero; same message everywhere. Run founder account (why/beliefs/lessons) + brand account (launches, campaigns). Funnel: TOF (trends, outlier formats, clips) → MOF (how-tos, long-form, case studies, BTS) → BOF (demos, testimonials, offers, lead magnets, FAQs); skew mix by account type (news account ~90% TOF; product IG ~90% BOF). Pillars (3–5) = overlap of audience cares × your credibility × product. Rent on socials, own via newsletter from day one. Cult community: name, recognition, visual identity, shared language, qualification, a home, rituals (weekly events, IRL meetups, spotlights, challenges).

### S-003 · Outlier-score research engine for short-form
- **Source:** @0x_fokki · 2026-07-08 · https://x.com/0x_fokki/status/2074798903124259223
- **Access:** full text (article "How I Predict Viral Videos Before They Explode"; the Claude prompt blocks were images and are not in the text)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Finds formats that are working now and reskins them.
- **How to use it:** Track ~40 channels in one lane in a Sheet; score; feed winners to an LLM.
- **Key details / steps:** outlier score = video views ÷ channel median views; >10 = signal, >30 = copy this week. Separate topic (dies in ~a week) from format (repeats for months); log the exact first frame and first on-screen text line. Paste 20 outlier titles/hooks into an LLM to extract the skeleton and generate ~30 concepts; script "for shots, not prose". Reusable formats: "POV: you're the [role] when [event]", "What if [thing] but [twist]", invisible-force gag, oddly satisfying process, 1 vs escalation, creature reveal, "day in the life of [unexpected]". Loop: Make.com scenario — new video in Drive → post to TikTok/Shorts/Reels → after 48h pull views → write outlier score back to the same sheet → Telegram ping of the week's winning format. Format window ≈ 2 weeks. Author's cost claim ~$50/mo tools.

### S-004 · Fresh-account IG growth: warm-up + 7-second format
- **Source:** @KCodes7777 · 2026-04-07 · https://x.com/KCodes7777/status/2041613931899154554
- **Access:** full text (article "I got 1.3M views on a new IG account in 2 weeks")
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Zero-budget organic playbook for an app/product page.
- **How to use it:** Follow the day-by-day warm-up then post one fixed format daily.
- **Key details / steps:** One specific niche; new account with contact upload OFF (Accounts Center → Your info and permissions → Upload contacts, or iPhone Settings → Instagram → Contacts); display name includes niche keyword (indexed for search); bio = what + who + CTA; logo + 5 highlight covers before posting. Warm-up: D1–2 follow 10–15, like 20–30, 5 comments; D3–4 like 30–40, comment 10, save 10–15 performing posts, watch Reels to completion; D5–6 build saved reference library; D7 first post. Format: free stock clip (Pexels/Canva) cut to exactly 7s, hook text on screen whole time, last 3s add "read description below…", long value caption (5 bullets matching "5 things…" hook) → replays + time-on-post. Hook template "5 [signs/things/reasons] that [outcome]"; negative/warning/mistake framings outperform; reassurance also spreads. Post 2×/day then 1×/day; CTA in caption, corner overlay, bio link.

### S-005 · Why TikTok/IG videos stall under 1k views
- **Source:** @cesaralvarezll · 2026-03-17 · https://x.com/cesaralvarezll/status/2033891852621840387
- **Access:** full text (article; embedded example videos not viewable)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Two-cause diagnosis: account not warmed, weak hook.
- **How to use it:** Warm 3–7 days (10–30 min/day niche engagement), then 1 post/day; engineer the first 3 seconds.
- **Key details / steps:** Retention is the core metric. Hook types: visual (motion, transitions, start mid-action), text (on-screen title), verbal (question, bold statement, story start). When one hits, iterate on that format; repost top performers after 3–6 months.

### S-006 · X For-You algorithm signals + "movie-clip quote tweet" meta agent
- **Source:** @phosphenq · 2026-03-18 · https://x.com/phosphenq/status/2034281831885893893
- **Access:** full text (article "The AI Agent That Knows What's Viral"; code blocks were images, not captured)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Explains the open-sourced X ranking stack and a daily agent that detects the current winning format.
- **How to use it:** Score your feed/lists by engagement relative to author size, have an LLM extract patterns, recommend posts, track results, recalibrate weekly.
- **Key details / steps:** Per the article: xai-org/x-algorithm (Jan 2026) — Thunder (in-memory recent posts), Phoenix (Grok-based transformer predicting engagement), Home Mixer, Candidate Pipeline; 19 predicted actions (favorite, reply, repost, quote, click, profile_click, video_view, photo_expand, share, share_via_dm, share_via_copy_link, dwell, follow_author; negatives not_interested, block, mute, report; plus dwell_time, quoted_click). Mechanics: dwell time matters; author-diversity decay (each extra post of yours in a feed is discounted); out-of-network multiplier <1. Winning format observed: quote-tweet an article/announcement with a 10–20s emotional movie clip + 1–3 provocative lines. Other formats: "JUST IN:/BREAKING:" caps headlines, specific-number technical framing, threads whose first tweet stands alone. Note the article suggests Twikit scraping, which it itself flags as violating ToS — use official/connector access instead.

### S-007 · Mr. Beast-style X launch science (sample tests, QT networks)
- **Source:** @mattepstein · 2026-06-15 · https://x.com/mattepstein/status/2066664675542999369
- **Access:** full text (article "Using Claude to go Viral on X… (Mr. Beast's Framework)")
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Launch framework; author claims 25 viral X launches.
- **How to use it:** Engineer the 4 elements, pre-seed quote tweets, run the "sacred hour".
- **Key details / steps:** Author's model of X: post shown to ~300 people → pass → ~2,000 → larger pools by percentile. Paid vs earned attention: on X you earn every second — no slow intros, no "we're excited to announce", no vague category language. All four required: bold claim bigger than the product ("We raised $7.5M to kill AI slop"); immediate dopamine (coolest moment first); no context gaps (mom test on first 10s); strongest outcome (money > time; "sell the destination"). Quote tweets are new distribution nodes (example: a 3-word QT did 790k impressions) — pre-line up QT-ers with a one-sentence angle. Pre-launch research: what market loves/hates, the enemy, highest-status outcome, customers' exact words, most polarizing true claim; Claude drafts/pressure-tests ~30 claim versions. During: watch first-hour velocity, prioritize replies/QTs over likes, reply fast, add proof in replies, amplify rising QTs, answer objections. After: repurpose replies/QTs, clip, retarget on LinkedIn/email, build paid ads from organic winners.

### S-008 · Repurpose founder meeting transcripts into content
- **Source:** @domschats · 2026-10-10 · https://x.com/domschats/status/2109071150089445424
- **Access:** full text
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Turns all-day founder conversations into raw material for written posts.
- **How to use it:** Record meetings with a notetaker; agent strips confidential/private content and forwards to copywriter or drafts posts for approval. Author calls it "the single most valuable workflow for scaling impressions through written media".

### S-009 · Break-the-algorithm "tech fence" (personal attention hygiene)
- **Source:** @Jackkk (PewDiePie clip) · 2026-03-18 · https://x.com/Jackkk/status/2034179808184377698
- **Access:** full transcript (3.7-min clip)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Friction-based method to reduce compulsive scrolling.
- **How to use it:** Put social/attention apps in a second phone profile (the 5–6s switch is the friction); self-host tools you rely on; disable YouTube Shorts; optionally unfollow everyone; network-level DNS blocker for ads.

### S-010 · Hudson method (creator-seeded growth restart)
- **Source:** @Seanfrank · 2026-05-03 · https://x.com/Seanfrank/status/2051036381359849697
- **Access:** full text
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Creator-volume engine feeding all ad channels.
- **How to use it:** Seed hundreds of small/new TikTok creators; pay per video + commission with bonuses for 100+ videos/month; load all creative into every ad channel; scale spend while paying commission on ad sales. Author claims 6 brands restarted growth (5M→100M/yr).

### S-074 · LinkedIn founder process: zero → inbound in 90 days
- **Source:** @LoganTGott · 2026-07-29 · https://x.com/LoganTGott/status/2082466565346172937
- **Access:** title only (couldn't access) — the process is in an attached image; thread not retrievable.
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does / How to use it:** Placeholder — the steps are in an image in the post; anyone who reads it can append a fuller entry. Related: S-002, S-004.

## 2. Marketing, copy & launches

### S-011 · The 20 (+1) hills for a viral tech launch
- **Source:** @MitcheIl · 2026-06-18 · https://x.com/MitcheIl/status/2067703448137560400
- **Access:** full text (article "The Ultimate Playbook For A Viral Tech Launch")
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Launch-script rules from Shown Media.
- **How to use it:** Run your script through each rule before production.
- **Key details / steps:** Start with ICP (love/wish/hate); get out of your head; weirdly specific named/dated grievance; money beats time as motivator; sell the destination ("gets your kid into MIT" vs "AI tutor"); Mom Test the first line; enter the market's main argument ("Kill AI slop"); make it a little unbelievable; leave a door open for disagreement (Brilliant: "AI is making kids dumber" angered two camps → comments = velocity); keep the line that makes the client nervous; X is earned media — claim in ~5s, no montage; open on the most insane moment (retention cliff); bridge every leap; cast/coach a frictionless voice; execute within minutes; optimize for performance not beauty; hire YouTube-native strategists; go for the biggest video even for niche products; put the product inside the launch (Moda: founder replied to comments with decks the product built live). Bonus: ~300-person sample test decides reach.

### S-012 · Psychology of viral launch videos (retention engineering)
- **Source:** @mattepstein · 2026-07-15 · https://x.com/mattepstein/status/2077486346181226800
- **Access:** full text (article "The Psychology of Viral Launch Videos"; example videos not viewable)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Retention model + production process.
- **How to use it:** Design every second to answer three viewer doubts.
- **Key details / steps:** Retention cliff in first seconds, then sunk-cost flattening (after ~30s "I've come this far"). Doubt 1 "is this what I clicked?" (match caption/thumbnail/hook); Doubt 2 "seen it before?" (establish concept + show product at the start); Doubt 3 "will it bore me?" (example: 3M-view video with a shot change every 1.7s, <1 in 5 shots talking head). No sales talk/adjectives — demo the "aha" moment (Jobs' 2007 iPhone flick). Never let motion die (orienting response); no static UI screenshots; speed final video ~10%. Process: onboarding form (differentiator? what can be shown? backend to visualize? single most impressive thing?) → kickoff/demo → script around hook, pressure-tested by an internal "virality predictor" → founder talking head → Figma storyboard with real UI/brand → After Effects → review in Frame → ~10 full versions. Tools: Figma, Frame, After Effects, Premiere Pro, Photoshop, FL Studio, Slack.

### S-013 · Launch-video structure (visual template)
- **Source:** @abdinmotion · 2026-07-12 · https://x.com/abdinmotion/status/2076334604437332328
- **Access:** post text only — video has no speech (visuals carry the content — watch the original post). Author replies: made in After Effects + Figma storyboard + Premiere sound design, ~2 days, no AI tools.
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Annotated breakdown of launch-video sections.
- **How to use it:** Watch the video in the post and copy its section labels into your own storyboard template.

### S-014 · Unique mechanisms (UMP/UMS) for sophisticated markets
- **Source:** @codyplof · 2026-08-06 · https://x.com/codyplof/status/2085163125582541112
- **Access:** full text (article "Unique Mechanisms Explained")
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Copy framework giving buyers a new reason to believe instead of a bigger promise.
- **How to use it:** Write a UMP (why they failed before — external, not their fault) and a UMS (why this works differently), then a promise and a one-line explanation.
- **Key details / steps:** Sources: Stefan Georgi's RMBC, Todd Brown, Eugene Schwartz's market sophistication. Don't escalate claims ("6-minute abs"). Most buyers lack confidence; give an external reason for past failure. Examples: P90X "muscle confusion"; Plane Truth one- vs two-plane golf swing; Banjo Minnow "genetic response"; GLP-1s (biology not willpower — real mechanism); Grüns vs AG1 (adherence mechanism: gummies vs powder). Mechanisms can vary by persona/angle.

### S-015 · Kate Tolo's 11 rules for virality (Bryan Johnson / Blueprint)
- **Source:** @ColinandSamir · 2026-09-09 · https://x.com/ColinandSamir/status/2097739627306303803
- **Access:** full transcript (~50 min; auto-transcript noisy; printed examples shown on table — visual review helps)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Content system that took Blueprint from ~2,000 to 10M+ followers (her claims: $60M raise, ~300M monthly press reach).
- **How to use it:** Run each new post/email/thumbnail through the rules below.
- **Key details / steps:**
  - *Nightclub model:* every platform (YouTube, NYT homepage, an inbox, a phone home screen) is a club; the algorithm is the bouncer; your only job is to bring something that makes the people inside feel something (any strong emotion). Failure is invisible — a 100-view post is seen by almost no one, so post, post, post and follow small signals (200 views vs your 100 average).
  - *Never assume, always test:* e.g. two email CTAs — "nutritionally comparable to 1,808 calories…" vs "eat kilos of food or have one scoop"; simpler, emotional, visual wording tends to win; over-index on emotion vs rational specs.
  - *Start with text first:* write the story before visuals; visuals then follow the story (supplement capsules shot in a petri dish because the brand story is "a scientific experiment").
  - *Three-step writing:* (1) say it as simply as possible; (2) rewrite for value to the reader; (3) move the most "gossipy"/evocative element to the front (e.g. "90% of visible skin aging is from UV").
  - *Turn a press moment into a pitch / know your ticket price:* each club has its entry ticket — YouTube = title+thumbnail, press = headline, email = subject line; it's all copywriting.
  - *Ruthlessly create value:* if you induce fear for attention, soothe with a solution; if it gets too complex to hold in your head, strip back.
  - *If it works, say it again:* same tweet "Sleep is the most powerful drug…" got 220k views in 2025 and 348k in 2026; iterate small variants of winners ("longevity maxing" → "sleep maxing").
  - *Speak simply:* translate studies into human lines ("Own a dog: 63% lower dementia risk").
  - *See it in context:* preview copy in the real format (line wraps, hanging words); judge packaging on the actual shelf.
  - *Publish immediately / timely vs timeless:* skip content calendars; the slow "middle" (2 weeks of production for non-timely content) is dying.
  - *"Yes, and":* lean into critics and memes playfully; it converts negative energy into your energy.

### S-016 · Founder-POV + 4 elements applied to LinkedIn/X (cross-ref)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- See S-007, S-011, S-024. (Index pointer, no new content.)

### S-017 · Video-hook + CTA mass production and organic-ads rule (apps)
- **Source:** @maubaron · 2026-02-28 · https://x.com/maubaron/status/2027551137768083619
- **Access:** full text
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Automatable short-form formats for app installs.
- **How to use it:** Scraper collects viral video hooks (first 3s) → Python stitches hook + app CTA → bulk schedule (claim: 700 clips in 30 min). Other formats: UGC reaction + ≤8s demo; branded consistent slideshows; Jack Friks identity-label cards; memes + ManyChat. Paid ads only as "organic ads" (organic-looking hook + direct CTA) after organic winners exist.

## 3. Paid ads & creator programs

### S-018 · Performance-based creator program on Trybe (Wispr Flow)
- **Source:** @hectorserrranoo · 2026-10-08 · https://x.com/hectorserrranoo/status/2108260769603486100
- **Access:** full transcript (~15 min)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** How Wispr Flow launches 500–700 net-new UGC ads/month.
- **How to use it:** Start with a small hand-picked creator group, pay on performance with a guaranteed minimum, and scale the group in steps (details below).
- **Key details / steps:** Creators join group → make video → brand launches it (Meta, AppLovin, TikTok) → pay % of GMV (ecom) or % of ad spend (SaaS; Wispr = 7%). "Smart retainer": guaranteed minimum (e.g. $1,000 for 25 videos) topped up if commissions fall short; helps recruit before you have platform history. Start with 4–5 intent-picked creators filling ad-library gaps; recruit via IG keyword search + mining followers/likes, 100–200 DMs; scale 5→10→20→40, coast at 40–60; only ~5–7 of ~7,000 Trybe applicants accepted; $100 referral bonus for creators at/above level. Culture: creator coaches, Calendly access, weekly Thursday call with media buyer, giveaways (cash, camera gear, Meta glasses), retreat for top 6. Push new concepts: Meta clusters ~60%+ similar videos and suppresses reach.

### S-019 · Rev-share creators beat flat-fee UGC
- **Source:** @LukasPakter · 2026-07-07 · https://x.com/LukasPakter/status/2074374355572916425
- **Access:** full text
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Argument + numbers for commission-based creators.
- **How to use it:** Offer creators a % of revenue (Haus: 15% via jointrybe.com) instead of $200–300/video. Claims: $200k→$5M/month in a year, 4,000+ ads/month, CPA $89→$30, some creators earn $50k+/month.

### S-020 · Paid-ads program rebuild in 30 days
- **Source:** @hectorserrranoo · 2026-10-08 · https://x.com/hectorserrranoo/status/2108260769603486100
- **Access:** full transcript — same video as S-018 (the transcript content is the Trybe program; no separate 30-day calendar was stated).
- **Added by:** Grok Bot (initial import) · 2026-10-21

### S-021 · FaceTime-call ad format
- **Source:** @antonioventre_ · 2026-07-01 · https://x.com/antonioventre_/status/2072385506709512374
- **Access:** full text
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Pattern-break UGC format.
- **How to use it:** Record two people (real creators or AI) in a conversation styled as a screen-recorded FaceTime call; must look native, not polished.

### S-022 · LinkedIn ads for B2B pipeline
- **Source:** @googlewaqas · 2026-10-10 · https://x.com/googlewaqas/status/2108920397609472236
- **Access:** full text (post promises 15 steps; returned text covers ~12 and ends at retargeting)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **How to use it:** Account lists first, founder/customer-led native creative, angles not variants, engagement bidding, behavior-sequenced retargeting.

### S-075 · Scaling Meta ads isn't "duplicate + double budget"
- **Source:** @adamtaylorl · 2026-07-02 · https://x.com/adamtaylorl/status/2072667119536206067
- **Access:** title only (couldn't access) — the "how it actually works" part is an image/continuation not returned.
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does / How to use it:** Placeholder; see S-018 (new concepts beat near-duplicates — Meta clusters ~60%+ similar creatives).

## 4. Sales / GTM & outbound

### S-023 · Grok Bot GTM bot team (SpaceXAI)
- **Source:** @kristaletz · 2026-08-16 · https://x.com/kristaletz/status/2089103618121314689 (+ summary @aiedge_ https://x.com/aiedge_/status/2089405900394258879)
- **Access:** full text (article "Grok Bot for GTM"; routine screenshots not captured)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** A team of specialized bots for enterprise sales.
- **How to use it:** Connect your work tools, start with a pinned Chief-of-Staff bot, then add specialist bots one at a time (details below).
- **Key details / steps:** Connect Salesforce, Gmail, Calendar, Sheets, Drive, Slack, Notion, Granola, Figma, X, LinkedIn, warehouse; use mobile + voice. Bots: Chief of Staff (pinned; prep, inbox, post-call drafts, orchestrates/spins up others); daily meeting prep (short, phone-skimmable, can call slides bot); routines: inbox scan + auto-draft replies, follow-ups from Granola/Gong notes; Prospecting (pipeline plans, intent data, deep research incl. webinars/podcasts/posts, drafts in Gmail in your voice, runs overnight); Customer expert per strategic account (Slack, calls, weekly media rundown, feature requests, support tickets); Data analysis; Product expert ("Cursor 10x engineer" on codebase or Glean); 1:1 agent; Forecasting (updates Salesforce opp notes in your format); Slides (Figma brand system, master deck, translations; live slide update from Granola transcript — stop recording 5–10 min before end); Sales coach on Gong calls. Habits: demonstrate a task once and have it turn the recording into a skill; style profile from sent mail; anti-slop skill updated on every steer; parallel cloud agents; bots in group chats calling each other; periodic Chief-of-Staff audit to automate/prune.

### S-024 · Shared prospecting bot "PG by Krista"
- **Source:** @kristaletz · 2026-08-28 · https://x.com/kristaletz/status/2093378627932918087 → https://x.ai/bot/fcJJMM58AdXSTBdW3xWyW
- **Access:** full text (bot page)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Third-party bot: researches accounts, watches recent podcasts/webinars for personal hooks, can optionally sign into X/LinkedIn for recent posts, builds a contact spreadsheet, drafts outreach from CRM + meeting notes.
- **How to use it:** "Add to Grok Bot" (third-party; may act on your behalf — review permissions).

### S-025 · Intent-phrase LinkedIn prospecting
- **Source:** @fin465 · 2026-08-20 · https://x.com/fin465/status/2090272639839576492
- **Access:** full text
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Finds buyers who publicly declared intent.
- **How to use it:** Search LinkedIn posts for intent phrases: "anyone got recommendations for [tool]", "alternative to [competitor]", "looking for a good [software]", "got burned by [company], where do i go now", "has anyone used [company]". Filter for hours-old posts, also scrape likers, enrich verified email, 2-line email quoting their post, reply within 30 min. Mentions Origami AI for real-time LinkedIn keyword search.

### S-026 · Agent people-search / enrichment (treg.to)
- **Source:** @jasonzhou1993 · 2026-09-01 · https://x.com/jasonzhou1993/status/2094740336895840605
- **Access:** full text (treg.to page); video has no speech
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** One agent skill over 113 data providers; pay per answer.
- **How to use it:** Add the skill to an agent; ask in plain words (find marketing lead at X, verify email). Prices from page: email find from $0.0089, verify $0.003/check, person enrich from $0.028, company enrich from $0.010; misses free. Receipt: 27 people → 20 verified emails for $0.58. Bench claim: 43% → 78.2%.

## 5. SEO / AEO (AI search)

### S-027 · 11 optimizations to be recommended by Meta Muse & AI agents
- **Source:** @RobHoffman_ · 2026-10-19 · https://x.com/RobHoffman_/status/2112212215583658420
- **Access:** full text
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **How to use it:** Audit your site against the 11 points (accessibility tree, raw-HTML facts, question-H2 + ≤100-word "it depends" answer, definitions over slogans, text testimonials, "as of" dates, robots.txt `meta-webindexer`, broken links, semantic HTML, 30–90-day refresh with published/updated dates).

### S-028 · Railway's AI-recommendation growth playbook
- **Source:** @irabukht · 2026-10-14 · https://x.com/irabukht/status/2110189752666440181
- **Access:** full text (the "full guide in first comment" was not retrieved)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** 13 tactics behind a claimed $20M→~$100M ARR.
- **Key details / steps:** Claude Code picks Railway for 82% of Python apps (Vercel wins Next.js/React); GTM team works on getting models to recommend them; 6,653 how-to pages for self-hostable tools; 127 framework deploy guides; comparison + migration page per competitor; one file listing 414 help pages with summaries + plain-text versions; agent docs + one-step install; ChatGPT/Claude Code plugins; `ssh railway new` no-signup server; weekly changelog since 2021 (312 pages); team of 7.

### S-029 · Check AI attribution of customers
- **Source:** @iamshackelford · 2026-07-29 · https://x.com/iamshackelford/status/2082515673293705685
- **Access:** post text only (thread continuation not returned by search)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **How to use it:** Ask last 10 customers where they first heard of you; if several say ChatGPT, prioritize AEO. Claim: 63% of Americans used AI for shopping in last 6 months; #1 use is research/compare.

### S-073 · 42 startup backlink / launch directories
- **Source:** @hridoyreh · 2026-04-01 · https://x.com/hridoyreh/status/2039297374078869617
- **Access:** full text
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Directory list for backlinks + discovery (also feeds AI-search citations).
- **How to use it:** Work through the list — Indie Hackers, Hacker News, Product Hunt, BetaList, AlternativeTo, SaaSHub, DevHunt, Medium, Substack, Reddit, Software Advice, Quora, TrustMRR, TinyLaunch, Startup Stash, Capterra, G2, GetApp, Futurepedia, StackShare, Clutch, Chrome Web Store, Microlaunch, StartupBase and more (42 total). Prioritize those matching your category; reuse one canonical description.

## 6. Automation & AI agents (incl. Grok Bot)

### S-030 · 10 Grok Bot content bots
- **Source:** @ryangrowthh · 2026-10-21 · https://x.com/ryangrowthh/status/2112816157682204822
- **Access:** full text
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Bot roster for an X creator.
- **How to use it:** X Researcher (overnight outlier scan → morning report); Chief of Staff (MCP connections, routines); X Article Tracker (text ideas to bot); Analytics Coach (daily impressions + replies report); Competitor Watch (X lists); Bookmarks Brain (logs bookmarks, daily resurfacing + summaries of long-form); Quote Post Scout; Fact Checker; Sparring Bot; Banner/Visual Prompter. Idea: sponsor/paid-promo hunter bot.

### S-031 · Daily `what_the_market_is_telling_us.md`
- **Source:** @gregisenberg · 2026-08-02 · https://x.com/gregisenberg/status/2083954605533065561
- **Access:** full text
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **How to use it:** Morning agent pulls Stripe (pay/upgrade/downgrade/churn), PostHog (behavior), Intercom/Plain (tickets), Granola/Meet (calls), HubSpot/Salesforce (lost reasons), Linear/Jira/GitHub (bugs/requests), Ideabrowser MCP (outside signal). Output = what CHANGED this week + receipts + the product/GTM decision it affects (e.g. churned customers mention setup confusion & never invited a teammate → activation, not pricing).

### S-032 · Claude Code as a video editor (Fable launch video)
- **Source:** @trq212 · 2026-06-10 · https://x.com/trq212/status/2064826394589442448
- **Access:** full transcript (screen recording — visual review recommended)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Agent-driven post-production with no video editor.
- **How to use it:** Give the agent the folder of takes + prompt: transcribe every recording, stitch best takes into one clip (best takes are usually the last ones with fewest errors). Agent: Whisper transcripts per take → dedupe → per-scene edit JSON (candidate takes, reasons, start/end) → ffmpeg first cut → writes color-grading LUT/configs (from neutral Rec.709) → React components in Remotion timed to transcript beats → export designs to Figma for design team → "design updated in Figma, re-render" → final render via npx. 17 takes / 25 GB input.

### S-033 · GPT-6 Astra + Higgsfield MCP: full tutorial video in one chat
- **Source:** @adilinthewild · 2026-09-06 · https://x.com/adilinthewild/status/2096501790774817240
- **Access:** full transcript
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Assistant coordinates generation (talking head from a short clip of you), motion assets, assembly.
- **How to use it:** Inputs: short clip of you, After Effects project, render of motion graphics, style-reference video. Connect Higgsfield (plugin in ChatGPT or MCP server); test with one short sample first. Prompt structure: finished result → each input file + role → style + save location → ask for editable projects. Verify technical claims against docs before narration. Script around viewer outcome; split into short takes ending on sentence boundaries; measure actual durations. Presenter prompts in two sections (look/sound vs exact words), no music/graphics baked in; check face/voice/lip-sync consistency and dropped words. Use real interface captures, not generated screenshots. Assemble in DaVinci Resolve: story pass first, then demos/graphics, match dialogue levels across cuts; keep project portable; full watch-through before export.

### S-034 · Paperclip: run agents as a company
- **Source:** @NickSpisak_ · 2026-03-16 · https://x.com/NickSpisak_/status/2033518072724705437 (+ repo github.com/paperclipai/paperclip)
- **Access:** full text (article) + repo summary via search
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Self-hosted control plane: org chart, goal→project→task alignment, heartbeats (scheduled wakeups), per-agent monthly budgets that hard-stop, tickets with traced tool calls, multi-company, board-style approvals; adapters for Claude Code, Codex, Cursor, OpenClaw, Bash, HTTP.
- **How to use it:** `npx paperclipai onboard --yes` (Node 24.11+) → dashboard localhost:3100 → create company + mission → hire CEO agent → approve suggested hires + budgets.

### S-035 · OpenClaw + Claude + Codex trading-bot architecture (pattern only)
- **Source:** @zostaff · 2026-03-17 · https://x.com/zostaff/status/2033930728044372275
- **Access:** full text (code images not captured)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** "One thinks, one builds, one runs" agent pattern.
- **How to use it (pattern):** Strategist LLM returns probability + recommendation + confidence; coder agent writes/patches code with tests; orchestrator (persistent memory, cron, modular skills = folder with SKILL.md + scripts, Telegram remote) runs every 5 min and logs. Self-repair loop: metric drop → task → coder patches → tests → deploy. Treat profit claims as unverified.

### S-036 · Agent memory as a filesystem (OpenViking L0/L1/L2)
- **Source:** @slash1sol · 2026-03-15 · https://x.com/slash1sol/status/2033195648565104975
- **Access:** post text only (repo github.com/volcengine/OpenViking not opened; video has no speech)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Hierarchical memory: viking://user/memories, viking://agent/skills; L0 ~100-token summary, L1 overview, L2 full detail opened on demand.
- **How to use it:** Apply the 3-tier summary pattern to your own agent notes/skills to save tokens. MiroFish/trading claims = hype.

### S-037 · Claude as a runtime paired with repos (Anthropic cookbook)
- **Source:** @LunarResearcher · 2026-04-12 · https://x.com/LunarResearcher/status/2043330919868621142
- **Access:** post text (story is promotional; link resolves to github.com/anthropics/anthropic-cookbook)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **How to use it:** Learn agent patterns (tool use, evals, citations) from the cookbook and connect agents to codebases/data rather than chatting. Ignore the trading P&L/copytrade pitch.

### S-038 · Self-hosted mail for agents (OpenShip)
- **Source:** @openshipio · 2026-07-18 · https://x.com/openshipio/status/2078314296610632141
- **Access:** post + docs (search)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **How to use it:** Self-host deploy platform with Postfix/Dovecot mail, DKIM/SPF/DMARC; relay outbound via SES/SMTP for deliverability (docs say fresh VPS IPs are often blocklisted/port 25 blocked). See tools.md.

### S-039 · Graph engineering for reliable agents (LangGraph workshop)
- **Source:** @0xCodez · 2026-07-25 · https://x.com/0xCodez/status/2081017726261199185
- **Access:** full transcript (2h21m). Note: the post calls it an Anthropic workshop; the speaker in the audio presents LangChain's LangGraph/LangSmith and refers to "the LangChain team" (appears to be an AI Engineer conference workshop). Slides/notebooks not captured — visual review helps.
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Explains chains vs agents and how to get production-grade reliability.
- **How to use it:** Design agents as explicit graphs; evaluate answers AND tool trajectories; build a data flywheel.
- **Key details / steps:**
  - Chain = developer-defined control flow (reliable, rigid). Agent = LLM-decided control flow. Tool calling is just the LLM emitting a structured payload (tool name + args); ReAct = act → observe → loop until a plain-text answer. ReAct is flexible but unreliable (wrong tool, wrong args), worse with many tools and long dialogs.
  - Middle ground = graph: fixed steps where you know them, LLM decisions only at specific edges. State = short-term memory (a dict: question, documents, flags, steps); nodes read/modify state; edges route. Set a recursion limit for cycles.
  - Patterns: corrective RAG (grade retrieved docs; if irrelevant, add web search), self-RAG (check answer vs docs for hallucination + answer relevance), adaptive RAG (route question to index or web first), AlphaCodium-style code generation (run unit tests, feed errors back). Cheap inline unit tests fix hallucinated imports; also validate structured-output schemas in-app.
  - Explicit router node at graph start beats letting ReAct choose among tools; pass history into the router to decide whether to re-retrieve.
  - Three feedback loops: in-app self-correction; pre-production evals; production monitoring. Eval = dataset + app + evaluator (LLM-as-judge vs reference, or custom heuristics). Evaluate both final answer and tool-call trajectory (speaker's 5-question eval: local Llama-3 8B graph agent had perfect trajectory; a GPT-4o ReAct agent got good answers via odd trajectories).
  - Reference-free RAG checks for production: retrieval relevance, answer relevance, hallucination vs docs. Use fast small models (or fine-tuned classifiers, or fast inference like Groq) for in-loop yes/no grading; avoid 0–5 scales.
  - Bootstrap evals: LLM-generate Q/A pairs per document then audit; flag bad production cases with online evaluators, fix, add to the test set (Karpathy "data engine" flywheel).
  - Many tools: selection degrades even around 5; embed verbose tool descriptions and use semantic search to choose tools, or split into sub-agents/graph nodes.
  - RAG chunking: index small chunks but pass full parent documents to the LLM. Long-context caution: in his multi-needle test (120k tokens, 10 needles) retrieval fell to ~60%, worse for facts near the start; don't trust "stuff everything".
  - Text-to-SQL: always LIMIT results; add a query-check node before execution. Human-in-the-loop via LangGraph checkpoints.
  - "The model is not the moat; the system around it (orchestration, evals, guardrails, data flywheel) is." 

## 7. Research & market intelligence

### S-040 · Ecom ad/shop intelligence inside your LLM (TrendTrack MCP)
- **Source:** @Trendtrack_io · 2026-07-13 · https://x.com/Trendtrack_io/status/2076692456037343413
- **Access:** post + docs (search); video transcript is promo only
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **How to use it:** Add custom connector `https://api.trendtrack.io/v1/mcp` (OAuth); ask "what's scaling in [niche] this week?"; call check_credits first (1 credit/row; 10k/mo; $1 per 1k top-up).

### S-041 · AI UGC research (LightReel)
- **Source:** @Jibran_05 · 2026-03-16 · https://x.com/Jibran_05/status/2033589137018917027
- **Access:** post + pricing page
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **How to use it:** Ask competitor hooks, why a video flopped, creators by niche/city/follower range; $199/mo, 3-day trial.

### S-042 · Pre-test launches on simulated follower niches (Signal)
- **Source:** @jasonlai150_ · 2026-08-13 · https://x.com/jasonlai150_/status/2088022974788247646
- **Access:** product page
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **How to use it:** Cluster your X followers into niches → Grok drafts post/poster per niche → A/B on simulated agents → ship winner → export niche as Ads custom audience.

### S-043 · Predict video engagement with Meta TRIBE v2
- **Source:** @fuckgrowth · 2026-04-07 · https://x.com/fuckgrowth/status/2041580077826371733
- **Access:** full text (article "how to predict v*rality")
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** Open model predicting fMRI brain response (~70k points) to video/audio/text; trained on 1,000+ hours fMRI from 720 people.
- **How to use it:** Meta's Colab (Runtime → T4 GPU) → pip cell → restart → HF read token as HF_TOKEN secret → request Llama access (≈1h) → run on your drafts; move high-engagement moments earlier, cut flatlines; have an agent rank N variants. Links: huggingface.co/facebook/tribev2, aidemos.atmeta.com/tribev2. Claim: re-edit → 221k views (single anecdote).

## 8. Coding & building

### S-044 · AI engineer roadmap (12 months, no degree)
- **Source:** @eng_khairallah1 · 2026-06-23 · https://x.com/eng_khairallah1/status/2069341916798369801
- **Access:** full text
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **Key details / steps:** M1–3 Python + Git (5 tiny programs on GitHub); M3–5 LLM API: streaming, history, output format, rate limits, tool use; M5–7 RAG: chunking, embeddings, vector DB, retrieval evaluation, deploy; M7–9 agents: multi-tool loop, multi-agent check, explicit failure handling; M9–11 evals + deployment/monitoring/cost tracking; M11–12 case studies, build in public, apply (often AI-augmented SWE first).

### S-045 · Shopify AI Toolkit for coding agents
- **Source:** @Shopify · 2026-04-09 · https://x.com/Shopify/status/2042335629640355843
- **Access:** full text (shopify.dev docs)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **How to use it:** `claude plugin install shopify-ai-toolkit@claude-plugins-official` (or `npx skills add Shopify/shopify-ai-toolkit`, or Dev MCP `npx -y @shopify/dev-mcp@latest`); gives docs/schema lookup, GraphQL/Liquid/extension validation, store tasks via Shopify CLI.

### S-046 · Open models as cheap classifiers (Simple Jev)
- **Source:** @picocreator · 2026-09-18 · https://x.com/picocreator/status/2101006253829046539
- **Access:** full text (simplejev.ai)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **How to use it:** POST context + questions (choice/score) → JSON with choice, confidence, probabilities (reads next-token logits). Demo API needs no key (2k ctx, 2 RPS); ~$0.03/M input tokens on Featherless.

### S-047 · Scraping & marketing skill libraries
- **Source:** @gil906 https://x.com/gil906/status/2029307713306673653 (Scrapling) · @ihteshamali https://x.com/ihteshamali/status/2039342092124897568 (ericosiu/ai-marketing-skills)
- **Access:** repo descriptions only
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **How to use it:** Scrapling — Python framework from single request to full crawl; ai-marketing-skills — open-source skills for growth experiments, pipeline, content ops, outbound, SEO, finance. Mine for agent skills.

## 9. Design / creative (web, image, video)

### S-048 · $10k-look animated site in Claude Code
- **Source:** @monokern · 2026-06-28 · https://x.com/monokern/status/2071246711222055363
- **Access:** full text (build prompt was an image, not captured)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **Key details / steps:** Install skills: Anthropic frontend-design (github.com/anthropics/skills/tree/main/frontend-design) and UI/UX Pro Max (npm, github.com/nextlevelbuilder/ui-ux-pro-max); Auto mode. Collect section-by-section reference screenshots (Awwwards, Pinterest) into /reference. Start prompt with /ui-ux-pro-max and end by asking Claude to ask 4–6 questions first. Hero idea: cursor "flashlight" mask revealing a warm-lit photo (radius 100–150px, feathered). Review pass: list all issues, send in one message. Polish pass rubric: typography (no Inter), restrained palette, hierarchy, intentional animation, real mobile design, specific copy.

### S-049 · Scroll-scrubbed video websites (motionsites method)
- **Source:** @mikenevermiss · 2026-07-13 · https://x.com/mikenevermiss/status/2076603705323892815 (+ prompts https://x.com/mikenevermiss/status/2076609167406632974)
- **Access:** full transcript (design walkthrough — visual review recommended)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **Key details / steps:** Screenshot a reference → image model (GPT Image) recreates with your subject, then a text-free version → animate in Seedance via Higgsfield with "animate the image the same way as the attached video" (match duration, 1080p 16:9) → Claude Code session in empty folder: hero 500vh for scroll scrubbing, borrow a font/layout prompt from motionsites.ai, swap font (Helvetica Neue), add a smooth-scrub snippet for cross-browser playback, move content to bottom; product grid section (100vh, 33vw cards, ~280px image, 18px name, 16px price); after horizontal scroll, a centered div expands to full width revealing a second scrubbed video.

### S-050 · ChatGPT Images 2.5 — prompt-as-visual-decisions workflow
- **Source:** @Av1dlive · 2026-09-10 · https://x.com/Av1dlive/status/2098055179761525165
- **Access:** full text (example prompts were embedded images, not captured)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **Key details / steps:** Brief order: purpose → canvas → contents (exact words) → relationships → appearance → checks. Bind attributes to objects ("oxblood bag beside a cream cardholder"). Organize complex scenes by depth/panel/dominant subject. Write reading order/screen roles before decoration. Translate "premium" into visible materials/light. Reconstruct references as an inventory (canvas → groups → objects → parts → properties; separate visible/inferred/unknown) saved as JSON; give each reference a role (identity/layout/finish) and what to ignore; edit with change → preserve → allow; one change at a time, return to best accepted source; verify things that can fail (e.g. chart bar lengths — render real charts from data); sub-agents for controlled alternatives with fixed budget and shared checklist.

### S-051 · 12 camera moves for AI video prompts
- **Source:** @beginnersblog1 · 2026-06-28 · https://x.com/beginnersblog1/status/2071124287109661170
- **Access:** full text
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **Key details / steps:** Push-in, pull-back, pan, tilt, tracking, arc/orbit (<30°), crane/jib, zoom, dolly zoom, whip pan/crash zoom, handheld (add "subtle"), static angles (low=power, Dutch=unease, bird's-eye=scale). One move per clip; add "slow" to hide artifacts.

### S-052 · Timed shot-list prompts for Seedance 2.0
- **Source:** @Naiknelofar788 https://x.com/Naiknelofar788/status/2071174186978951379 · @john_my07 https://x.com/john_my07/status/2071977017474789557
- **Access:** full text (prompts); videos have no speech
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **How to use it:** Structure: Scene / Subject (@img reference, consistency clause) / Action timeline in second ranges / Camera / Audio / Style (+ Goal). Examples: 15s one-take space→café with speed ramping; early-2000s DV camcorder realism with autofocus hunting, exposure pumping, no music.

### S-053 · Seedance 2.0 course
- **Source:** @EXM7777 · 2026-04-14 · https://x.com/EXM7777/status/2044081887615103097
- **Access:** title only (couldn't access) — linked course is in a quoted post/video with no speech.
- **Added by:** Grok Bot (initial import) · 2026-10-21

### S-054 · Google Stitch design agent
- **Source:** @stitchbygoogle · 2026-03-18 · https://x.com/stitchbygoogle/status/2034332847893574080
- **Access:** post + video transcript (demo — visual review recommended)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **How to use it:** Describe a page (palette, vibe) → pick from generated visual directions → swap images by voice/chat → apply design system to whole site; features: AI canvas, design agent, voice, instant prototypes, DESIGN.md.

### S-055 · Restyle/recreate competitor ad angles (free method)
- **Source:** @OriSilver · 2026-06-26 · https://x.com/OriSilver/status/2070503656881860698
- **Access:** post text only — demo video has no speech (visual review needed); method not described in text.
- **Added by:** Grok Bot (initial import) · 2026-10-21

### S-056 · URL → many promo videos (Fastlane)
- **Source:** @gauravsbuilding · 2026-06-18 · https://x.com/gauravsbuilding/status/2067501867198996528
- **Access:** post + search
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **How to use it:** Enter website → generated shorts → swipe-review → schedule. See tools.md for pricing.

### S-057 · Site "slurp" → marketing engine (Ploy)
- **Source:** @bryantchou · 2026-06-17 · https://x.com/bryantchou/status/2067249680334131325
- **Access:** full text (ploy.ai)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **How to use it:** Paste URL (free tier) → Ploy ingests site in ~60s → run PloyBooks (AEO comparison pages, competitor alternatives, programmatic SEO, visitor-ICP outreach drafts, AI agent readiness audit, WebMCP).

## 10. Ecom & conversion (CRO)

### S-058 · 16 PDP sections for supplement brands
- **Source:** @jordanhill11 · 2026-05-28 · https://x.com/jordanhill11/status/2059969743688270072
- **Access:** full text
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **How to use it:** Audit a product page against the 16 sections; each one answers a buyer barrier (scam skepticism, ingredient transparency, outcome uncertainty, timeline, financial risk, social proof, competitor comparison).
- **Key details / steps:** Origin story · results timeline (week 1/4/8) · expert grid · third-party certifications · clinical stats · athlete/celebrity proof · objection accordion · press strip · real customer videos · competitor/cost comparison table · benefit tabs · reviews filterable by goal · ingredient + dose breakdown · product carousel · guarantee badge · video FAQ / founder Q&A.

### S-059 · Research-first landing pages with Claude Design/Cowork/Code
- **Source:** @eCom_Amin · 2026-04-21 · https://x.com/eCom_Amin/status/2046584225898627511
- **Access:** full text
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **Key details / steps:** Page-type decision tree by category/awareness; research prompts (winning offers, angles, funnel types, objections from reviews/Reddit); reverse-engineer a leader's funnel (AG1 sells a free guide → email → product); Design for structure (advertorial 8-part, 5-question quiz with results page, honest comparison page), Code for polish/deploy/analytics/Klaviyo flows/Calendly/checkout + cart abandonment + upsell; day-2 $200–500 test. Claimed results (quiz 11.8–12.4%, advertorial funnel 8.7%) are anecdotal.

### S-060 · Landing-page test takeaways
- **Source:** @dave_stickland · 2026-09-17 · https://x.com/dave_stickland/status/2100594324089995624
- **Access:** full text
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **Key details / steps:** 50% never pass section 2; top click is Shop; best revenue = PDP-style buy block above the fold above the listicle; video + social proof hold attention; nobody clicks "Learn more"; GIFs > static images.

### S-061 · TikTok Shop team structure & Amazon ad-payment cash-flow lesson
- **Source:** @jordantwestecom https://x.com/jordantwestecom/status/2044485809924149255 · @MbtHawk https://x.com/MbtHawk/status/2041974437088514365
- **Access:** full text
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **Key details / steps:** TikTok Shop needs store mgmt (1–2), product mgmt (1–2), creator/affiliate (1–2), content+live (1–2), ads (1). Amazon (from Apr 15, 2026, passed) deducts ad spend from payouts → lost ~60-day card float; model cash flow without float, bridge with credit line, check Pay by Invoice, front-load inventory.

## 11. Founder, strategy & fundraising

### S-062 · Start a company from zero (Wispr Flow CEO Tanay Kothari)
- **Source:** @tankots · 2026-09-30 · https://x.com/tankots/status/2105358597333131400
- **Access:** full transcript (~30 min; auto-transcript has noise)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **Key details / steps:** Order: 1) self-reflection — what you've cared about for years (not what's exciting), what you want, your spike; "most startups die because founders lose the will to fight"; 2) co-founder — same cares, same values (theirs: integrity, customer-first, no selling data), complementary traits; they spent 3 months aligning before starting; 3) marry a problem/customer, not an idea; build fast, yes/no "does it solve the problem", be willing to kill ideas (Wispr Flow was product #8); get 100 people who love it; 4) capital — venture compresses 10 years into 1 with matching expectations vs a traditional business; seed dilution aim ~10% (norm 20–25%); VCs invest in you and your story; reference-check VCs (integrity, will they have your back, will you learn); 5) PMF — if you have to ask, you don't; iterate between idea and PMF. Final lesson: perseverance.

### S-063 · Hormozi 1-1 coaching: scaling a community/education business
- **Source:** @theharut · 2026-03-16 · https://x.com/theharut/status/2033435006354493577
- **Access:** full transcript (~9.5 min; auto-transcript noisy)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **Key details / steps:** Don't risk the base (existing customers' word of mouth is the main asset); hire someone to do promotion full-time — 2 hrs/week of your management for 40 hrs of promotion is a good trade; consider affiliates; renewals compound growth without more sales; three levers: raise price (lowest operational drag), increase volume, hire others to deliver; keep top performers in the main community if they're engaged because they drive upsells.

### S-064 · Seed market split: raise for the game you're in
- **Source:** @jnpayne · 2026-05-30 · https://x.com/jnpayne/status/2060742335390962162
- **Access:** full text
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **Key details / steps:** For consumer/commerce founders: ignore the AI seed narrative ($10M at $40–45M post), raise as little as needed for proof of concept, pick VC or seed-strapping (not in between), position on capital efficiency, target funds not chasing AI (e.g. OpenSky).

### S-065 · Non-dilutive R&D funding (NSF SBIR/STTR)
- **Source:** @kseniam0s · 2026-10-06 · https://x.com/kseniam0s/status/2107498859341439133 (+ seedfund.nsf.gov)
- **Access:** full text
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **Key details / steps:** Phase I up to $305K, Phase II up to $1.25M, Fast-Track up to $1.55M (post); site says up to $2M, zero equity. Eligibility: US startup ≤500 employees, ≥51% US citizen/PR owned, not majority VC-owned, work in US. Process: 3-page Project Pitch → invitation → full proposal (next deadline Nov 4 per post). NSF funds deep tech based on fundamental science/engineering; Phase I success ~10–20%.

### S-066 · Business-credit "second file" (financial tactic, verify independently)
- **Source:** @hxxntrr · 2026-10-17 · https://x.com/hxxntrr/status/2111517635259326649
- **Access:** full text (ends in a sales pitch)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **Key details / steps:** Separate personal (SSN) and business (EIN) credit; business cards at 0% APR for 12–18 months that report to business bureaus rather than personal; keep personal utilization low. Treat as a talk-to-your-CPA topic, not advice.

## 12. Quant / prediction-market methods (educational)

### S-067 · Five probability formulas (EV, Bayes, Kelly, base rate, KL)
- **Source:** @hanakoxbt · 2026-03-16 · https://x.com/hanakoxbt/status/2033566488641089750
- **Access:** full text (code images not captured)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **Key details / steps:** EV = Σ pᵢxᵢ (enter only +EV); Bayes P(H|E)=P(E|H)P(H)/P(E) for proportional updates; Kelly f* = (p·b − q)/b, use ¼–½ Kelly; base rate P(A|signal)=TP/(TP+FP); KL divergence between related markets to spot mispricing. Useful as general decision-making math.

### S-068 · LMSR, Bregman projection & risk rules
- **Source:** @0xRicker · 2026-03-14 · https://x.com/0xRicker/status/2032798292128522327
- **Access:** full text
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **Key details / steps:** LMSR price_i = e^{q_i/b}/Σe^{q_j/b} (small b = bigger price impact); EV gap entry if >0.05 after fees; KL threshold; Bregman projection for multi-outcome arbitrage; walk-forward backtests, fractional Kelly, 20% drawdown stop, fees 1–2% erode small edges. Profit claims unverified; gambling/financial risk.

## 13. AI/ML understanding & mental models

### S-069 · Why bigger neural nets generalize (double descent + lottery tickets)
- **Source:** @_yusufknl · 2026-09-12 · https://x.com/_yusufknl/status/2098724555963425208
- **Access:** full transcript (~18 min)
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **Key details / steps:** Classical theory predicts overfitting past capacity; 2019 double-descent result: test error falls again past the interpolation point. Lottery Ticket Hypothesis: iterative magnitude pruning (remove 10% smallest weights, reset survivors to original init, retrain, ~30 rounds) finds a ~4% subnetwork matching full accuracy; larger nets = more "tickets", so smaller winning subnetworks → simpler models (Occam's razor). Narrator's view: scaling alone may be too slow for human-level AI, but next-word prediction with better learners could get there.

### S-070 · Context graphs as organizational memory
- **Source:** @akoratana · 2026-04-01 · https://x.com/akoratana/status/2039381472826827012
- **Access:** full text
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **Key details / steps:** Coordination cost grows superlinearly with headcount; hierarchy = lossy compression of information; a context graph stores decision traces (why things became true), not just data — the shift from "agent memory" to "organizational judgment".

### S-071 · Force-first design (Gaudí method)
- **Source:** @anishmoonka · 2026-06-14 · https://x.com/anishmoonka/status/2066115917235519614
- **Access:** full text
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **Key details / steps:** 1) find the forces before the form; 2) build a cheap model and let it compute (hanging-chain catenary models); 3) copy nature's solutions (tree-like branching columns on lines of thrust); 4) make complex from simple repeatable parts (ruled surfaces from straight lines); 5) make the constraint do the work. Also: parametric (rule-based) design.

### S-072 · Peptides: how to think about them (Huberman × Dr. Abud Bakri)
- **Source:** @hubermanlab · 2026-06-01 · https://x.com/hubermanlab/status/2061447675724091690 (+ @peptidedaily_ summary clip https://x.com/peptidedaily_/status/2064346484905312753)
- **Access:** full transcript (~2.8 h incl. ads). Medical/personal content — informational only, not advice; anecdotes are the speakers' own.
- **Added by:** Grok Bot (initial import) · 2026-10-21
- **What it does:** A framework for evaluating peptide claims and sourcing risk.
- **Key details / steps:**
  - Categorize: peptides with known receptors and strong clinical effects (GLP-1s) vs no clear receptor (BPC-157, TB-500/TB4; Russian "bioregulators" like EDR/"pinealon", epitalon described as epigenetic/DNA-groove binders).
  - BPC-157: from Croatian gastric-juice research (one group produced almost all animal data); animal wound/tendon healing; angiogenesis (VEGF) raises theoretical tumor concern — no animal cancer signal reported; LD50 unknown; phase 1/2 rectal enema trials for ulcerative colitis (abstracts only). Regulatory: moved to FDA compounding Category 2 in late 2024; compounders sell "PDA" (pentadecapeptide arginate); state medical boards vary.
  - Sourcing tiers: pharma (most stringent) > compounding pharmacies (variable quality) > "research use only" gray market (unknown) > black market. Guest says API for nearly all peptides is made in China. Ask your prescriber what the pharmacy charges vs what they charge.
  - Thymus: shrinks after puberty; thymosin alpha-1, thymulin (zinc-dependent — low zinc status lowers it), TRIM trial (growth hormone + metformin + DHEA regrew thymus on imaging). Cheap marker the guest highlights: lymphocyte-to-monocyte ratio on a standard CBC with differential.
  - GH secretagogues (tesamorelin, ipamorelin, MK-677) reduce insulin sensitivity; the "trinity stack" (GLP-1 + GH/GHRH + androgen therapy) is described as a celebrity protocol with unknown health effects.
  - GLP-1s: start low (0.25 mg) and titrate; pair with lifestyle changes ("training wheels"); watch electrolytes/food intake; retatrutide also hits GIP and glucagon.
  - Guest's guidance: get peptides through a physician who monitors you (e.g. IGF-1 for GH secretagogues); fundamentals (sleep, light, diet) first. GHK-Cu topical has human aesthetic data, especially with red light (sunlight noted as a free source).

---
## Appended entries (future runs add new entries below, newest last, then add them to the Index)
