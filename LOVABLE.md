# Lovable demo: prompt and content

How to use: create a new Lovable project, attach three photos from `public/assets/img/`
(`portrait.jpg`, `portrait-standing.jpg`, `walking-bw.jpg`), and paste everything below the line
as the first prompt. If Lovable shortens copy, paste the page's section again and say
"use this copy verbatim".

---

Build a four-page personal portfolio site for Felix Hofmann, a Principal Product Manager in Berlin.
React + Vite + Tailwind with React Router. Pages: `/`, `/about`, `/contact`, and case studies at
`/work/douglas`, `/work/wiwin`, `/work/trusted-shops`, `/work/redline`. Also add `/impressum`.

## Design direction (follow strictly)

Editorial, like a well-set magazine or annual report. It must NOT look like a SaaS landing page or
an AI-generated template.

- No gradients, glassmorphism, drop shadows, rounded cards, emoji, icons in circles, or animated
  counters. No hero background image. No scroll animations besides plain hover states.
- Structure comes from typography and thin horizontal rules (1px), not boxes. Section headers sit
  under a full-width 1px dark rule with a small uppercase label on the left (3/12 columns) and a
  serif heading on the right (9/12 columns).
- Colors: paper background `#F4F2ED`, darker paper `#E9E5DC`, ink `#14171C`, soft ink `#3F4650`,
  muted `#6A7079`, rules `#CDC8BD`, one accent navy `#1D3654` used sparingly: the italic words in
  the hero, list markers, one full-bleed navy band for the energy section.
- Fonts from Google Fonts: **Newsreader** (serif, weights 350–500, with italic) for headings and
  body text; **IBM Plex Sans** (400/500) for labels, nav, tables and small UI text; **IBM Plex
  Mono** (400) for dates and index numbers.
- Big numbers are Newsreader at weight 350, tight letter-spacing (-0.03em), about 60px on desktop.
- Labels: Plex Sans 12px, uppercase, letter-spacing 0.09em, muted color.
- Body text 19px, line-height 1.6, max width about 36em. Headings use text-wrap: balance.
- Max content width 1200px with generous side padding. Everything stacks to one column below 760px.
- Photos are sharp rectangles (no rounding), portrait aspect ratio.
- Masthead: name "Felix Hofmann" in serif on the left, nav (Work, About, Contact) in Plex Sans on
  the right, one dark 1px rule underneath. Footer: dark 1px rule on top, one line of text, links
  to email, LinkedIn, Impressum.

## Home `/`

**Hero** (7/12 text, 5/12 photo `portrait.jpg`)
- Label: PRINCIPAL PRODUCT MANAGER · BERLIN
- H1: "I get to the bottom of complicated systems, then build them and *explain them plainly.*"
  (the last three words in navy italic)
- Lede: "Twenty years of product management on consumer apps, e-commerce and regulated platforms, for
  Douglas, ON, Eurowings, Trusted Shops and A1 Telekom. Today I'm Principal Product Owner at
  Sonova. On the side I'm building an AI product where every answer has to show its source."
- Buttons: dark square button "Read the case studies" (scrolls to #work), underlined text link
  "Get in touch".

**Facts strip** (three columns separated by thin vertical rules)
- NOW: Principal Product Owner, Sonova
- BEFORE: Trusted Shops, ON, Douglas, Eurowings, IONOS
- LOOKING FOR: Senior and principal product roles in applied AI and the energy transition

**IN NUMBERS: "What the work added up to."** 3×2 grid, each item: big number, sentence, mono source.
- €1B+ · Annual revenue running through the Douglas iOS and Android apps I owned · Douglas · 2020–21
- 0 · Minutes of downtime while those apps moved to a new SAP Hybris backend · Douglas · 2020–21
- +50% · Conversion on a BaFin-regulated investment platform, after lab usability testing · WIWIN · 2022–23
- #1 · App Store ranking for brand keywords in 10 markets, rating held at 4.7 through a rebrand · Trusted Shops · 2025–26
- 250k · Users within weeks of launching a secure messenger on iOS and Android · IONOS · 2016–17
- 1M · Users on a bootstrapped dating app I co-founded, with a #1 Google ranking · M47 Interactive · 2009–15

**SELECTED WORK: "Four case studies, each a different kind of hard."** A ruled list, each row links to
the case study: mono index | small uppercase client + large serif title | serif result + sans detail.
- 01 · DOUGLAS · RETAIL APPS · Moving a billion-euro app business onto a new backend without a minute of downtime · **0 downtime** · 4 Scrum teams, 40+ people, millions of customers
- 02 · WIWIN · REGULATED FINTECH · Making a BaFin-regulated investment flow feel safe enough to finish · **+50% conversion** · KYC, payment and tokenization in one journey
- 03 · TRUSTED SHOPS · CONSUMER APPS · Growing a consumer app through 30,000 partner shops · **+27% sign-ups** · #1 for brand keywords in 10 App Store markets
- 04 · REDLINE · OWN AI PRODUCT, IN BUILD · An AI contract reader that has to prove every claim it makes · **100% cited** · Every risk flag quotes its source sentence, checked in CI

**ON AI: "I'd rather show you than claim it."** Two columns.
Left: "Most of my career came before large language models, and I haven't yet shipped an AI feature
to paying users. I'd rather you read that here than work it out from my CV." / "So I'm learning AI
the way I learned every domain before it, from BaFin rules to the financing rules for solar modules:
by going deep enough to build the thing myself, and writing down what I don't know yet."
Right, a ruled list:
- **Redline, an AI contract reader.** I wrote the research, the PRD and ten architecture decisions. Coding agents built the tickets against them. The build gate: every risk flag must quote a real sentence from the document, verified in CI. → Read the case study
- **Automation in daily product work.** n8n workflows and Claude tooling at Trusted Shops, alongside owning the apps and the web portal.
- **An agent workspace for my own job search.** I run my search on a Claude Code workspace and have extended it with research on about a hundred target companies. Building on it is how I learn where agents help and where they quietly make things up.

**Full-bleed navy band. BEFORE APPS: SOLAR: "Energy isn't a new interest for me."**
"From 2008 to 2012 I ran two companies importing photovoltaic modules from China by the container,
selling direct to installers and EPCs in Germany and Italy. German banks wouldn't finance
installations with unknown module brands, so I set up the reference projects they needed and took
two brands to bankability."
Figures: ~€1M annual revenue · 2 brands made bankable in Germany · 2 markets, sold direct to installers. Link: "The energy thread, in full" → /about#energy

**RECORD: "Where I've worked."** Table: Years | Company | Role
2026 – Sonova, Principal Product Owner · 2025–26 Trusted Shops, Principal Product Manager, D2C apps and web portal · 2024–25 ON, Principal Product Manager, D2C e-commerce app · 2024 Lotto24, Principal Product Manager, freiheit+ launch · 2022–23 WIWIN, Principal Product Manager, investment platform · 2020–21 Douglas, Principal Product Manager, Retail Apps · 2019 Eurowings Digital, Senior Product Owner, Digital Services · 2016–17 IONOS, Product Manager, Mobile Messenger · 2013 – A1 Telekom Austria, App supplier, project and product management · 2009–15 M47 Interactive, Co-founder, Product Manager Mobile Apps · 2008–12 BSL Greentech, Felix Solar, Founder, PV module import · 2005–08 Jamba!, Product Manager Mobile

## Case study template (all four)

Breadcrumb "Work / 0N", large serif H1, lede. Then a 4-column meta row (Client, Role, Period, Team)
under a dark rule. Then three big figures. Then sections, each a 3/12 uppercase label + 9/12 prose,
separated by thin rules. The Result section opens with a pull quote (navy left border, serif
italic). End with previous/next links.

### /work/douglas
- H1: Moving a billion-euro app business onto a new backend without a minute of downtime
- Lede: Douglas needed its shopping apps on a new commerce backend while millions of customers kept using them. Four teams, one migration, and no pause in product work.
- Meta: Douglas, European beauty retail · Principal Product Manager, Retail Apps (contract) · 08.2020 – 04.2021 · 4 Scrum teams, 40+ people · iOS, Android
- Figures: €1B+ annual revenue running through the apps · 0 downtime during the move to SAP Hybris · 40+ people across four Scrum teams
- Situation: Douglas runs one of Europe's largest beauty e-commerce businesses, and more than a billion euros a year runs through its iOS and Android apps. Those apps had to move onto a new SAP Hybris commerce backend, with millions of customers using them throughout.
- What made it hard: Changing the backend touches nearly everything a shopper does: search, product pages, basket, checkout, account. Four Scrum teams were working on the apps at the same time, and the business couldn't stop shipping while the foundation changed underneath them. Other work didn't wait either. Search and discovery were being redesigned, and external technology suppliers were building real-time photo and video editing into the apps.
- What I did: Led product for the iOS and Android apps across four Scrum teams and more than 40 people, owning roadmap and backlog through the migration. · Ran the move to SAP Hybris alongside ongoing product work instead of freezing the roadmap. · Redesigned search and discovery during the same period. · Coordinated the external technology suppliers delivering real-time picture and video editing.
- Result (pull quote): The apps moved to the new backend with zero downtime for millions of customers. Then: Search and discovery came out of the same period redesigned, so customers got an improved app rather than just a replatformed one.
- What carries over: When many teams change a live system together, sequencing and communication are product work, not project admin. The same problem shows up when an AI platform swaps models under live traffic, or when an energy company pulls dozens of installers onto one platform.

### /work/wiwin
- H1: Making a BaFin-regulated investment flow feel safe enough to finish
- Lede: WIWIN lets private investors put money into sustainable projects. Regulation decided what the flow had to contain. My job was to make people trust it enough to complete it.
- Meta: WIWIN, sustainable-investment crowdfunding · Principal Product Manager (contract) · 05.2022 – 08.2023 · Nearshore development team · web, mobile web
- Figures: +50% conversion after lab usability testing · 3 external services in one journey: KYC, payment, tokenization · BaFin, the regulator every step had to satisfy
- Situation: Crowdinvesting falls under BaFin, Germany's financial regulator. Every step from sign-up to investment carries requirements: identity checks, disclosures, payment handling. WIWIN needed an investment and self-service platform that met all of them.
- What made it hard: Compliance rules don't care whether a flow is pleasant, and every requirement adds a step. In investing, extra steps feel like risk. If a flow is confusing, people start to wonder whether their money is safe, and they leave. Three external providers, for KYC, payment and tokenization, also had to feel like one product to the investor, and the platform was built with a nearshore team.
- What I did: Owned the investment and self-service platform end to end, working with the nearshore team. · Translated the compliance constraints into a usable flow, so the rules shaped the design from the start. · Integrated the three external services: KYC, payment and tokenization. · Ran lab usability testing to find where the flow lost people's trust.
- Result (pull quote): Conversion rose 50%, from making the flow feel more secure and removing steps it didn't need.
- What carries over: I treat regulation as a design input, not something to route around. That now applies directly to AI: the EU AI Act is putting AI products in the same position crowdinvesting was in, with obligations the product has to meet and users who need to trust it anyway.

### /work/trusted-shops
- H1: Growing a consumer app through 30,000 partner shops
- Lede: Trusted Shops reaches consumers through the online shops that carry its badge. I owned the apps and web portal where those consumers land, and the strategy for getting more of them there.
- Meta: Trusted Shops, review and trust SaaS · Principal Product Manager, D2C apps and web portal (contract) · 11.2025 – 05.2026 · iOS, Android (Flutter), consumer web portal
- Figures: +27% sign-ups from a growth strategy across 30,000 partner shops · #1 App Store ranking for brand keywords in 10 markets · 4.7 star rating held steady through a full rebrand
- Situation: Trusted Shops certifies online shops and collects their reviews. On the consumer side, shoppers use its iOS and Android apps and a web portal. Most of them find it through the roughly 30,000 partner shops that carry the Trusted Shops mark.
- What made it hard: This is a business-to-business-to-consumer product. Consumer growth runs through partners whose main concern is their own shop. At the same time the apps were being rebranded, which is a reliable way to lose ratings and search position, in ten markets at once.
- What I did: Owned iOS, Android and the consumer web portal end to end. · Worked on app store optimization until the apps ranked #1 for brand keywords in 10 markets. · Managed the rebrand of the apps while keeping the rating at 4.7 stars. · Initiated a growth strategy across the 30,000 partner shops. · Outlined a two-to-five-year strategy for the department. · Used n8n automation and Claude tooling in day-to-day product work.
- Result (pull quote): Sign-ups rose 27%, and the apps came through the rebrand with their rating and search position intact.
- What carries over: A lot of products reach customers through someone else: installers, retailers, platforms, integrations. Growth then depends on making the product worth it for the partner first. That holds for an AI tool sold through platforms just as much as for a heat pump sold through a regional installer.

### /work/redline
- H1: An AI contract reader that has to prove every claim it makes
- Lede: Redline reads a contract before a freelancer signs it, flags the clauses that could hurt them, and drafts a reply they can send. It's my own product, it's still in build, and it's where I'm learning the parts of AI product work that don't show up in a demo.
- Meta: Own product, pre-launch · Founder and product manager · Started 08.2026 · Next.js, Supabase, LLM via OpenRouter
- Figures: 100% of risk flags must quote a real sentence from the document, enforced in CI · 10 architecture decision records, written before the code · 7 tests that define "good", one build gate and six launch gates
- The user: A US freelancer or small-business owner looking at a contract the other side drafted. They suspect a clause could hurt them and can't tell which one. A lawyer's review costs around $670 on average (ContractsCounsel), so most people just sign. Before building anything I collected 18 sourced pain findings and looked at 11 competitors, including free tools that already explain contracts.
- The real problem: A language model that paraphrases a contract can sound right and be wrong, and the reader has no way to tell the difference. For this user, a confident mistake is worse than no answer. So the product question wasn't "can a model read a contract?" It was "how does the user check what the model says?"
- Decisions (small serif subheads):
  - Every flag cites its sentence, exactly: The server splits the stored text into sentences with fixed positions. The model cites a sentence ID and repeats the quote, and the quote has to match the stored text byte for byte or the whole analysis fails. I dropped character offsets early because models are bad at counting characters. Nothing is fuzzy-matched.
  - Quiet is a feature: Redline flags only what is uncapped or inescapable. A fair contract returns zero risk flags and a checklist of what was checked. A tool that finds something in every document is a horoscope.
  - Absences are kept separate: Missing protections, like a contract with no payment deadline, go in their own list. They cite nothing, because they claim nothing about the text.
  - Confidence follows provenance: How firmly Redline says something depends on what the statement rests on, never on how sure the model sounds. Where the answer depends on facts it doesn't have, like jurisdiction or leverage, it says nothing.
  - Say no to OCR: Scanned documents are refused. A citation is worthless if it points at misread text.
  - Explain, never advise: Redline says what the document says and does. It doesn't tell anyone what to do legally. DoNotPay's $193K FTC settlement came from exactly that claim.
- How it's built: Research first, then a PRD with seven tests, then ten decision records, then tickets. Coding agents built the tickets in an unattended run. Every ticket was checked with typecheck, the full test suite, a production build and a scan for stubs and mocks before it was committed. Wherever an agent had to decide something without me, the decision went into a build report I review.
- Honest status (render as a plain darker-paper box, not a card with shadow): **Where it stands, September 2026.** 17 of 20 build tickets are done and CI passes. What isn't done: No output has been verified against the real model yet. An upstream rate limit blocked every attempt, so only the stubbed pipeline is proven. · The real test corpora, including a set of fair contracts that must come back clean, are still to be assembled by hand. I don't want an agent-written "fair" contract grading the model. · A lawyer's review of the severity ranking and a direct test against a free competitor are both still open. · Who pays, and how, is undecided. Then: I'm publishing the gaps on purpose. Eval design, failure behaviour and deciding what not to claim are the job.
- What carries over: Evaluation as a product deliverable. Designing for the times the model is wrong. Keeping cost, latency and quality in view together. And the same instinct as in regulated fintech: if users can't check it, they shouldn't have to trust it.

## About `/about`

- Label ABOUT, H1: "Twenty years, one habit: understand the system before changing it."
- Intro, 7/12 prose with a navy drop cap + 5/12 photo `portrait-standing.jpg`:
  1. I studied computer science at TU Berlin, then moved to the Universität der Künste for a Diplom in electronic business. Engineering on one side, design on the other. That still describes how I work: I can read an API spec and argue about a flow in Figma in the same afternoon.
  2. My first product job was at Jamba! in 2005, launching mobile web in more than 20 countries and adding €40M in turnover. A/B testing there lifted conversion 48%, and I haven't stopped testing since.
  3. In 2009 I co-founded M47 Interactive, a bootstrapped mobile startup where I was product and tech lead. Without outside money, our dating app grew to a million users and a #1 Google ranking. In parallel I was running two solar import companies, which is further down this page.
  4. Since then I've mostly worked as an interim and contract product lead. Companies bring me in when the problem is urgent and tangled: a backend migration under live traffic at Douglas, a regulated investment platform at WIWIN, a charity lottery shop at Lotto24 that had to launch on a tight timeline. Today I'm Principal Product Owner at Sonova, working on a platform that routes consumer demand for hearing care to independent partner stores.
  5. Short projects are the format I've chosen, and I do stay when something is worth it. I've supplied apps to A1 Telekom Austria since 2013, co-founded RoofUz in 2022, and have co-run Weserland, a Berlin coworking space for 40 creative freelancers, since 2011.
- HOW I WORK: "Four things I do on every engagement." 2×2 ruled grid with mono numbers 01–04:
  - Find the real constraint: The blocker is rarely where it looks. With the solar brands it was bank financing, not price. At WIWIN it was trust, not features. I go deep until I can name it.
  - Measure the change: A/B tests and usability labs at Jamba!, mobileJobs, WIWIN and ON moved conversion by +48%, +28%, +50% and +7%. If a change can't be measured, I'm careful about calling it a win.
  - Give teams room: I do my best work with people who take ownership, and I try to create the conditions for it. At ON I moved dedicated teams into squads and brought in an agile design process, and features shipped 20% faster.
  - Say what you know, and when you'll know more: I once went quiet during a crisis while I worked out the right answer. It cost me trust. Now stakeholders hear what I'm doing and when they'll get an answer, even mid-analysis.
- WHAT CLIENTS SAY, pull quote: "Thank you Felix for taking over the interim product management for our mobile-first-site freiheitplus.de delivering the MVP on time! You showed us strong product, tech, communication and agile management skills." (Björn Behrendt, Co-Founder & MD, MarketingPush, on the freiheit+ launch, LinkedIn recommendation)
- Navy band, id `energy`, THE ENERGY THREAD: "Solar modules, a utility portal, and a campaign to quit coal."
  - **2008 – 2012: BSL Greentech and Felix Solar.** I founded and ran two trade companies importing photovoltaic modules from Chinese manufacturers, by the container, through Rotterdam and Hamburg. We sold direct to installers and EPCs in Germany and Italy, the two biggest European solar markets of the time, and reached roughly €1M in annual revenue across a portfolio of module brands.
  - The hard part wasn't selling modules. German banks would only finance installations using brands with a local track record. An unknown brand couldn't sell at scale, however good or cheap it was. So I set up the reference projects the banks needed and took two brands from unknown to bankable.
  - When Germany cut its feed-in tariffs in 2011 and 2012, domestic demand dropped sharply. I read that as the signal to wind both companies down, and I did.
  - **2019: climatecampaign.com.** A self-started initiative to help people switch to renewable electricity providers.
  - **2020: STADTENERGIE.** At interstruct I shipped a mobile-first site and self-service portal for this utility.
  - **Since 2022: RoofUz.** A co-founded platform bringing digital processes to wood construction, a trade that has barely been digitized. It won the BIM-Löwen award and was named one of the top 50 European startups.
- FULL RECORD (id `record`): "Every engagement, with what changed." Table Period | Company and role | What changed:
  2026 – · Sonova · Principal Product Owner · Lead-routing platform connecting consumer demand to independent hearing-care partners
  11.2025 – 05.2026 · Trusted Shops · Principal PM, D2C apps and web portal · #1 brand keywords in 10 markets; 4.7 rating through rebrand; +27% sign-ups
  09.2024 – 07.2025 · ON · Principal PM, D2C e-commerce app · 20% faster delivery; A/B testing program, +7% conversion; cross-country ASO
  03.2024 – 08.2024 · Lotto24 · Principal PM · Launched the freiheit+ charity lottery shop on a tight timeline, hitting CAC targets
  05.2022 – 08.2023 · WIWIN · Principal PM · BaFin-compliant investment platform; KYC, payment, tokenization; +50% conversion
  2022 – · RoofUz · Co-founder · Digital processes for wood construction; BIM-Löwen award
  02.2022 – 04.2022 · IONE Software · Principal PM · POS order module; bill splitting and business-meal flows
  05.2021 – 09.2021 · TLGG · Product Owner · D2C food-supplement store concept; basis for a C-level go/no-go
  08.2020 – 04.2021 · Douglas · Principal PM, Retail Apps · 4 Scrum teams; zero-downtime SAP Hybris migration; search redesign
  03.2020 – 09.2020 · interstruct · Product Manager CX · Mobile-first site and self-service portal for utility STADTENERGIE
  02.2019 – 07.2019 · Eurowings Digital · Senior Product Owner · 3 Scrum teams; navigation redesign; taxi, rail and bus partner integration
  11.2018 – 03.2019 · mobileJobs · Product Manager · +28% conversion in blue-collar recruiting funnels via A/B testing
  04.2018 – 08.2018 · Cornelsen · Product Strategy Manager · C-level digital-learning strategy from market and regulatory analysis
  09.2017 – 04.2018 · Lokalleads · Product Owner · B2B automation and sales backend for craft businesses
  08.2016 – 08.2017 · IONOS · PM Mobile Messenger · Secure messenger to 250k users within weeks; invented RealEmoji
  06.2013 – · A1 Telekom Austria · App supplier · 10+ branded apps across iOS, Android and Windows; budget responsibility
  01.2009 – 03.2015 · M47 Interactive · Co-founder · Bootstrapped dating app to 1M users; performance-based ad system
  2008 – 2012 · BSL Greentech, Felix Solar · Founder · PV import into Germany and Italy; ~€1M revenue; two brands made bankable
  10.2005 – 08.2008 · Jamba! · Product Manager Mobile · Mobile web in 20+ countries, +€40M turnover; +48% conversion
- EDUCATION AND LANGUAGES: "Trained in both code and design." Universität der Künste Berlin, 2001 – 2005: Diplom (Master's), Electronic Business · Technische Universität Berlin, 1999 – 2001: Vordiplom (Bachelor's), Computer Science · Languages: German, native. English, C1, the working language of every product team I've been part of for the last decade.

## Contact `/contact`

- Label CONTACT, H1: "If you're building something complicated, I'd like to hear about it."
- Left 7/12: label EMAIL, then the address as a huge serif link: felix.hofmann@haorga.com (mailto).
  Then a ruled two-column list: LinkedIn: linkedin.com/in/felix-gerd-hofmann (link to
  https://www.linkedin.com/in/felix-gerd-hofmann) · Based in: Berlin, Germany · Open to: Senior and
  principal product roles, permanent or interim · Focus: Applied AI, the energy transition, consumer
  products at scale · Work setup: On-site, hybrid or remote; open to relocation · Languages: German
  (native), English (C1). Buttons: "Write an email" and "Connect on LinkedIn".
- Right 5/12: photo `walking-bw.jpg`.
- No contact form.

## Impressum `/impressum` (German)

Impressum, Angaben gemäß § 5 DDG: Felix Hofmann, Weserstraße 21, 12045 Berlin, Deutschland.
E-Mail: felix.hofmann@haorga.com. Verantwortlich für den Inhalt nach § 18 Abs. 2 MStV: Felix Hofmann,
Anschrift wie oben. Note in the Datenschutz section that this demo is hosted by Lovable.

## Don't

- Don't invent any metric, company, testimonial, logo wall or client quote beyond the copy above.
- Don't add a skills bar chart, a "tech stack" icon grid, or a timeline with dots.
- Don't rewrite the copy into marketing language.
