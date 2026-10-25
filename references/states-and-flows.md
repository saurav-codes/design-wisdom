# States, flows, forms and navigation

Open this when you build or review onboarding, empty/loading/error/limit screens, status pages, forms, filters, AI output UI, or nav and information architecture. It adds tactics and numbers on top of frontend-design, which already covers the basic state checklist, inline errors and a11y floor.

## Walkthroughs to run on a real product

### Write the state table before the screens
For every async job, payment, import, deploy or order, list each state: pending, processing, on hold, failed, refunded, done. Design one screen per state with a next step. In a money app most people only open it to check "did it land?", so the team designed 15 status screens. Trust is won on screens you hope nobody sees.
- Look for: any state where the UI shows a bare word ("Pending") or nothing.
- Fix: headline status sentence, timeline with the current step, who or what is working on it, one contact or retry action.
Sources: TimGabe ([I Redesigned a Neobank App](https://www.youtube.com/watch?v=0GMQRCnOQmo)); amirmoradiUX ([How to Become a Product Designer in the AI Era](https://www.youtube.com/watch?v=ky_F3jdnT4Y)); uxpeak ([Top 5 Advanced UX/UI Design Tips, Part 3](https://www.youtube.com/watch?v=Xzh8xjimmp8))

### Render every state of every control on one test page
Payment: processing, success, failure. Button: active, disabled, loading. Steppers: minus disabled at the minimum of 1. Know what each state must tell the user, then check them side by side before shipping.
- Look for: min/max limits that are not disabled, success states that exist only in code.
Sources: amirmoradiUX ([How to Become a Product Designer in the AI Era](https://www.youtube.com/watch?v=ky_F3jdnT4Y)); amirmoradiUX ([Figma Agent vs Claude](https://www.youtube.com/watch?v=wx2ylgMU8WM))

### Annotate onboarding as a motivation curve
Walk the flow step by step and write the expected user motivation (rising or falling) beside each step, as growth.design case studies do for Grammarly. The steps where it dips are where you ask for effort before showing value.
- Look for: a data request or permission prompt placed before the first win.
Sources: amirmoradiUX ([I Became a Product Designer Without a Degree](https://www.youtube.com/watch?v=_ln-Xjd3acM))

### Reframe a drop-off as a trust or value problem
A drop after an eligibility step was not "users are confused". It was "we ask for personal data before showing value". Shortening the form may not help if the cause is trust. Fix directions: show value earlier, reorder, show examples before asking for input.
Sources: amirmoradiUX ([Why My Designs Kept Failing](https://www.youtube.com/watch?v=Bh0KK5xQOGo))

### Map the visitor journey and delete clicks
List every step from first load to the goal (book, buy, sign up). For each, ask what the visitor needs to do and how to make it simpler, more obvious and more pleasant. When they are ready to act, the action is one click away.
Sources: DesignSpo ([24 Web Design Concepts You Need To Know](https://www.youtube.com/watch?v=a_6s4AKQ2VI))

### Card sort before you lock navigation
List 20 to 40 nav items and settings, have 5 people group and name them, then compare with your grouping. Look for items placed somewhere you did not expect. UserTesting found some of its own nav assumptions were wrong and fixing them early was cheap. Follow with a navigation test on a light prototype.
Sources: Jason Giles ([How UserTesting does user testing on UserTesting](https://www.youtube.com/watch?v=X-Fqc1t_gE4))

### Test two versions in hours instead of arguing
When two interaction solutions are both viable, build quick versions of both and put them in front of a handful of users before review.
Sources: Jason Giles ([How UserTesting does user testing on UserTesting](https://www.youtube.com/watch?v=X-Fqc1t_gE4))

### Spend polish by flow importance
Rank screens by importance. Onboarding, first run and the main action get the deepest attention. Settings and billing get less. Define states and edge cases early and mark where the emotional moments sit. Settle tokens and core components before redesigning several flows so they feel like one product.
Sources: TimGabe ([Our World Class App Design Formula](https://www.youtube.com/watch?v=wmTkiF23GRQ)); TimGabe ([How Top 1% Apps Earn Your Second Visit](https://www.youtube.com/watch?v=YA3QpYIKqNI))

## Onboarding: value before effort

### Reach the first win inside 60 seconds
Let the product speak before asking for effort, like a free sample in a store. A breathing app starts a real session at once. TimGabe cites: retention rises considerably when users find value in the first 60 seconds, and apps lose 77% of users in 3 days on average. Tinder let users connect, auto-pull photos and swipe in under a minute; he cites most dating apps losing over 70% after session one, and Tinder sessions averaging 11 minutes against 3.
- Look for: tours, goal wizards and profile steps standing between sign-in and the core action.
- Fix: land the user in the core action with sensible defaults. Measure time to first value.
Sources: TimGabe ([The Hidden App Growth Killer](https://www.youtube.com/watch?v=55hDj88zKa8)); TimGabe ([How Tinder's Design Hacked Society](https://www.youtube.com/watch?v=4yKtlOWClhA))

### Cut onboarding to what the product technically needs
Granola's onboarding is two screens: sign in with Google, grant mic access. The next meeting is the value. Raycast launched with no formal onboarding because it had one search bar and a rigid open, type, act loop; onboarding came later. If the first screen needs a tutorial to start, fix the first screen.
- Fix: keep only auth and required permissions. Make the main control obvious before adding any tour.
Sources: TimGabe ([How To Solve The App Onboarding Paradox](https://www.youtube.com/watch?v=Aa89MC8jX2c)); TimGabe ([How Raycast Reached a $100M+ Valuation](https://www.youtube.com/watch?v=eWGNjTLK84c))

### Let people try or build before the account wall
Suno lets people make and share a song before asking for data, phone or payment. Duolingo has users pick language and goal and do a first lesson before signup. TimGabe and uxpeak cite endowment and IKEA effects: people value what they built. Let users pick a name, palette or template first and label the gate button "Continue", not "Sign up".
- Look for: can a visitor reach the first aha (demo, sample output, sandbox) before the account wall, permission or card form?
- Fix: pre-signup mini setup or live demo that saves state, then ask for an email to keep it. Defer email verification, profile and preferences until after the first success. Use social login to prefill.
Sources: hatchconference ([Designing Products for Trust](https://www.youtube.com/watch?v=_rq9djF2dqI)); uxpeak ([The UX Psychology Behind Apps People Can't Stop Using](https://www.youtube.com/watch?v=2TlIg3VokY8)); TimGabe ([How Tinder's Design Hacked Society](https://www.youtube.com/watch?v=4yKtlOWClhA))

### Move the scary first action into onboarding
In one app, drop-off happened at the record button but onboarding completion was high. The fix was to move the mic test into onboarding, where motivation is high, and replace the dead end with a real sample output (interactive recap). That answers "does it work" and "what will it give me" before the app opens.
- Fix: make the first core action an onboarding step that ends in a sample result. Never show a refusal wall after tiny test input.
Sources: TimGabe ([How Top 1% Apps Earn Your Second Visit](https://www.youtube.com/watch?v=YA3QpYIKqNI))

### Never start a checklist at zero
Goal gradient. The speaker cites a car wash card with 8 empty stamps against a 10-stamp card with 2 pre-filled (same 8 washes needed): the pre-stamped card was completed at nearly double the rate. LinkedIn's meter never starts at zero.
- Fix: show setup at 20% with "account created" checked instead of 0% with five empty steps.
Sources: uxpeak ([The UX Psychology Behind Apps People Can't Stop Using](https://www.youtube.com/watch?v=2TlIg3VokY8))

### Personalize first run so it feels owned
Let users pick voice, speed, theme, name, avatar or card style and show it reflected at once, like adjusting seats and mirrors in a new car. In the neobank redesign users picked their card as step one, so it felt theirs before any deposit. TimGabe cites the mug study: owners demanded about twice as much to sell as buyers would pay.
Sources: TimGabe ([The Hidden App Growth Killer](https://www.youtube.com/watch?v=55hDj88zKa8)); TimGabe ([I Redesigned a Neobank App](https://www.youtube.com/watch?v=0GMQRCnOQmo))

### Branch first run by persona and by user stage
Identify 3 main personas and what each wants to feel or achieve, ask one question (goal or role), and change the checklist, copy and feature suggestions per answer. After setup, branch the dashboard by activity: new user gets welcome, weekly goals and a few simple categories; regular user gets today's plan; power user gets stats first. Hide advanced widgets from new users.
- Fix: switch on item count (0, a few, many). A/B test the variants.
Sources: TimGabe ([How Netflix Made Us All Binge](https://www.youtube.com/watch?v=hIm3d3JAsPw)); uxpeak ([Top 5 Advanced UX/UI Design Tips, Part 3](https://www.youtube.com/watch?v=Xzh8xjimmp8))

### Learn by doing, with a three-card cap if you need a tour
Give the first task with guided hints (Sudoku) and coach marks on the real UI instead of video or text. If a welcome is unavoidable, use three cards, one idea each, no input fields, so users leave thinking "I can do this" (IKEA instructions idea: a 12-page manual up front makes people quit).
Sources: TimGabe ([The Hidden App Growth Killer](https://www.youtube.com/watch?v=55hDj88zKa8))

### Find the friction sweet spot
Shortening onboarding is usually the biggest win, but stripping too far leaves users unguided. Count the steps and the screen where value first appears (aim for within the first 5). Move secondary data into tooltips or accordions. Test removing one step and see if users still understand. A story-style welcome carousel can explain value without extra steps.
Sources: TimGabe ([Give Me 13 Minutes & I'll Grow Your App](https://www.youtube.com/watch?v=v1f9iYZ2GhQ))

### Make a long quiz earn its length
Every extra question must change what the user sees on the first screen, or filter for buyers with real pain. Cal AI (20+ steps) and Noom (113 screens), per the speaker, justify length by personalizing. TimGabe cites Aronson and Mills 1959: more effort raises the value of the outcome, and Forer 1948 (Barnum effect): generic text feels personal. His example asks birth date, time and city before a paywalled result.
- Fix: if the payoff is personal (plan, score, setup), gather inputs first and show a "building your result" step before the paywall. Drop questions that change nothing.
Sources: TimGabe ([How To Solve The App Onboarding Paradox](https://www.youtube.com/watch?v=Aa89MC8jX2c)); TimGabe ([The Twisted Psychology Behind Top 1% Apps](https://www.youtube.com/watch?v=nQKWYmrixCU))

### Use plain, warm language in intimidating categories
For finance, health, insurance and crypto, use friendly visuals and warm detail, and do not assume users know the rules (Phantom did this for crypto).
- Fix: no jargon on first-run screens. Add a plain-language line next to every technical field.
Sources: TimGabe ([The Secret Behind Weirdly Addictive Apps](https://www.youtube.com/watch?v=Du2lkZ_cux8))

### Add a human voice and task help
Corebook put a short voice message from the template's creator on the welcome page; the speaker says it improved onboarding and stickiness. After launch, a client FAQ plus screen recordings of their own site, kept forever, answers "how do I log in, add a post, add a product" like SaaS docs. Split long text into story-style cards with progress dots.
- Fix: a 30 to 60 second video or audio intro with a skippable text version. Short in-app how-to for the real first tasks. Watch what new users ask in the first two weeks to find missing guidance.
Sources: Hatch Conference ([Death to the brand guidelines PDF](https://www.youtube.com/watch?v=C7pcY87_3jo)); SelfMadeWebDesigner ([Complete Web Design Process](https://www.youtube.com/watch?v=T5JglDcd54A))

### Greet by name and ask in plain questions
"Hi, Emily. How did you sleep last night?" beats "How many hours did you sleep yesterday?". Name plus natural language makes people feel recognized and lowers friction.
Sources: uxpeak ([This Video Will Take You From Junior to Senior UX/UI Designer](https://www.youtube.com/watch?v=YlN28RNChl0))

## Empty states and starting points

### Give empty states a starter kit
Beyond frontend-design's headline, line and one action: add practical tips ("invite teammates, set deadlines") and a friendly illustration. Character.ai ships ready-made bots to try at once. Copy.ai gives a template library. A blank basket makes people wonder if something is broken.
- Look for: a lone "Create" button on an empty list.
- Fix: 3 to 5 starter templates or sample data to try immediately, next to the create action.
Sources: uxpeak ([Top 5 UX/UI Design Tips, Part 2](https://www.youtube.com/watch?v=gG4urkinFQI)); Hatch Conference ([The Shape of AI, Emily Campbell](https://www.youtube.com/watch?v=FX_JDRKhZEU)); amirmoradiUX ([How to Become a Product Designer in the AI Era](https://www.youtube.com/watch?v=ky_F3jdnT4Y))

### Prefer implicit defaults over an empty prompt box
A plain AI chat box forces users to know what to ask. Loom found automation that needs no prompt (auto title, summary, chapters) was adopted more than tools users had to drive. Offer the prompt box as the fallback.
- Fix: pre-filled titles, suggested next actions, auto summaries as the main path.
Sources: hatchconference ([Loom's VP of Design](https://www.youtube.com/watch?v=aH3GHVnL7YU))

### Give chat and prompt boxes a real first screen
Booking.com's AI planner shows three things: a note that output is machine-generated and may contain errors, a friendly line ("I'm still learning but happy to help") that sets expectations, and clickable example questions because many users have never used a chat AI.
- Fix: 3 to 4 clickable example prompts, one line on what it can and cannot do, a visible error-possible note.
Sources: hatchconference ([The Impact of AI on UX Design, Jascha Goltermann](https://www.youtube.com/watch?v=YDGiKuuoSzM))

### Break big AI generation into a plan step
An AI grant-writing tool dumped 20 pages at once. A plan step before generation made the surprise smaller and gave users control.
- Fix: show an outline for approval, then generate.
Sources: TimGabe ([The Secret Behind Apps Big Players Can't Copy](https://www.youtube.com/watch?v=zH0SVLzLBpU))

## Waits, status and progress

### Explain every wait
An unexplained wait feels longer than an explained one. "Pending" became "Your transfer was temporarily on hold while we completed routine checks" plus a contact support button. Multi-step waits show a count like "2 of 8".
- Look for: bare "Pending" or "Processing".
- Fix: reason, expected time, help action. Step counter on long processes.
Sources: TimGabe ([I Redesigned a Neobank App](https://www.youtube.com/watch?v=0GMQRCnOQmo))

### Narrate long jobs and keep the UI alive
Perplexity shows what it is doing and why it needs something (like location) when it asks, which builds trust during waits. Treat in-between moments as intentional.
- Fix: live step text for imports, AI runs and deploys ("Reading 3 sources...", "Provisioning database..."). Skeletons, streaming text, a small pulse on submit. Never a frozen button.
Sources: hatchconference ([Designing Products for Trust, Metalab](https://www.youtube.com/watch?v=_rq9djF2dqI)); TimGabe ([How Top 1% Apps Keep You Hooked](https://www.youtube.com/watch?v=D9SXaj6qQIQ))

### Treat latency as a design constraint for AI
A model that reasons well but takes 10 minutes breaks a "co-create with me" product; the panel lost months building for slow agent workflows. For high-stakes work, run in the background and show results when ready.
- Fix: streaming or staged progress, UI stays interactive, cancel button, long jobs move to a background state with a notification instead of a blocking spinner.
Sources: Panel ([AI is Redesigning Design Tools](https://www.youtube.com/watch?v=Rrt_MDrpraU))

### Show progress steps, but hide a scary count
A "step 2 of 5" bar relieves users and uses goal-gradient. With many steps (12) and no value yet, a visible total can cause early bounce; Typeform hides step counts in long forms by default.
- Fix: step bar up to about 5 steps. Longer flows get a plain fill bar without a total, or value up front.
Sources: TimGabe ([The Hidden App Growth Killer](https://www.youtube.com/watch?v=55hDj88zKa8))

### Status pages reduce anxiety with a headline, timeline and person
Order tracking redesign: confident headline ("Your order is on the way"), icons for time slot and address, a human courier card with photo and call/message buttons, and a visual timeline instead of a text list of dates.
Sources: uxpeak ([Top 5 Advanced UX/UI Design Tips, Part 3](https://www.youtube.com/watch?v=Xzh8xjimmp8))

### Put a rarely used safety control one tap away
TimGabe cites a 1972 noise study: people with a stop button worked better even if they never pressed it. The neobank put freeze card, lock online payments, set limits and show PIN one tap away, with freeze on the dashboard. A real person by WhatsApp, Telegram or email works the same way.
- Fix: pause, freeze, undo, export, contact human on the main screen, not buried in settings.
Sources: TimGabe ([I Redesigned a Neobank App](https://www.youtube.com/watch?v=0GMQRCnOQmo))

## Errors, limits and recovery

### Make error recovery the premium moment
TimGabe cites a 2007 review: when a failure is handled very well, people can end up as happy as if nothing went wrong (service recovery paradox). A declined payment got an alert about checking the balance with a contact support button beside it. Failed transactions with "zero information on what to do" lose people.
- Fix: every error names the cause, the fix, and a next action (retry, change method, contact support).
Sources: TimGabe ([The Psychology of Premium Apps](https://www.youtube.com/watch?v=8EAYZe6y3I8))

### Never answer an action with nothing
Users tested their mic, hit stop, and were told the session was too short to count, with nothing to show. A founder: "I was expecting anything instead of nothing."
- Fix: say why, state the threshold, say what to try, and keep partial output visible.
Sources: TimGabe ([The Psychology of Premium Apps](https://www.youtube.com/watch?v=8EAYZe6y3I8))

### Build one limit-reached component with count and date
Two screens showed the same generic "You've used all your sessions" with no count or date. The shared fix: a "2 of 2 sessions used" badge, "You've used both sessions this month", and the exact refresh date.
- Fix: used/total, plain statement, reset date or upgrade path, in one component for quota, trial and usage limits.
Sources: TimGabe ([The Psychology of Premium Apps](https://www.youtube.com/watch?v=8EAYZe6y3I8))

### Replace a "maybe" with a plain warning next to the cause
TimGabe cites a UCL finding that people stress more over a maybe than a sure thing. Beside the crypto address the screen said "Use the wrong network and your money may be lost or take weeks to recover." Clear warnings beat vague reassurance.
- Fix: the specific irreversible-risk warning sits next to the field that causes it, not in a footer.
Sources: TimGabe ([I Redesigned a Neobank App](https://www.youtube.com/watch?v=0GMQRCnOQmo))

### Turn the worst moments into a designed one
Chrome's offline dino turned a dead page into a game; the speaker cites about 270 million plays a month four years after launch. List the worst moments (payment fails, connection lost, 404, 500) and add care there.
- Fix: custom offline, 404 and 500 pages with personality and a clear way back.
Sources: TimGabe ([The Psychology of Premium Apps](https://www.youtube.com/watch?v=8EAYZe6y3I8))

### Be honest about product rules in the UI
An order screen offered "cancel" at any time but the product could not honor it. The better one followed the rule and explained it.
- Fix: hide or disable actions the backend will refuse, with the reason in text ("Cannot cancel after preparation starts").
Sources: amirmoradiUX ([How to Become a Product Designer in the AI Era](https://www.youtube.com/watch?v=ky_F3jdnT4Y))

### Keep negative feedback in the system
Games teach because failure is visible. A system that only says "good job" hides how the product works.
- Look for: checklists and dashboards that only celebrate. Failed states, over-limit warnings and "this did not count because X" need real copy and styling.
- Look for: streaks, badges, rings or confetti the user could not explain back. Tie them to a real outcome or remove them.
Sources: hatchconference ([The Danger of Gaming the System](https://www.youtube.com/watch?v=_m2T86qycPA))

## AI output states

### Give every AI answer sources, a stop button and a way to steer
Perplexity patterns: pick a focus, attach files, show reasoning steps, let the user pause or redirect mid-run, cite sources the user can inspect and exclude, suggest next questions. Hallucinations make visible sources critical.
- Fix: Stop button, visible progress steps, inline citations with links, a way to reject a source. Never present generated output as final without provenance.
Sources: Hatch Conference ([The Shape of AI, Emily Campbell](https://www.youtube.com/watch?v=FX_JDRKhZEU))

### Add refinement chips and a feedback control under output
One-tap shaping (shorter, longer, snappier, more professional) saves users from searching for words. Booking.com puts small "helpful / not helpful" controls on each recommendation and longer AI answer for a tight quality loop.
- Fix: 3 to 5 refinement buttons plus regenerate and undo. Inline thumbs up/down with an optional reason, not a modal.
Sources: Hatch Conference ([The Shape of AI, Emily Campbell](https://www.youtube.com/watch?v=FX_JDRKhZEU)); hatchconference ([The Impact of AI on UX Design](https://www.youtube.com/watch?v=YDGiKuuoSzM))

### Summarize, then link to the source record
Beyond "don't make me think", speaker adds "don't make me work as hard": Slack summarizes threads and links to dig deeper, Productboard links insights back, Salesforce suggests relevant docs.
- Fix: every summary or AI suggestion links to the underlying record.
Sources: Hatch Conference ([The Shape of AI, Emily Campbell](https://www.youtube.com/watch?v=FX_JDRKhZEU))

### Turn "explainable" and "respect agency" into controls
For recommendations, automations and AI actions, add a visible "why this", a way to correct it (tell the recommender "less personalization, more variety"), and an off switch.
Sources: Hatch Conference ([What can Designers do FOR A.I., Nadia Piet](https://www.youtube.com/watch?v=Lzja_NoTflc))

### Test search and defaults with varied real queries
Zalando found "nude cocktail dress" returned only one skin tone: correct for the algorithm, wrong for the people searching. Airbnb tested profile information hierarchy to reduce biased behavior.
- Fix: try varied real queries and adjust ranking or UI, not just data.
Sources: Hatch Conference ([What can Designers do FOR A.I., Nadia Piet](https://www.youtube.com/watch?v=Lzja_NoTflc))

## Forms and inputs

### Show cost and resulting state before the commit button
Show exactly what the user will receive and the fee before they pay. TimGabe cites StubHub: hiding fees until checkout made people 14% more likely to buy, but a fee found at the end feels like a trick and nobody makes a second deposit after being tricked. In a transfer, show "new balance" right under the amount, with sender and recipient clear and an avatar for recognition.
- Fix: live summary (amount, fees, total, what arrives) above the final button. For destructive or billing flows show the result (new total, remaining quota, what will be deleted).
Sources: TimGabe ([I Redesigned a Neobank App](https://www.youtube.com/watch?v=0GMQRCnOQmo)); uxpeak ([This Video Will Take You From Junior to Senior UX/UI Designer](https://www.youtube.com/watch?v=YlN28RNChl0))

### Pre-fill the most common value
Blank forms stack decisions. uxpeak cites the Columbia jam study (24 flavors gave 3% purchase, 6 flavors gave 30%) and that 70 to 90% of users never change defaults. Pre-select the common option so the task becomes scan and adjust.
- Fix: audit forms for empty fields with a sensible default (timezone, currency, plan, date range).
Sources: uxpeak ([The UX Psychology Behind Apps People Can't Stop Using](https://www.youtube.com/watch?v=2TlIg3VokY8))

### Use chips or a combobox instead of free text or long selects
Free text invites typos and inconsistent answers. Show common options as tappable chips with an "Other" that allows typing. A 50-option dropdown is a poor experience; use a searchable combobox with a short common list on top and inclusive defaults.
- Fix: role, company size, use case, country as chips or select. Country, title, job role as combobox.
Sources: uxpeak ([This Video Will Take You From Junior to Senior UX/UI Designer](https://www.youtube.com/watch?v=YlN28RNChl0)); hatchconference ([Systems of Exclusion, Luke Murphy](https://www.youtube.com/watch?v=iLtVIEcHdSo))

### Match the input to how often and how precisely it is used
One-time, approximate setup (weight at signup): sliders and wheels are fine. Frequent, precise entry (logging 350 g of food): text field, stepper or numeric input. Offer both slider and typed input for ranges like price. Plus/minus steppers suit adjusting an existing number (cart quantity, thermostat). If users already know they want 3 bedrooms, show all options as segmented buttons.
- Fix: segmented control for small known sets. Stepper only for quantity, with units (kg, g) where relevant.
Sources: uxpeak ([Top 5 Advanced UX/UI Design Tips, Part 3](https://www.youtube.com/watch?v=Xzh8xjimmp8)); uxpeak ([$42K vs $297K UX/UI Design](https://www.youtube.com/watch?v=U7jTCgIWS4w)); uxpeak ([This UI/UX Redesign Will Teach You More Than 100 Tutorials](https://www.youtube.com/watch?v=GGg61sdEjeI))

### Keep the label visible while typing
A minimal form where the placeholder label vanishes once you type means you cannot check what the field asked. Cleaner can be worse.
- Fix: persistent top-aligned labels, or floating labels that shrink rather than disappear.
Sources: amirmoradiUX ([How to Become a Product Designer in the AI Era](https://www.youtube.com/watch?v=ky_F3jdnT4Y))

### Give forms explicit hover, focus and submit states
Buttons: slight scale down and shadow on hover. Inputs: a visible focus border plus soft shadow at one clear width, not too thick. Define loading and success states for submit, use smooth short transitions, and use correct input types (email, URL, tel).
Sources: SatoriGraphics ([Making Website Forms Is SO FAST With Framer](https://www.youtube.com/watch?v=20mQsuTTDBU))

### Ask only what you need and say why
Ask whether a field is truly needed. If it is, make it optional and open (free text with autocomplete). Delete gender and title fields unless a real feature uses them. Where kept, offer "Non-binary" rather than "Other", order alphabetically, add "prefer not to say". If a product needs a specific fact, ask the real question instead of proxying through gender. For legally required data, simplify the UI, handle compliance on the backend where possible, and say why it is needed.
- Fix: one-line helper "We ask for this because ..." with a policy link under every sensitive field. Clean data on the backend instead of restricting the UI.
Sources: hatchconference ([Systems of Exclusion, Luke Murphy](https://www.youtube.com/watch?v=iLtVIEcHdSo))

### Use prebuilt accessible form parts and scan every screen
Hand-assembled forms keep failing on basics. Brad Frost cites the WebAIM Million report: about 50 accessibility errors per page on top million home pages, mostly missing labels and low contrast.
- Fix: run axe or Lighthouse on each screen and fix at the shared component. Accessible name on icon buttons.
Sources: Brad Frost ([Is Atomic Design Dead?](https://www.youtube.com/watch?v=PK_PICNTgAg))

## Filters, selection and live feedback

### Put the outcome in the apply button
"Show 41 homes" updates live; "Show homes" could mean 41, 4 or 0. Users know whether they narrowed enough before pressing.
- Fix: live count in the button. Reword or disable at 0. A sticky bottom action area can pair the primary action with its key parameter (quantity plus add to cart, price with unit).
Sources: uxpeak ([$42K vs $297K UX/UI Design](https://www.youtube.com/watch?v=U7jTCgIWS4w)); uxpeak ([This UI/UX Redesign Will Teach You More Than 100 Tutorials](https://www.youtube.com/watch?v=GGg61sdEjeI))

### Build filters as a panel over results with live context
Level 1, one page per filter, hides choices and costs 7 taps. Level 2, one panel with slider plus typed input and live count. Level 3, histogram behind the price slider, all bedroom options visible, "3+" kept separate from "exactly 3". Level 4, match count and median beside the control ("459 of 1,557"), count per option before selecting, range selection (2 to 4), a monthly payment converted into a budget line. Extra info can add noise; show only what helps decide.
- Fix: drawer or panel so results stay visible, per-option counts, distribution on numeric filters. Users never do arithmetic.
Sources: uxpeak ([$42K vs $297K UX/UI Design](https://www.youtube.com/watch?v=U7jTCgIWS4w))

### Make search focus useful
Tapping search is a moment of intent. Show recent searches, popular items and ignorable personalized suggestions instead of a blank screen. The placeholder says what can be searched (place, dish, cuisine).
Sources: uxpeak ([Top 5 Advanced UX/UI Design Tips, Part 3](https://www.youtube.com/watch?v=Xzh8xjimmp8)); uxpeak ([$42K vs $297K UX/UI Design](https://www.youtube.com/watch?v=U7jTCgIWS4w))

### Show the effect of a value inside the control
A sleep selector shows a big face and a message ("Good sleep, aim for 8 hours") that change live as the user slides, plus comparison with last night.
- Fix: sliders, plan selectors and scoring inputs show a live preview or summary of the current value.
Sources: uxpeak ([This Video Will Take You From Junior to Senior UX/UI Designer](https://www.youtube.com/watch?v=YlN28RNChl0))

### Change at least two things for the selected state
Color plus weight, fill plus size, border plus check. For nav: change icon style and color, and make the label bolder or darker. Color-only or label-only changes are too weak.
Sources: uxpeak ([Top UI/UX Design Tips: Bottom Mobile Navigation Bar](https://www.youtube.com/watch?v=wLJ40GV2XEc)); uxpeak ([From Junior to Senior UX/UI Designer](https://www.youtube.com/watch?v=YlN28RNChl0))

### Show the comparison at the moment of completion, in a small cohort
Show standing when a task ends (workout, transaction, listen). Strava ranks against neighborhood and friends because a global leaderboard feels unwinnable. Shrink the cohort until winning feels possible, and add a human acknowledgement line for effort.
Sources: TimGabe ([Why Leaderboards Kill App Retention](https://www.youtube.com/watch?v=BxhsCu9hNpY))

### Badge only what needs action
A small badge on the top-right of the icon, outlined with the bar background color to pop, readable number, a color unlike the bar. Badge every minor update and users stop noticing.
Sources: uxpeak ([Top UI/UX Design Tips: Bottom Mobile Navigation Bar](https://www.youtube.com/watch?v=wLJ40GV2XEc))

## Navigation and information architecture

### Collapse the IA to the top-level jobs
The British Airways app redesign reduced thousands of pages to three jobs: discover, book, manage. Card sorting became the navigation directly.
- Fix: list every page, group by user job, test whether the top level can be 3 to 5 verbs (Discover, Create, Manage).
Sources: hatchconference ([Speaking to Stakeholders, Kevin Hawkins](https://www.youtube.com/watch?v=ppAIzybHoCQ))

### Keep top-level nav to 3 to 5 destinations
Good: Home, Search, Create, Messages, Profile if frequent. Bad: logout, legal, settings detail, back button, logo. Six is the hard max; more makes targets small and triggers choice paralysis.
- Fix: move settings, billing, logout and legal into a profile menu. Always label icons in B2B/SaaS. Use familiar icons (magnifier, not binoculars). Icon-only is fine only for young tech-savvy audiences.
Sources: uxpeak ([Top UI/UX Design Tips: Bottom Mobile Navigation Bar](https://www.youtube.com/watch?v=wLJ40GV2XEc))

### Give every nav item default, hover and current styles
Do not leave browser-blue underlined links. Hover example: underline appears. Current example: accent color on the page you are on. As you scroll or route, the active item updates.
- Look for: `aria-current` or `.active` styling, a visible hover, and active-state updates on scroll and route change.
Sources: ShantanuKumar ([How to design a simple website](https://www.youtube.com/watch?v=o8S9qJbvpkU))

### Separate the bar from content
The "big mistake pros still make" is a nav bar that blends into content.
- Fix: a 1px border, a different background tint (light gray bar under white screen), or a small soft shadow. Check against the page bg.
Sources: uxpeak ([Top UI/UX Design Tips: Bottom Mobile Navigation Bar](https://www.youtube.com/watch?v=wLJ40GV2XEc))

### Remove navigation the content format does not need
A short-video app plays on open: no episode list on the player, swipe up for next, no scrubber, no "still watching?". The format removed the need for the UI.
- Fix: ask of each nav element, progress bar or control whether the content type needs it. Delete what it does not.
Sources: TimGabe ([How a Chinese Unicorn App Out-Addicts Netflix](https://www.youtube.com/watch?v=7dCZrtH15zc))

### Keep labels plain and placement fixed, content order logical
Same nav position on every page, plain-word labels (Pricing, Docs, Sign in), no layout tricks that get in the way of navigating. Disjointed order, random content and no visual hierarchy make a layout hard to follow.
- Look for: page sections that do not follow the story (problem, solution, proof, CTA), and DOM order that differs from visual order.
Sources: SatoriGraphics ([Master Layout Design In 8 Minutes](https://www.youtube.com/watch?v=DKwSrMYt15g)); SatoriGraphics ([How To Actually Use Layout Design Properly](https://www.youtube.com/watch?v=q4_jHQru_LQ))

### Organize catalogs by use, not audience
Splitting nav into Men and Women for skincare, toys or clothing is reductive; even a "gender neutral" section was only links back to the same items.
- Fix: categorize by product type, use case or fit. Filters can offer fit without gating the category.
Sources: hatchconference ([Systems of Exclusion, Luke Murphy](https://www.youtube.com/watch?v=iLtVIEcHdSo))

### Give category tiles rhythm
A plain list of category names forces reading every row. Color-coded tiles with a clean image are clear in seconds.
- Fix: tile grid with icon and tint for categories or integrations pages.
Sources: uxpeak ([Top 5 Advanced UX/UI Design Tips, Part 3](https://www.youtube.com/watch?v=Xzh8xjimmp8))

### Redirect on every URL change and fix dead links fast
When a route is renamed or a page deleted, add a 301 redirect or update or remove the link. Crawl internal links for 404s.
Sources: SelfMadeWebDesigner ([50 Web Design Tips & Tricks](https://www.youtube.com/watch?v=rRFD6tENX2U)); SelfMadeWebDesigner ([How to Be A Web Designer in 2026](https://www.youtube.com/watch?v=vYvzOyTA2z4))

### Write the title and meta description as the search preview
They are what people see before clicking. Set a unique `<title>` and meta description per page that state the benefit. Pick heading level by structure, not by visual size, and let the outline be skimmable.
Sources: SelfMadeWebDesigner ([How to Be A Web Designer in 2026](https://www.youtube.com/watch?v=vYvzOyTA2z4)); SelfMadeWebDesigner ([50 Web Design Tips & Tricks](https://www.youtube.com/watch?v=rRFD6tENX2U))

## Where designers disagree

### Short onboarding or long quiz
Most sources: default to as short as possible, defer data and reach value in the first 60 seconds or 5 screens. TimGabe ([The Twisted Psychology Behind Top 1% Apps](https://www.youtube.com/watch?v=nQKWYmrixCU)) and the Cal AI and Noom examples argue a long personalized quiz raises perceived value of the result. Reconcile: long only when each answer changes the first screen or filters for real pain.

### Show the step count or hide it
Progress bars relieve users and use goal-gradient. But with 12 steps and no value yet, Typeform hides the count. Show it up to about 5 steps, hide totals beyond that.

### Reveal fees early or late
TimGabe ([I Redesigned a Neobank App](https://www.youtube.com/watch?v=0GMQRCnOQmo)) cites StubHub: hiding fees until checkout lifted purchase 14%, then argues it burns repeat trust. Treat the lift as a short-term win and show the cost up front.

### Ask for data early or build before the wall
Several sources say defer personal data until after value. The astrology-style example gathers birth data before the reveal. Defer by default, ask early only when the input visibly shapes the result.
