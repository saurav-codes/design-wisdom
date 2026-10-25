# Audit Playbook

Runnable audit and critique moves for a real web app: perception passes on screenshots, first-time-user simulations, break-it passes, flow walks, cross-screen comparisons, measured scans, and self-critique loops. Open it when reviewing a built screen or flow, or when you need a repeatable way to find what is wrong before you fix it.

## Perception passes on a screenshot

### Blur and squint the page
Screenshot the page, apply `filter: blur(4px)` to `blur(8px)` in devtools (or view at 25% zoom, or squint). You should see shapes, not words. In one demo the headline and button survived but the email field vanished, and a filled input background fixed it.
- Look for: H1 and primary CTA are the two strongest shapes; the CTA is among the top 2-3 blobs; 3-5 clear clusters appear from gaps alone; no hot spot darker or lighter than the rest; no one-sided empty area; low-contrast chips, ghost buttons and pale text that disappear. Faces and high-contrast color pull the eye hardest, so check they are not pulling away from the CTA.
- Fix: raise contrast, add a filled background to the weak control, change size or weight, tighten spacing inside groups and widen it between groups. Do not add decoration or arrows. Fix spacing before touching color or borders.
Sources: SelfMadeWebDesigner ([9 Web Design Hacks I Wish I Knew Years Ago](https://www.youtube.com/watch?v=TeMtV8BaZt0)); SatoriGraphics ([PERFECT LAYOUT DESIGN Step by Step](https://www.youtube.com/watch?v=eiV7E_LVlxs)); SatoriGraphics ([Graphic Design Principles Master-Class! (Ep 1 White Space)](https://www.youtube.com/watch?v=FDFD2-poyGw)); willpatersondesign ([5 tips to INSTANTLY up your DESIGN GAME](https://www.youtube.com/watch?v=9epeFitJIoE))

### Rank-order test: write the intended 1-2-3, then see what wins
Before looking, write what the viewer should see first, second and third (for example headline, proof, CTA). Then screenshot, blur or shrink to a thumbnail and name the first three things your eye lands on, out loud. If two things compete for first, demote one. The end of the path should be the primary CTA or key data, not a decoration.
- Look for: nav, logo, badge or illustration winning over the headline; an oversized logo or all-caps menu pulling attention; content stuck in the four corners with an empty middle (traps the eye); key info in the bottom-left, the least read area; a path that stalls, loops or darts.
- Fix: change size, weight, color or space of the wrong element. Shrink nav links and logo, use sentence case or lighter weight for menu items, keep login and sign-up buttons smaller than the hero CTA.
Sources: SatoriGraphics ([The Beginner's Guide To Visual Hierarchy](https://www.youtube.com/watch?v=kK1TOpI948o)); SatoriGraphics ([MASTER Hierarchy For Non-Amateur Graphic Designs In 2026](https://www.youtube.com/watch?v=ZZKHTk_31ik)); DesignSpo ([PRO Vs AMATEUR Website Design (With Examples)](https://www.youtube.com/watch?v=x8Vp8k3jXaA)); DesignSpo ([How to Make Your Website Look PROFESSIONAL](https://www.youtube.com/watch?v=jtjOJkmnzs8))

### Label every element tier 1, 2 or 3
Split the screen into zones. In each zone mark the headline and main image as tier 1, subheads, secondary graphics, nav and logo as tier 2, body and small details as tier 3. Exactly one thing per zone may have the biggest size, weight and color contrast.
- Look for: two tier-1 elements in one zone; on cards and rows, title, rating, price and meta all sharing one size and one gray.
- Fix: make one thing biggest (name, number, rating) and push the rest smaller, lighter or muted. Compare computed font-size and color of title vs meta; they must not match.
Sources: SatoriGraphics ([Master 5 Design Principles With This Course! (MUST WATCH)](https://www.youtube.com/watch?v=FpwZTl3dCZE)); uxpeak ([$42K vs $297K UX/UI Design: The Difference Is HUGE](https://www.youtube.com/watch?v=U7jTCgIWS4w))

### Grayscale pass
Set `filter: grayscale(1)` on `html` and scan every screen. Headings, CTAs, key numbers, charts and status states must stand out without hue. Color should reinforce hierarchy, not rescue it.
- Look for: a muted-gray button next to a gray card that look identical; text on tinted buttons, badges and muted captions that merge with their background; status shown only by color.
- Fix: widen the lightness gap, not the hue. Add an icon or text for status.
Sources: SatoriGraphics ([Graphic Design Principles Master Class! (Advanced Colour Theory)](https://www.youtube.com/watch?v=HonJiqr7eqY)); willpatersondesign ([How to Choose The RIGHT Brand Colors?](https://www.youtube.com/watch?v=BdJTnYqhaZQ)); SatoriGraphics ([Elevate Your Graphic Designs With These Simple Color Fixes!](https://www.youtube.com/watch?v=U9Kl3rMAfFI))

### Shrink after the contrast checker passes
A pair can pass WCAG and still be unreadable when small. Scale the page to 50% and 25%, view it on a phone, and view it in grayscale. Mid-tone on mid-tone looks distinct at full size and merges when small. In devtools the element picker tooltip shows the ratio for any text you hover.
- Look for: muted gray text, placeholder text, disabled states, text on images.
- Fix: darken the text or lighten the background. Avoid mid-tone on mid-tone.
Sources: SatoriGraphics ([Elevate Your Graphic Designs With These Simple Color Fixes!](https://www.youtube.com/watch?v=U9Kl3rMAfFI)); SelfMadeWebDesigner ([The Only 5 Web Design Skills That Actually Matter (2026)](https://www.youtube.com/watch?v=vbFn0C-pvis))

### Review at two scales: 33% for the whole, 100-200% for details
Keep a zoomed-out full-page screenshot (about 10-33%) beside the live 100-200% view. Judge hierarchy and page rhythm on the first, spacing and alignment on the second, and check after every detail edit that the whole still holds. Beginners polish micro and never zoom out. Also picture a phone held at arm's length: the headline and primary action must survive, fine detail may not.
- Look for: clipped icons, rough image edges, misaligned details at 200%; a decorative item winning at 33%; letter gaps in a big heading that look bigger or smaller than the rest.
- Fix: shrink or mute the winner, nudge `letter-spacing`, then re-check at 33%.
Sources: SatoriGraphics ([The ONLY Video That Will Make You A Better Designer In ONE DAY!](https://www.youtube.com/watch?v=exYfWADm-Ns)); willpatersondesign ([Secret Techniques for Creating Eye-Catching Posters](https://www.youtube.com/watch?v=6at6VQD6iVQ)); SatoriGraphics ([Why Your Designs Still Look Amateur (And How Pros Think Differently)](https://www.youtube.com/watch?v=UtEnQCWd0m4))

### Flip the page to see weight, not words
Apply `transform: scaleX(-1)` (or `scaleY(-1)` on a big headline) to a screenshot or the page. You stop reading and see masses, so uneven gaps, heavy corners and off-center items jump out. Circle each one, then decide which to fix.
- Look for: lopsided weight, off-center hero, unequal gaps, one element heavier than its siblings, wobbly nav or card rows, icon misalignment.
- Fix: rebalance the heavy side with a counterweight (a stat, caption or divider), equalize gaps, nudge optically.
Sources: willpatersondesign ([How Professional Designers Test Logos](https://www.youtube.com/watch?v=j299fIs_fMI)); willpatersondesign ([3 PROVEN Typography Methods to Fix Your Design](https://www.youtube.com/watch?v=MFUXBlnTS5Y)); willpatersondesign ([Logo Design Process #2](https://www.youtube.com/watch?v=BLlsk3RZZ_g))

### Balance checks: center line, cover-up, invisible box
Draw a vertical line down the middle of a hero or split layout and weigh both halves (image, big type, color blocks). For an intentionally lopsided layout, cover one side and check the other still feels anchored. Outline a lockup (logo plus nav, image plus text) and check equal breathing room on opposing sides.
- Look for: a heavy image with a light headline opposite; a big empty side with no counterweight (tension turns into confusion); one piece sticking out of the box.
- Fix: add a small stat, caption or divider on the empty side; equalize padding around the group.
Sources: willpatersondesign ([How To Create STUNNING Layouts - 5 Tips](https://www.youtube.com/watch?v=9JiKfJdXZWU)); SatoriGraphics ([Graphic Design Principles Master-Class! (Ep 1 White Space)](https://www.youtube.com/watch?v=FDFD2-poyGw)); willpatersondesign ([Logo Hack: The Trick That Changed Everything](https://www.youtube.com/watch?v=kVLw_eZNhyw))

### Test in real context and at the smallest real size
Never judge a logo, icon, card or hero alone on a blank canvas. Screenshot it inside the real page, in dark mode, on a phone, on a busy background, in a browser tab, in an email header and in the social share card. For marks and thin-line icons, render at 16, 24, 32 and 48px (about 57% per step) plus the app-icon size, and in one color.
- Look for: gaps between shapes that close up, thin strokes that vanish, gradient or shadow doing the work of the shape, a palette that works on white but fails on the product.
- Fix: thicken strokes, widen small gaps, ship a simplified small variant, drop detail that needs contrast tricks.
Sources: willpatersondesign ([I Paid 5 Designers to Brand the Same Food Truck](https://www.youtube.com/watch?v=1ujCESMLLME)); SatoriGraphics ([The FULL Guide To Logo Design Rules (2026)](https://www.youtube.com/watch?v=g2bSztQ_Q7g)); willpatersondesign ([Reviewing INSANE Subscriber LOGO Designs! Ep 17](https://www.youtube.com/watch?v=V0ye52TRGYo)); SatoriGraphics ([How To Train Your Graphic Design Eye To Beat AI in 2026!](https://www.youtube.com/watch?v=-KIWKgxu8cw))

## First-time-user simulations

### Four-question fresh-eyes review of the first load
Give the first-load screenshot (desktop and about 390px wide) to someone who knows little about the product, or simulate that with no prior knowledge. Ask: is the headline understandable right away, is it clear what the site is about, do you know what to do next, does it look good on mobile. Fail the page if any answer is no or "I would have to scroll to know". The cause is the curse of knowledge: after long work you cannot see what is obvious to newcomers.
Sources: SelfMadeWebDesigner ([The Easiest Way to Build Killer Websites](https://www.youtube.com/watch?v=O7MaPnRy5Us))

### Cold-read test with no brief
Show the screen, hero or icon with no copy and one sentence of context at most. Ask what the product is, who it is for, and what they would click first. If they guess the wrong category (a betting app, a restaurant, a dating app), the visual signal is wrong. Also ask what the icon or illustration looks like by accident, and rotate or flip it.
- Look for: icons that read as another letter, another brand or something rude; imagery from the wrong category.
- Fix: change imagery, color, shape or headline until the cold guess is right.
Sources: willpatersondesign ([I Paid 5 Designers to Brand the Same Food Truck](https://www.youtube.com/watch?v=1ujCESMLLME)); willpatersondesign ([Reviewing UNREAL Subscriber LOGO Designs! Ep 21](https://www.youtube.com/watch?v=FJsdWxs-B5Q)); willpatersondesign ([Logo Design Process 2014](https://www.youtube.com/watch?v=Ca0HOtVoO5Y))

### Five-second and three-second recall
Show a screen for 3-5 seconds, hide it, then ask for what they remember, in order. Judge the sequence, not the details. A wrong first item means the hierarchy failed, a missed CTA means the layout did not guide them, and needing to explain the design means it failed. A variant: show it for 10 seconds, return hours later, and ask for 3 words and 1 color they remember.
- Look for: first remembered item is not the headline or value; CTA not remembered; scattered answers on words and color (palette too wide).
- Fix: change order with size, weight, color and space, not extra text. Reduce the palette and repeat the key shape.
Sources: SatoriGraphics ([The ONLY Video You Need To Learn High-Level Design Thinking](https://www.youtube.com/watch?v=VzQl1Tl_LPM)); SatoriGraphics ([The Difference Between Amateur and Pro Designers Is Brutal](https://www.youtube.com/watch?v=CMv2vrpgp0w)); SatoriGraphics ([FULL Graphic Design Course - Using Principles On Actual Designs!](https://www.youtube.com/watch?v=I4C-Smqsf7Y)); SelfMadeWebDesigner ([11 years of web design knowledge in 7 minutes](https://www.youtube.com/watch?v=ityZtG3FMgw))

### First-impression trust check
Open the page cold, look for 3 seconds, then write what it is, who it is for and what to do next. TimGabe cites: people form impressions in 50 ms and decide on trust in under 3 s, mostly from visual design, and a bad first impression can scare off 20-30% of new users. Ask: trust builder or trust killer.
- Look for: clutter, weak hierarchy, inconsistent spacing, cheap or random imagery, copy that does not state the outcome.
- Fix, in this order: clean hierarchy, generous spacing, imagery that supports the headline, balanced type, outcome-focused copy.
Sources: TimGabe ([Give Me 13 Minutes & I'll Grow Your App](https://www.youtube.com/watch?v=v1f9iYZ2GhQ))

### Think-aloud with a stranger, then one task
Find someone unrelated to the project. Have them scroll the page and say aloud what they see, feel and want to do next. Then give one concrete task (change your plan, invite a teammate, book a call) and stay silent. If you simulate this yourself, log every hesitation, wrong click and re-read, and flag every button you thought was obvious that they missed.
- Look for: assumptions you did not know you had; hesitation points on the path.
- Fix: the hesitation points first.
Sources: SelfMadeWebDesigner ([How to Be A Web Designer in 2026 (Free Resources & My Best Advice)](https://www.youtube.com/watch?v=vYvzOyTA2z4)); SelfMadeWebDesigner ([11 Years of Brutally Honest Web Design Advice in 7 Minutes](https://www.youtube.com/watch?v=WxZHUe8mvhU))

### Five users, silent, then look for patterns
Give about five target users a staging link and one task. Do not explain or defend. Let the prototype and the tester talk while you observe, and watch where they struggle, smile or ignore the button you loved. Tell them "we are not testing you". Fix what 3 or more hit before testing again. If three users get stuck on the same screen it is a design defect, not user error. Expert bias hides it from the builder.
- Look for: rage-clicks, backtracking, hesitation. Survey scores can be off the chart while recordings show rage-clicking, so combine what they say with what they do.
Sources: amirmoradiUX ([Stop Designing Features Nobody Wants](https://www.youtube.com/watch?v=S60C_F1FSk4)); Hatch Conference ([Samuel Huber - Prototyping for the Planet](https://www.youtube.com/watch?v=Bsvw9hm3FtY)); Hatch Conference ([Jason Giles - Leading with Empathy](https://www.youtube.com/watch?v=1CeXDNJTHXE)); Jaime Levy ([Getting Lost in Discovery](https://www.youtube.com/watch?v=WwrgZ0hYa9A))

### Ask about past behavior, not opinions
When collecting feedback: "tell me about the last time you did X", "what confused you", "what made you hesitate". Not "would you use this" or "what feature do you want". Analytics shows what, interviews show why. Keep a short clip of a user struggling as evidence.
Sources: amirmoradiUX ([How to Become a Product Designer in the AI Era [Full Course]](https://www.youtube.com/watch?v=ky_F3jdnT4Y)); amirmoradiUX ([Why My Designs Kept Failing (Even When They Looked Good)](https://www.youtube.com/watch?v=Bh0KK5xQOGo))

### Test as the tired scroller
Picture someone on a phone in the evening, tired, brightness low, not zooming. Check the page at low brightness on a phone. Hierarchy and CTA must read without effort.
Sources: SatoriGraphics ([The ONLY Video That Will Make You A Better Designer In ONE DAY!](https://www.youtube.com/watch?v=exYfWADm-Ns))

## Break-it passes

### Break it on purpose
Turn the network off mid-flow, fail a payment, empty every list, hit a usage limit. Design those states as carefully as success screens. TimGabe cites: a 2018 survey where one bad experience is enough for about a third of people to leave. Few teams do this, so it is a cheap place to buy a premium feel.
- Look for: dead ends, raw error codes, blank screens, lost input. Do it in devtools: throttle to offline, mock a 402 or 500 on checkout, seed empty data, screenshot each state.
- Fix: every state says what happened, what to do next, and gives a way out.
Sources: TimGabe ([The Psychology of Premium Apps](https://www.youtube.com/watch?v=8EAYZe6y3I8))

### Play the flow like a user, failure paths included
Do not accept a generated flow by looking at it. Add an item, change the quantity, go back and edit, press the back button, then force a failed payment. Ask: does it remember what I entered, do I always know what is happening, can I recover? Check against real business rules too (for example, cancel only allowed before processing starts).
Sources: amirmoradiUX ([How to Become a Product Designer in the AI Era [Full Course]](https://www.youtube.com/watch?v=ky_F3jdnT4Y))

### Stress with ugly real content
Components look fine with perfect sample data. Seed rows and cards with: a 60+ char name, 3x longer titles, empty descriptions, 1-word and 12-word and 80-character-no-space strings, a missing image, a tall image, a 2-line error. Then try 200% browser zoom and a 320px viewport. It must look fine completely full and nearly empty. Fix the component, not the page.
- Look for: clipping, overlap, layout jumps, unequal card heights, a caption whose owner is unclear.
- Fix: `min-width: 0`, `overflow-wrap: anywhere`, line clamps, aspect-ratio boxes. Make the gap between a caption and its own image smaller than the gap to the next item.
Sources: amirmoradiUX ([How to Become a Product Designer in the AI Era [Full Course]](https://www.youtube.com/watch?v=ky_F3jdnT4Y)); SelfMadeWebDesigner ([33 UNIQUE Website Layouts with Real World Project Examples](https://www.youtube.com/watch?v=nZ2BJt9PgKE)); Brad Frost ([Is Atomic Design Dead? - Hatch Conference Berlin 2023](https://www.youtube.com/watch?v=PK_PICNTgAg))

### Render a state matrix per page
Make a table of role x data volume x auth (logged out, logged in, user, admin, new, experienced, empty, full) and screenshot each cell. Do not check only the happy state.
- Look for: dead space in the new-user state, clutter in the power-user state.
Sources: Brad Frost ([Is Atomic Design Dead? - Hatch Conference Berlin 2023](https://www.youtube.com/watch?v=PK_PICNTgAg))

### Design the gap between click and result
Beginners polish the button; pros design what happens after the click. For each primary action (pay, deploy, import, invite) list what the user sees during, after success, after failure and after a delay. A missing item is a gap.
Sources: amirmoradiUX ([What I Wish I Knew Before 10 Years in UX (The 3 Levels)](https://www.youtube.com/watch?v=gr0Val2QSbM))

### Three-question flow walk
At each step of the core flow confirm the user knows: what just happened, how to take it back, what to do next. This catches what generated UIs skip: system status, undo, recovery. Nielsen's #1 (visibility of system status) and #5 (error prevention) catch most SaaS bugs.
- Look for: save, delete, pay or invite with no visible confirmation, no undo or cancel, or no next step.
- Fix: progress, success confirmation, disabled-while-submitting, confirm or undo for destructive actions.
Sources: TimGabe ([The Psychology of Premium Apps](https://www.youtube.com/watch?v=8EAYZe6y3I8)); Wolfgang Bremer ([Human Centered Leadership](https://www.youtube.com/watch?v=WJQK1w8Tvz4))

### Hunt first-use dead ends on the core feature
Try the core action the lazy way: tiny input, test input, empty input. In one case study users tapped record to test the mic, spoke about 20 seconds, hit a "not long enough, needs 10 minutes" wall and never returned (founder guessed about 10% of downloads lost). First contact with the core feature sets trust for everything after.
- Fix: replace the wall with a demo or real sample output, or move the test into onboarding where motivation is high.
Sources: TimGabe ([How Top 1% Apps Earn Your Second Visit](https://www.youtube.com/watch?v=YA3QpYIKqNI))

### No-vision and extreme-user drill
Set screen brightness to zero, or use only a screen reader and keyboard, and finish sign-up, checkout and error recovery. Note every moment where the only signal was color, an icon or a visual-only toast. Do not review only for the average user (the fighter-seat study: seats built from the average of about 4,000 pilots fit nobody). Review big text, small phone, slow network, color-blind, one hand, keyboard only.
- Fix: add a second channel (text, sound, haptic, aria-live message). Success, error and loading states announced via `aria-live` or `role="status"`. Prefer user-adjustable settings (text size, reduced motion, density) over one fixed default.
Sources: Hatch Conference ([Natalia Filvarova - Embrace Multisensory & Accessible Design](https://www.youtube.com/watch?v=OjlSIq29YzM))

### Mobile overflow and real-device check
DevTools device mode can look perfect while a real iPhone breaks. Load each page at 375px and check `document.documentElement.scrollWidth > innerWidth` (accidental horizontal scroll), body text size, intro animation length, and throttle CPU and network to find effects that stutter. Also view the published page, not the editor, at tall, short and very wide viewports.
- Look for: viewport-unit bugs, fixed bars, safe areas, tap targets, a hero that cuts off on short screens or shows next-section content on huge ones.
Sources: TimGabe ([6 Stunning Websites For UI/UX Inspiration](https://www.youtube.com/watch?v=evhZQg2NHfo)); SelfMadeWebDesigner ([50 Web Design Tips & Tricks to Level Up Instantly](https://www.youtube.com/watch?v=rRFD6tENX2U)); TimGabe ([Learn Framer For Beginners: Mini Course (2024)](https://www.youtube.com/watch?v=wgMgje60Ovw))

### Diff and history views show old to new
Figma's version compare says "position, rotation or scale changed" without saying which, which is the opposite of comfort. In audit logs, version history, settings change logs and review screens, list each field with its before and after value. Never show only "something changed".
Sources: Hatch Conference ([Henrique Gusso - Wise: Designing with the Precision of Code](https://www.youtube.com/watch?v=BHlWX9HeTtM))

## Flow and journey walks

### Walk sign-up to first success and hunt micro-friction
Click through signup, onboarding and the first task as a new user. At each step ask: where does a user pause, get confused, or do something the product could do for them? Count taps from landing to first value, list every extra click, blank field, interstitial and empty screen, then pick the 1-3 worst.
- Look for: each tap, extra screen or "Are you sure?" is a moment to quit.
- Fix: autofilled forms with smart defaults, one-click common actions, dashboards pre-filled with sample data instead of empty states, optional choices that default, confirmations only where they protect against a real mistake.
Sources: TimGabe ([How Netflix Made Us All Binge (Design Breakdown)](https://www.youtube.com/watch?v=hIm3d3JAsPw)); TimGabe ([How a Chinese Unicorn App 'Out-Addicts' Netflix](https://www.youtube.com/watch?v=7dCZrtH15zc))

### Walk the flow backwards from the goal
Start at the end state (payment confirmation, thank-you page) and walk back to where the user enters. Trace each conversion path in reverse: landing to signup to first value, upgrade to billing to confirmation. Every screen must offer one clear next action and no dead ends.
Sources: SelfMadeWebDesigner ([How to Be A Web Designer in 2026 (Free Resources & My Best Advice)](https://www.youtube.com/watch?v=vYvzOyTA2z4))

### Journey map the slow, stressful and silent moments
List the screens in order from signup to the end of the main loop. Mark waits, long forms, errors and empty states. For each marked step ask where the user slows, where stress peaks, where it is silent or empty, and give it a deliberate design. Negative moments are as memorable as positive ones.
- Fix: a one-line reassurance, progress hint or inline help on each long form or slow step, added before the user has to ask.
Sources: TimGabe ([The Tiny Design Rule Behind Top 1% Apps](https://www.youtube.com/watch?v=11h4H3TAGkM))

### Walk filters and wizards with a tap counter
Count taps and note what disappears after each step. A one-filter-per-page flow took 7 taps for two filters, and each new page hid earlier choices, so users could not see trade-offs.
- Fix: if interacting choices sit on separate screens, merge them into one scrollable panel. For data-entry screens, add instant feedback that reacts as the user chooses (a summary, a comparison with last time, a tip).
Sources: uxpeak ([$42K vs $297K UX/UI Design: The Difference Is HUGE](https://www.youtube.com/watch?v=U7jTCgIWS4w)); uxpeak ([This Video Will Take You From Junior to Senior UX/UI Designer](https://www.youtube.com/watch?v=YlN28RNChl0))

### Time the golden tasks and benchmark before and after
Pick 3-5 core tasks (sign up, invite a teammate, upgrade plan, export). Record clicks, seconds, errors and satisfaction for each, then re-count after changes. Mews cites: time on task for the most frequent golden tasks fell over 46% in 12 months. UserTesting cites: a QX score rose 8 points after launching a surveys feature, with 36% more platform usage in the first four months and 25% feature adoption.
Sources: Hatch Conference ([The Path to zero Screens - Juan Hidalgo](https://www.youtube.com/watch?v=Fb7XJo0EyaE)); Jason Giles ([How UserTesting does user testing on UserTesting](https://www.youtube.com/watch?v=X-Fqc1t_gE4))

### Dogfood the whole launch path on the real deploy
Fill every contact form, buy the products, sign up for every lead magnet, run password reset, and confirm the emails arrive, redirects fire and success states show. Do it before launch, not after pulling the site back.
Sources: SelfMadeWebDesigner ([Complete Web Design Process: What Took Me 10 Years to Learn in 12 Minutes](https://www.youtube.com/watch?v=T5JglDcd54A))

### Read the funnel and recordings for what users already work around
Look for the step users retry or abandon, then question whether the step should exist, not just how to style it. Hotjar recordings showed users failing to enter passwords, support confirmed it was the top complaint, and a back-end dev asked "why passwords at all?". The fix was password-less login. Netflix saw that 15% of viewers fast-forwarded past intros, added Skip Intro, and (TimGabe cites) it gets 136 million presses a day.
- Look for: repeated manual steps (scrubbing, copy-pasting, repeating a step). A high onboarding completion rate can mean high-intent users: compare "finished onboarding" with "completed first core action". In one case study half the finishers never used the core feature.
- Fix: a shortcut button for the workaround; spend polish budget on the weakest screen at the moment users come back unprompted (case study: median 10 minutes after a therapy session ended, where the recap screen was a text block and a "see full recap" button).
Sources: Hatch Conference ([Death to Handovers! - Hatch Conference 2023](https://www.youtube.com/watch?v=NfC0mRzFZMs)); TimGabe ([How Netflix Made Us All Binge (Design Breakdown)](https://www.youtube.com/watch?v=hIm3d3JAsPw)); TimGabe ([How Top 1% Apps Earn Your Second Visit](https://www.youtube.com/watch?v=YA3QpYIKqNI))

### Benchmark your own surfaces against each other
Compare mobile web with the native app, desktop and the best competitor, and report the gap as numbers. Airbnb's team found mobile web loaded in 7.3s vs 2.4s for a competitor, which justified funding a redesign. A "responsive so it is free" mobile view nobody optimized is the usual culprit.
Sources: Hatch Conference ([Why Designers Struggle in This Economy and What to Do About It](https://www.youtube.com/watch?v=FIUsadeMdoE))

### Ask the exit question
Can a user finish the product and hit a ceiling? If a user left today for a competitor, what would they have to rebuild from scratch? If the answer is "nothing much", there is no investment layer.
- Fix: list what each user has deposited (settings, history, rules, integrations) and make it visible; add compounding metrics or periodic resets that keep earned status.
Sources: TimGabe ([How To Scientifically Design Addictive Apps](https://www.youtube.com/watch?v=yBpv5rZoBjA)); TimGabe ([The New Way Apps Dominate in 2026](https://www.youtube.com/watch?v=yYs7iv81Ppk))

## Cross-screen and cross-surface comparison

### Compare screen 1 with screen 80
Teams review one happy-path screen at a time, but users live with all of them side by side. Screenshot every screen of one flow next to each other. TimGabe cites: a 2009 University of York study where moving a nav bar from left to right more than doubled time on page, and users still said it did not slow them down.
- Look for: nav position, header style, card style, button hierarchy and copy tone that differ without a reason.
- Fix: unify, as one shared pattern, not screen by screen.
Sources: TimGabe ([The Psychology of Premium Apps](https://www.youtube.com/watch?v=8EAYZe6y3I8))

### Use the product for an hour and log where it stops feeling like one product
Click through the main flows as a daily user. List different empty states, different wording for the same event, odd spacing, mismatched badge styles and limit messages. Fixes are small copy and layout decisions repeated across hundreds of places, and no component library hands them to you. Keep a frustration notepad too, since frustration is often a flourish that stopped the page doing its job (broken scroll, odd navigation).
Sources: TimGabe ([The Psychology of Premium Apps](https://www.youtube.com/watch?v=8EAYZe6y3I8)); SelfMadeWebDesigner ([How to Keep Your Creative Edge as a Web Designer](https://www.youtube.com/watch?v=E9i-NgImx8c))

### Billboard-to-button: landing page vs logged-in app
Walk the journey in order: marketing page, site, signup, first use, support and cancel flows. Open the landing page and the app side by side and compare type, color, radius, illustration and tone of voice. Dropbox did this after a bold rebrand and ended up toning the brand down and raising product expression so both felt like one thing.
- Look for: a lively landing page over gray-table dashboards.
- Fix: carry the brand accent, type and copy voice into the app shell, empty states and emails.
Sources: Hatch Conference ([Designing the Design Process: Lessons from Grammarly's VP of Design](https://www.youtube.com/watch?v=6UcZ8pyYakg)); Hatch Conference ([Building design systems that work for your whole Organisation - Sarrah Vesselov](https://www.youtube.com/watch?v=2ljl0aUdcpg))

### Raise the weakest page to the landing page standard
Reviewers look for reasons not to buy. FAQ, contact, billing, settings, case-study and empty-state pages usually get far less effort, which costs trust. Screenshot the least-visited pages and compare them to the landing page. Check that color, type, imagery and voice stay consistent on settings and billing too.
Sources: DesignSpo ([$1,000,000 Design Portfolios](https://www.youtube.com/watch?v=DaeEKKSpgXU)); DesignSpo ([PRO Vs AMATEUR Website Layouts (With Examples)](https://www.youtube.com/watch?v=L0Pk3OVbxRU))

### Audit end to end and tag each issue by layer
Build a table of screens with columns for three layers: feature (missing on another platform), ergonomic (same task, different path, for example "My trips" reached differently in app and web), stylistic (visual, tone, motion). Score each issue high, medium or low on visibility, effort and conversion. Fix the high-visibility, low-effort ones first.
- Look for: a feature in the app that is missing on web; nav labels and routes for the same object that differ; buttons, tone and spacing that differ.
Sources: Hatch Conference ([How Design Moves Revenue, Retention, and Market Share at Skyscanner](https://www.youtube.com/watch?v=5yJYLrbvOYY))

### Inventory duplicate components before adding features
One team found the "one" primary button existed in at least 10 variants across products. A design system started on top of that chaos does not fix it. Grep the codebase for button, input and card implementations (styled variants, one-off classes, inline styles). If you find more than one primary button style, merge them into one component first.
Sources: Hatch Conference ([Death to Handovers! - Hatch Conference 2023](https://www.youtube.com/watch?v=NfC0mRzFZMs))

### Scroll at speed and check for sameness
If the layout repeats section after section, the brain predicts the ending and stops engaging. Three or more sections in a row sharing one structure (icon, title, text in a 3-up grid) is the tell. Fix by changing one to a split image and text, a full-width quote or a table. Also review the page bottom to top: a reversed pass exposes redundant or misaligned things you stopped seeing.
Sources: SelfMadeWebDesigner ([Master Website Layouts in Under 10 Minutes (Video 1)](https://www.youtube.com/watch?v=EF_ucfA3CJs)); SelfMadeWebDesigner ([50 Web Design Tips & Tricks to Level Up Instantly](https://www.youtube.com/watch?v=rRFD6tENX2U))

### Category swap and template teardown
Screenshot 10-20 competitor SaaS heroes, hide the names and check whether yours is distinguishable by layout, color, type or imagery. If it could swap with a competitor, pick one signature element and commit. Read a stock-template teardown in reverse to spot template-looking pages: default fonts, default palette, stock sections you do not need, stock imagery, stock rounded corners, no custom background pattern. Each unchanged item is a generic signal.
Sources: SatoriGraphics ([The FULL Guide To Logo Design Rules (2026)](https://www.youtube.com/watch?v=g2bSztQ_Q7g)); SelfMadeWebDesigner ([The Seismic Shifts Happening In Web Design](https://www.youtube.com/watch?v=oY87jJx4sAI)); TimGabe ([How To Design a $5k Website in 5 Minutes](https://www.youtube.com/watch?v=hCKdIwbhS-s))

### Compare with a best-in-class reference and read its real numbers
Open 1-2 top sites for that page type or flow (billing, onboarding, settings; pull 5-10 real examples). Take their structure and hierarchy, not their look. Then read their real numbers: select an element and open the Computed tab (not Styles, which shows variables and calc) for final font-size, line-height and letter-spacing. Spotify example from the notes: heading 43.43px size and 43.43px line-height (ratio 1), paragraph 24px with 30px line-height, eyebrow letter-spacing 0.6px. The CSS Overview panel (More tools) lists a page's colors, fonts and sizes in use.
- Fix: match the ratios and derive tokens from the reference instead of guessing; adapt to the product's own voice.
Sources: DesignSpo ([PRO Vs AMATEUR Website Design (With Examples)](https://www.youtube.com/watch?v=x8Vp8k3jXaA)); SelfMadeWebDesigner ([9 Web Design Hacks I Wish I Knew Years Ago](https://www.youtube.com/watch?v=TeMtV8BaZt0)); SelfMadeWebDesigner ([The Only 5 Web Design Skills That Actually Matter (2026)](https://www.youtube.com/watch?v=vbFn0C-pvis)); TimGabe ([Design Better Than 99% of UI Designers](https://www.youtube.com/watch?v=PGQnGEH7c-E))

### Put before and after side by side, in context
Screenshot old and new at the same width, then drop both in a realistic frame (browser or phone). Judge first impression plainly (do you trust it more?), then list what was cut, what is now emphasized, and whether the color mood fits the business. Effectiveness shows in context, not on an isolated artboard.
Sources: SatoriGraphics ([Making FAMOUS Graphic Designs Better!? (Before & After Graphic Design Ep7)](https://www.youtube.com/watch?v=INMuAYZDums)); willpatersondesign ([I Secretly Redesigned Local Company Logos](https://www.youtube.com/watch?v=mjtSEWPJIAs))

## Measured consistency scans

### Count what is in use
Count distinct font sizes, weights, families, colors, radii, grays and button heights on a screen and compare with the declared scale. A failing screen had 6 sizes and 4 weights; target 4 sizes and 2 weights. Target 2 font families and about 3 colors plus neutrals.
- Look for: computed font-family outside the declared fonts; a stray bright color used nowhere else; spacing by feel (11px, 13px, 17px, 25px, 33px) off the 4/8 scale; the same gap used between everything ("linear spacing"); title-to-subtitle gap not clearly smaller than block-to-block gap; menu or form inputs in a different font than the rest; headline > subtitle > input and nav size order broken; two shape languages on one screen (4px corners on cards, circles on category images).
- Fix: merge near-duplicates into tokens. Review one screen fully before the next.
Sources: TimGabe ([4 levels of UI/UX design (and BIG mistakes to avoid)](https://www.youtube.com/watch?v=86PGRyQjdzQ)); TimGabe ([Our World Class App Design Formula](https://www.youtube.com/watch?v=wmTkiF23GRQ)); SatoriGraphics ([Beginner VS Advanced Graphic Design (What It Really Looks Like)](https://www.youtube.com/watch?v=wS_eGNASZZY)); DesignSpo ([The Golden Rule Of Web Design (and why you're breaking it)](https://www.youtube.com/watch?v=CASPWJUsHPM))

### Planted-bug scan
Designers catch these instantly, so run the scan on every page: mixed icon families, one icon with a heavier stroke than its row (put all icons on one row at the same size and compare stroke, corner radius and fill), two button sizes in one row, uneven padding and radius, nav items that look disabled but are not, flat icons next to 3D renders, stock photos next to hand art.
- Fix: one icon library, one stroke token, one visual dialect per page.
Sources: Hatch Conference ([Designing the Design Process: Lessons from Grammarly's VP of Design](https://www.youtube.com/watch?v=6UcZ8pyYakg)); willpatersondesign ([I Paid 5 Designers to Brand the Same Food Truck](https://www.youtube.com/watch?v=1ujCESMLLME)); uxpeak ([$42K vs $297K UX/UI Design: The Difference Is HUGE](https://www.youtube.com/watch?v=U7jTCgIWS4w))

### Count the hero and competing elements
In the first viewport count CTAs, text tiers and blocks. Flagged examples: five CTAs, a button bigger than the headline, two different subtitles, a hero split into four blocks. More than 1 primary CTA or more than 2 text tiers means merge or demote.
Sources: DesignSpo ([I redesigned YOUR websites](https://www.youtube.com/watch?v=-F1F4YISY4E)); DesignSpo ([PRO Vs AMATEUR Website Layouts (With Examples)](https://www.youtube.com/watch?v=L0Pk3OVbxRU))

### Heading-tree and text-over-image checks
Extract h1-h6 from the DOM, read only the headings and ask whether the page is still understandable. Do not use h-tags for styled bold labels. Separately, audit every label on a photo or card image: a busy image fights the words.
- Fix: a scrim, a color overlay, a solid backing, lowered image opacity, or grayscale images that turn to color on hover, until text passes contrast.
Sources: Hatch Conference ([Best practices to build Accessible Designs using Figma and annotations](https://www.youtube.com/watch?v=6fHkr3SL51Y)); SelfMadeWebDesigner ([33 UNIQUE Website Layouts with Real World Project Examples](https://www.youtube.com/watch?v=nZ2BJt9PgKE))

### Does the visual show the product?
Ask of each image or illustration whether it shows the actual product in use. Generic stock photos say nothing. A viewer should say "that is clearly this product". Also proof the product name and key words everywhere (grep for spelling variants in title, meta, footer and emails).
- Fix: real product screenshots or custom graphics in hero and feature sections.
Sources: DesignSpo ([How to Make Your Website Look PROFESSIONAL](https://www.youtube.com/watch?v=jtjOJkmnzs8)); willpatersondesign ([Logo Design Subscriber Critique Ep 18](https://www.youtube.com/watch?v=fctkGnnIU_0))

## Intent and subtraction critique

### Hold the screen against a one-sentence goal and metric
Write the page's goal as one sentence ("Start a free trial in under a minute") and the one metric it should move (signup rate, trial start, upgrade click). Then ask whether the thing in the sentence is the most prominent element. If the headline fights the product image or the CTA is tucked in a corner, the hierarchy is wrong. For a landing page, a CTA that appears once is a bug. Say what each page prioritizes: hero is conversion and clarity, docs are readability, dashboard is speed.
Sources: SatoriGraphics ([The ONLY Video You Need To Become A Better Graphic Designer In 2026](https://www.youtube.com/watch?v=ljBtqaX8MIY)); SatoriGraphics ([Change How You Think As A Designer, With Just ONE Video!](https://www.youtube.com/watch?v=4PHzHgDjiu4)); TimGabe ([6 Stunning Websites For UI/UX Inspiration](https://www.youtube.com/watch?v=evhZQg2NHfo)); SelfMadeWebDesigner ([50 Web Design Tips & Tricks to Level Up Instantly](https://www.youtube.com/watch?v=rRFD6tENX2U))

### Write the critique as keep, fix, add, remove
Before editing, write what to keep (real strengths), what to resize or respace, what to add (often social proof) and what to remove (redundant buttons or links). Do not rewrite what already works. For each screen section ask: what choice was made, what problem did it solve, how would I solve it better, what feels odd, what is missing. Order the fixes: too much text, too small, too many sections, competing CTAs, text over faces, low contrast. Most fixes are small tweaks, not rebuilds.
Sources: DesignSpo ([I Redesigned YOUR Websites - Episode. 2](https://www.youtube.com/watch?v=oO8MzIVyiv0)); DesignSpo ([I redesigned YOUR websites](https://www.youtube.com/watch?v=-F1F4YISY4E)); DesignSpo ([PRO Vs AMATEUR Website Layouts (With Examples)](https://www.youtube.com/watch?v=L0Pk3OVbxRU))

### Remove one element at a time and see if the screen still works
In devtools delete dividers, icons, badges, secondary buttons, extra labels and decorative illustrations one at a time. Keep the deletion if nothing is lost. If an element is liked but not needed, demote it instead (smaller, lower contrast, footer corner). Shrink the dominant element slightly to free space. Common wins: stacked dividers, double CTAs, icon plus text plus illustration all saying the same thing, an intro line repeating the headline.
- Look for: when a screen feels weak, the urge to add gradients, borders, badges and shadows first. Remove and tighten before decorating.
- Fix: keep the primary CTA and one hero visual. Do not strip until the brand is no longer recognizable in a glance: simple is not generic.
Sources: willpatersondesign ([The Process Of My New Logo Design - 10,000 Subscribers!](https://www.youtube.com/watch?v=Df6VPHvAs7A)); SatoriGraphics ([How To INSTANTLY Make Your Graphic Design Better! (FAST!)](https://www.youtube.com/watch?v=0SxzNcCrDxE)); willpatersondesign ([Reviewing INTERESTING Subscriber DESIGN work Ep 34](https://www.youtube.com/watch?v=TLRBHvjN3No)); willpatersondesign ([Reviewing MODERN Subscriber LOGO Designs! Ep 22](https://www.youtube.com/watch?v=ZoDNTGQD0SY))

### Ask why of every element
Treat each element as if it pays rent. For each decorative border, gradient, icon, badge or color accent write the one-line reason it exists and what it communicates. "It looks cool" or "the prompt said so" means delete. Also write the principle with its reason ("whitespace around X because Y"); a principle with no reason is decoration. Justify choices aloud as if presenting: why this size, position, color, micro-spacing.
Sources: SatoriGraphics ([How A Graphic Designer MUST Think in 2026 To Survive!](https://www.youtube.com/watch?v=WFkGbyH24AY)); SatoriGraphics ([How To Train Your Graphic Design Eye To Beat AI in 2026!](https://www.youtube.com/watch?v=-KIWKgxu8cw)); SelfMadeWebDesigner ([11 Years of Brutally Honest Web Design Advice in 7 Minutes](https://www.youtube.com/watch?v=WxZHUe8mvhU))

### 90-second hierarchy pass: quiet the unimportant first
On a busy dashboard or pricing page, give yourself 90 seconds and change only font-size, font-weight, color and margin. Decide 1st, 2nd and 3rd, make the headline central, features rhythmic. Build hierarchy by muting rather than boosting: lower contrast, size or opacity of metadata, secondary links and borders before enlarging the main item.
- Look for: if it still reads flat after the pass, there are too many primary elements.
- Fix: keep fine print and helper text in smaller, lower-contrast type below the main content. Do not hide the detail layer, quiet it.
Sources: SatoriGraphics ([The ONLY Video That Will Make You A Better Designer In ONE DAY!](https://www.youtube.com/watch?v=exYfWADm-Ns)); SelfMadeWebDesigner ([50 Web Design Tips & Tricks to Level Up Instantly](https://www.youtube.com/watch?v=rRFD6tENX2U))

### Three-question skim per section
Scroll fast. For each section ask: does the visitor understand what this is, why it matters to them, what to do next? If any answer is no, the section needs better delivery, not more content.
- Fix: rewrite that section's headline and CTA, and delete anything that does not answer one of the three.
Sources: TimGabe ([Give Me 10 Minutes & I'll Boost Your Website Conversions](https://www.youtube.com/watch?v=TIfiy1fodDs))

### Ask what question each element asks the user
Every block quietly asks a question. "Is this worth $19 a month?" makes people leave; "can I try this free?" makes them proceed. Write the implied question per block on paywalls, pricing cards, checkout and booking screens. A screen with correct title, price, dates and button can still be only a form: look for small thumbnails, bare inputs and generic buttons ("Reserve", "Submit").
- Fix: change copy, layout or the number shown so the question is easy; use a large visual, a concrete detail and a button that carries the outcome.
Sources: uxpeak ([Top 3 UX/UI Redesigns That Make You Design Like a Pro](https://www.youtube.com/watch?v=zr37ibqXl1U))

### Check tokens against one emotion and "is not" lines
Write one core emotion (calm, urgency, trust, joy), not five, plus 3-5 "this brand is NOT ..." lines. Review color, font, radius, motion easing and imagery against them. Anything neutral or off gets redone: no round corners on a serious brand, no sharp angles on a friendly one. Before "fixing" something plain or raw, ask whether it is intentional brand voice.
Sources: SatoriGraphics ([Why Your Designs Still Look Amateur (And How Pros Think Differently)](https://www.youtube.com/watch?v=UtEnQCWd0m4)); SatoriGraphics ([The ONLY Video That Will Make You A Better Designer In ONE DAY!](https://www.youtube.com/watch?v=exYfWADm-Ns)); SatoriGraphics ([Is Kanye West BETTER At Graphic Design Than YOU!?](https://www.youtube.com/watch?v=L8Iw1RgXaDs))

## Self-critique and iteration loops

### Reset your eyes before the review pass
After hours on a screen the brain normalizes flaws, and after 50 hours you cannot see your own work. Do the review as a separate step: step away 1-2 hours or overnight, reload, change viewport, try dark mode, grayscale, a real phone or another monitor, scroll bottom to top. Typos, odd alignment, text too small and heavy areas jump out because you now see it like a stranger. Switching device or window size also helps when a review stalls.
Sources: SatoriGraphics ([The ONLY Video That Shows You How Expert Designers Think!](https://www.youtube.com/watch?v=brzjHzzxD0E)); willpatersondesign ([Bad Logos Made Good! Logo Design Process](https://www.youtube.com/watch?v=KY0NHR2eTUQ)); SatoriGraphics ([How To INSTANTLY Make Your Graphic Design Better! (FAST!)](https://www.youtube.com/watch?v=0SxzNcCrDxE)); SelfMadeWebDesigner ([50 Web Design Tips & Tricks to Level Up Instantly](https://www.youtube.com/watch?v=rRFD6tENX2U))

### Get a blind outside read with the goal sentence only
Give a fresh agent or person the goal sentence plus screenshots, with no explanation, and ask only "where does this fail the goal?". If you have to explain the design, it failed. For scoring, have the judge rate the same categories (design, UX, originality, overall) without knowing the build process; blind scoring removes bias. Record repeat offenders (hierarchy, proximity, spacing) as a checklist. Always give context when asking for review: audience, goal, one-sentence product description. Judging without the problem is meaningless.
Sources: SatoriGraphics ([The ONLY Video You Need To Become A Better Graphic Designer In 2026](https://www.youtube.com/watch?v=ljBtqaX8MIY)); SelfMadeWebDesigner ([Let's See Who's Better...Human or AI Web Design](https://www.youtube.com/watch?v=5LW_-J9q9h8)); SatoriGraphics ([The ONLY Typography Video Graphic Designers Need To See!](https://www.youtube.com/watch?v=a4Pj9MAPtuo)); willpatersondesign ([Reviewing Your Designs On Reddit!](https://www.youtube.com/watch?v=mP7OWR1lCb4))

### Score the screen
Two scorecards. Six-point: copy, visuals, color, font sizes, spacing, structure. Beginner screens fail all six (wordy labels, flashy gradients and blur, one loud color, random pixel values, accidental grouping); copy and type sizes are usually the cheapest wins. Three-question 1-5: point of view (does it stand for something), consistency (one system or five stitched apps, and does it hold on screen 100), execution (any real product decision, or only a stock pattern). TimGabe's AI alarm app scored 5/15 as a plain prompt, 8/15 with design vocabulary, 4/15 flooded with references, 15/15 with a human art director. A clean but empty UI is slop; fix by adding one decision, not more components.
Sources: TimGabe ([4 levels of UI/UX design (and BIG mistakes to avoid)](https://www.youtube.com/watch?v=86PGRyQjdzQ)); TimGabe ([The Only Formula Behind Truly Great Apps](https://www.youtube.com/watch?v=YS7uOXjmJTA)); uxpeak ([$42K vs $297K UX/UI Design: The Difference Is HUGE](https://www.youtube.com/watch?v=U7jTCgIWS4w))

### Annotate the screenshot with numbered, specific fixes
Mark up a large screenshot with numbered callouts or red circles (what works, what does not) and a concrete fix per mark, such as "icon 4 px too high" or "gap 12 should be 16". Then fix the circles one by one and keep before and after screenshots to verify each fix. Write critique as instructions ("make the total the biggest number", "give fees their own group", "reduce emphasis on the banner"), never "make it look better".
Sources: willpatersondesign ([Master the Art of Branded Typography](https://www.youtube.com/watch?v=-gSlKmwtEcA)); willpatersondesign ([ScrawlrBox Logo Design Process - Real Client!](https://www.youtube.com/watch?v=WSojTkvDevE)); amirmoradiUX ([How to Become a Product Designer in the AI Era [Full Course]](https://www.youtube.com/watch?v=ky_F3jdnT4Y))

### Record findings as observation, interpretation, action
Three columns: what happened (three users hunting for the delivery fee), what it might mean (they need the total earlier), what to change (show total in basket). Keep them separate since the interpretation may be wrong. Write the readout as screen, problem, fix, evidence, not "simplify and optimize UX". For change notes use signal, cause, change, expected metric: "users dropped after X because Y, so I changed Z".
Sources: amirmoradiUX ([How to Become a Product Designer in the AI Era [Full Course]](https://www.youtube.com/watch?v=ky_F3jdnT4Y)); Jaime Levy ([Getting Lost in Discovery](https://www.youtube.com/watch?v=WwrgZ0hYa9A)); amirmoradiUX ([What Actually Makes You a Senior Designer (After 10 Years in UX)](https://www.youtube.com/watch?v=6OCnMMOdC2I))

### Turn vague feedback into specifics
When a comment is a preference ("I don't like it", "make it pop"), ask why and what it reminds them of. One client rejected an orange and green homepage because the colors reminded her of carrots; fixing by your own taste would have missed that. Ask for specific likes and dislikes in writing. If the requested tweak takes minutes, make it and show before and after side by side. Ask for dislikes first: knowing what is rejected narrows direction faster than what is liked.
Sources: SelfMadeWebDesigner ([How to Build a UX Design Portfolio that Get's You Hired w/ Sarah Doody](https://www.youtube.com/watch?v=XDPZOqMoS9g)); willpatersondesign ([How To Deal With BAD Client Feedback](https://www.youtube.com/watch?v=13Z-pZI1m74)); willpatersondesign ([How I Designed Enter Shikari's New Logo (Full Process)](https://www.youtube.com/watch?v=I-X-W8ZiGYQ))

### Make 3 to 10 rough variants, reject each with a reason
Before polishing the first idea, produce 3 or more clearly different directions (different layout, theme, star element), not three tweaks of one. Include one stripped-down control variant and one stretch variant. Write the specific rejection reason for each; it becomes the next constraint (Linear went through about five layouts for a project page, rejected for dashboard feel, too much on screen, hidden issues, no push to write). The first good layout is often best, but produce two alternatives anyway and compare.
Sources: Hatch Conference ([Adrien Griveau: How Linear designs for Planners](https://www.youtube.com/watch?v=9sJCu7BPvSw)); willpatersondesign ([Logo Design Process: Creating a REAL Client's Logo from Scratch](https://www.youtube.com/watch?v=Umin1iXhsn0)); SelfMadeWebDesigner ([6 EASY Tips to 10x Any Site's Design](https://www.youtube.com/watch?v=pbhLsV-Dyho)); willpatersondesign ([Negative Space Logo Design Process](https://www.youtube.com/watch?v=KnaI8EJtDUc))

### Premortem before sending
Ask where it could go wrong: could it be misread, does the palette work on another background, does the type hold on a small phone. Check dark and light mode, small widths, long strings and a different background behind each component. Name where it will live and what breaks first, otherwise the platform decides for you.
Sources: SatoriGraphics ([Why Your Designs Still Look Amateur (And How Pros Think Differently)](https://www.youtube.com/watch?v=UtEnQCWd0m4)); SatoriGraphics ([The Difference Between Amateur and Pro Designers Is Brutal](https://www.youtube.com/watch?v=CMv2vrpgp0w))

### Rescue a screen that feels off
Run in order: step away, check the basics (alignment, hierarchy, balance, proximity, contrast), restate the goal and the feeling, remove anything with no purpose, and save a copy first so deleting is safe. Typical fixes in the source example: split one lump of text into 3 proximity groups, add one contrasting accent for emphasis, widen margins, move a decorative illustration to a small footer spot. Duplicate before each risky edit and keep the version history.
Sources: SatoriGraphics ([How To INSTANTLY Make Your Graphic Design Better! (FAST!)](https://www.youtube.com/watch?v=0SxzNcCrDxE)); willpatersondesign ([Redesigning Your Logos! (Most Common Mistakes) Ep8](https://www.youtube.com/watch?v=-bwYtTjcjqc))

### Time-box polish and stop at good enough
Experienced designers leave small things unresolved and return later. Time-box polish passes (30 minutes to finish a page, then it is done). Fix hierarchy, spacing and states first and skip pixel-fiddling that does not change comprehension. Drop any choice with no concrete answer to "why". If the page is stuck on a weak element, look for a spark, not a copy.
Sources: SatoriGraphics ([The ONLY Video That Shows You How Expert Designers Think!](https://www.youtube.com/watch?v=brzjHzzxD0E)); SelfMadeWebDesigner ([Master the Creative Process as a Web Designer](https://www.youtube.com/watch?v=PM-Y_EhiOX0))

### Create fast, edit slow: delete, then amplify
After generating many options, delete the obvious and redundant first. Then find the few moments with real power (a bold color use, a good whitespace area, one icon) and amplify them into the design language, repeating that one distinctive moment across screens.
Sources: Hatch Conference ([Cam Worboys: How AI is Redefining the Role of UX and Product Designers](https://www.youtube.com/watch?v=KyOMQJUxQ28))

## Auditing AI-generated screens

### Five-problem checklist for a typical generated form or modal
One example screen had five faults: placeholder text instead of real labels, a tiny close button, an error shown only as a red border with no message, two buttons that both look primary, bottom gray text too light to read.
- Look for: visible labels, close-button tap target, an error message in words, exactly one primary button per view, footnote contrast.
Sources: amirmoradiUX ([How to Become a Product Designer in the AI Era [Full Course]](https://www.youtube.com/watch?v=ky_F3jdnT4Y))

### Component reuse is not good UX: check scope and completeness
Two AI tools reused the right design-system components on a real task and still shipped issues: a missing minus button on a quantity stepper, a weak small CTA with lots of empty space, an invented extra ticket type not in the spec, stray white backgrounds behind sections.
- Look for: anything added that was not asked (diff the UI against the requirement list and remove extras); control completeness (stepper has both + and -, disables at min); CTA weight; leftover background boxes.
Sources: amirmoradiUX ([Figma Agent vs Claude: Which One Designs Better?](https://www.youtube.com/watch?v=wx2ylgMU8WM)); amirmoradiUX ([How I Use AI as a Product Designer (4 Real Workflows)](https://www.youtube.com/watch?v=OEjBGWPvA3I))

### Judge variants on four named criteria
When comparing generated variants (5-50 can appear), score each on hierarchy, spacing, noise and primary-action visibility, then say in one sentence why one wins, naming a concrete cause (hierarchy, spacing, state, honesty). Judging and naming the fix is the skill, not generating the screen.
Sources: amirmoradiUX ([How to Become a Product Designer in the AI Era [Full Course]](https://www.youtube.com/watch?v=ky_F3jdnT4Y))

## Where designers disagree

### Gradients on the signup button
DesignSpo's finishing pass adds a subtle gradient on the signup button, a fading hover shadow and a dotted pattern background in the live build. frontend-design bans gradients of any kind. Follow frontend-design.
Sources: DesignSpo ([How To Build A Website From Start To Finish (FULL PROCESS)](https://www.youtube.com/watch?v=b2TP7K9ZFWk))

### Design system first or extract it later
TimGabe says do not start with a design system: design freely and extract tokens and components on second or third reuse, building variants only when needed. frontend-design says write a token plan before building. For a new surface, write the small token plan and still extract components only when something repeats.
Sources: TimGabe ([Your First Design System in Figma (Beginner Tutorial)](https://www.youtube.com/watch?v=_uva2dQPlV8))

### Review once or review again after a break
Several sources want the review in a separate pass after hours or overnight, with a fresh reviewer, and repeated rounds. frontend-design says verify in bounded passes (one batched round, at most one more) and stop. Run the break-and-fresh-eyes pass once, time-boxed, rather than open-ended.
Sources: SatoriGraphics ([The ONLY Video That Shows You How Expert Designers Think!](https://www.youtube.com/watch?v=brzjHzzxD0E)); SelfMadeWebDesigner ([Master the Creative Process as a Web Designer](https://www.youtube.com/watch?v=PM-Y_EhiOX0))
