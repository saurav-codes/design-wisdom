# Hierarchy, Layout, Spacing and Responsive Layout

Open this when a screen feels flat, crowded, off, or "templated", or before laying out a landing page, dashboard, settings or billing screen. It adds tactics and numbers on top of frontend-design. Open it for review passes too.

## Diagnose first (tactics before polish)

### Rank the content 1-2-3 before you style anything
Sort every element in a section into primary, secondary, tertiary. Then encode the rank with size, position and contrast. Exactly one element is level 1. Pricing: plan name and price primary, feature highlights secondary, fine print tertiary. Event-style content: the key info (date, price, total) may outrank the headline, so rank by what the user needs, not by what is easiest to enlarge.
- Look for: two elements at the same size and weight competing for first read; a promo banner louder than the amount due.
- Fix: write the ranked list in the plan, then check the rendered page gives the top item the strongest weight. Demote the loser by size, weight or tone.
Sources: SatoriGraphics ([The Layout Design Workflows You Need](https://www.youtube.com/watch?v=Uz3B2u9Ug8o)); uxpeak ([Top 5 UX/UI Design Tips, part 1](https://www.youtube.com/watch?v=8pMUkEbAM7g)); DesignSpo ([How to Make Your Website Look PROFESSIONAL](https://www.youtube.com/watch?v=jtjOJkmnzs8))

### Ask three flow questions on a screenshot
Where does the eye land first, where does it go second, where does it end? The end point should be the action or the confirmation. The biggest element is the hook, not always the most important item. Sketch the intended 1-2-3 path, then compare with the screenshot.
- Look for: an eye path that ends on decoration, a footer link, or a dead corner.
- Fix: move the CTA to where the path ends, after the value statement, not above it.
Sources: SatoriGraphics ([The ONLY Video On Visual Hierarchy](https://www.youtube.com/watch?v=4QNEDhrsRLo)); SatoriGraphics ([Control A Viewers Eye](https://www.youtube.com/watch?v=dTsWYQawXRw))

### Shrink it to thumbnail size
Zoom to about 25% or look at it as a thumbnail. What you can still read should be the main message, in the right order. At 50% zoom, look for clumps: crowding is almost always a micro-space problem (elements too close), not too much content.
- Fix for crowding: shrink elements slightly and add room, before cutting copy.
Sources: willpatersondesign ([How To MASTER Visual Hierarchy](https://www.youtube.com/watch?v=X301kKG7WOY)); SatoriGraphics ([Making Designs BETTER In Seconds](https://www.youtube.com/watch?v=Y3lcMq0yfjM)); SelfMadeWebDesigner ([11 Years of Brutally Honest Web Design Advice](https://www.youtube.com/watch?v=WxZHUe8mvhU))

### Count the loud elements per viewport
Count colored badges, floating widgets, filled buttons, banners. A menu screen with a shouting banner, six colored tags, a chat bubble and two big buttons fails because of many small loud things, not one.
- Fix: keep one loud element, push the rest to neutral styles. Reserve the saturated accent for the primary CTA and critical alerts.
Sources: amirmoradiUX ([How to Become a Product Designer in the AI Era](https://www.youtube.com/watch?v=ky_F3jdnT4Y)); TimGabe ([How Addictive Apps Are Made](https://www.youtube.com/watch?v=AnL49w4yIOw))

### Give each element a job, or delete it
Audit components and write each one's job for the user. If the job is "decoration" or "fill dead space", delete it. Remove one element at a time until meaning breaks, then put the last one back. Never remove the cue that tells users what the thing is.
Sources: SatoriGraphics ([5 GOLDEN Rules Of MINIMAL Graphic Design](https://www.youtube.com/watch?v=2mO5DiX4ipU)); willpatersondesign ([Reviewing UNREAL Subscriber LOGO Designs! Ep 21](https://www.youtube.com/watch?v=FJsdWxs-B5Q))

### Wireframe in gray boxes, with real content, before color
Gray boxes make people argue about placement (the thing to settle first) instead of color. Lay out with plain boxes sized by importance and judge the weight distribution from the shapes alone. Then swap in real copy, because real length changes the layout. Do the first pass in one neutral palette and add the accent after hierarchy and spacing work.
Sources: amirmoradiUX ([The 14 UX Deliverables That Get You Hired](https://www.youtube.com/watch?v=xyyMVYMOO6Y)); willpatersondesign ([How To Create STUNNING Layouts](https://www.youtube.com/watch?v=9JiKfJdXZWU)); willpatersondesign ([How To Design A Professional Typographic Vintage Logo](https://www.youtube.com/watch?v=3uw-BAJLseE))

### Fix a weak page in this order
Typography, spacing, grid and structure, one deliberate break of the monotony, color, visuals, small details. The early steps alone make a mediocre page look decent. Add no glows or effects until spacing and type are settled. For a messy existing UI, change the shared tokens (type scale, line height, spacing scale) first, because every component consumes them.
Sources: TimGabe ([Design Better Than 99% of UI Designers](https://www.youtube.com/watch?v=PGQnGEH7c-E)); Hatch Conference ([Building design systems that work for your whole Organisation](https://www.youtube.com/watch?v=2ljl0aUdcpg))

### Diagnose from the bottom when a screen feels off
Order of causes: unclear goal, untrimmed scope, wrong flow, wrong placement, then surface styling. "If your user feels lost, it is not because your colors are bad, it is because your structure is broken."
Sources: amirmoradiUX ([The 5-Layer Framework That Gets Designers Paid Like Seniors](https://www.youtube.com/watch?v=gekAqINXbwc))

### Find dead space and decide: fill it or make it intentional
Scan each screen for large empty zones that nothing leads into. Either place a purposeful element there (proof, testimonial, logos) or align the emptiness to the grid so it reads as chosen.
- Look for: a heavy image on one side and a blank, unbalanced other side.
Sources: willpatersondesign ([Watch Me Design a Typographic Poster](https://www.youtube.com/watch?v=RvykWGAUTiw)); DesignSpo ([I Redesigned YOUR Websites - Episode 2](https://www.youtube.com/watch?v=oO8MzIVyiv0)); SelfMadeWebDesigner ([Ultimate Website Layout Guide](https://www.youtube.com/watch?v=s2DVOZ62F8w))

## Building hierarchy

### Use several levers, and try whitespace first
Levers: size, weight, color, whitespace, position, orientation, typeface style (serif body with sans heading is a cheap one). To promote an element, try in order: more space around it, bigger size, heavier weight, accent color. To demote, reverse. Whitespace is the most forgotten lever. Size is amplified or cancelled by contrast and space: a small high-contrast element with room can beat a large low-contrast one in clutter.
Sources: SatoriGraphics ([This Design Technique Changes EVERYTHING](https://www.youtube.com/watch?v=UFF7GAjRPOs)); SatoriGraphics ([MASTER Hierarchy For Non-Amateur Graphic Designs In 2026](https://www.youtube.com/watch?v=ZZKHTk_31ik)); SatoriGraphics ([I Wish I Knew These Graphic Design Rules SOONER](https://www.youtube.com/watch?v=05EKAJPRrGw))

### Make the size jump obvious, and skip a weight
The step between heading and subtitle must be clear, not 10 percent. Examples given: headline 64px at 110% line height with a 32px subtitle (2:1); 96px headline with a 24px subtitle; section title 48px semibold with a 24px gray sub. For secondary text, drop at least one weight step (800 vs 600, 600 vs 400) and a little size. Avoid a muddy 400 vs 500.
- Look for: adjacent elements with near-identical size and weight.
- Fix: headline 700-800 against body 400. A second tier is roughly 50-80% smaller than the first.
Sources: DesignSpo ([I Redesigned YOUR Websites - Episode 2](https://www.youtube.com/watch?v=oO8MzIVyiv0)); willpatersondesign ([How To Design A Modern Typographic Poster](https://www.youtube.com/watch?v=JudTy2aLG2o)); willpatersondesign ([5 tips to INSTANTLY up your DESIGN GAME](https://www.youtube.com/watch?v=9epeFitJIoE)); SatoriGraphics ([MASTER Hierarchy For Non-Amateur Graphic Designs In 2026](https://www.youtube.com/watch?v=ZZKHTk_31ik))

### Value big, label small
In metric cards the number is the loudest thing and the label is small and muted. A common mistake is big labels that steal attention from values. In detail and settings pages, bold the value, mute the label, add a leading icon on key fields. A page of identical "label: value" rows is a monotone wall.
- Fix: stat number 28-40px semibold, label 12-14px muted.
Sources: uxpeak ([Top 5 UX/UI Design Tips, part 1](https://www.youtube.com/watch?v=8pMUkEbAM7g)); uxpeak ([Junior to Senior UX/UI Designer](https://www.youtube.com/watch?v=YlN28RNChl0))

### Make the main job the biggest thing, tuck secondary controls into its corner
Money transfer example: the amount is the hero, the currency picker sits inside the amount field. On checkout and billing, the total must be the biggest number and the pay button must look like a button. A discount banner must not outrank the amount due.
Sources: uxpeak ([Junior to Senior UX/UI Designer](https://www.youtube.com/watch?v=YlN28RNChl0)); amirmoradiUX ([How to Become a Product Designer in the AI Era](https://www.youtube.com/watch?v=ky_F3jdnT4Y))

### Use a one-color pop and desaturate the rest
In a muted UI, a single colored element becomes the focal point. When color contrast is weak, desaturate or fade competing elements instead of enlarging the focal one. In dashboards, mute secondary chart series and keep only the key series saturated. Use contrast as peaks and valleys: full contrast only where attention should rest.
Sources: SatoriGraphics ([The ONLY Video On Visual Hierarchy](https://www.youtube.com/watch?v=4QNEDhrsRLo)); SatoriGraphics ([MASTER ADVANCED Hierarchy In 9 Minutes](https://www.youtube.com/watch?v=59e7KyACsX4)); SatoriGraphics ([MASTER Hierarchy For Non-Amateur Graphic Designs In 2026](https://www.youtube.com/watch?v=ZZKHTk_31ik))

### Put one dominant tile in every multi-card section
In bento grids and card rows, make one card visually dominant (larger, darker or brighter) and let the rest support. Put the key reassurance (no commitment, money-back) in that tile. Without it the section scatters, and autoplay media in one tile steals focus from the text you want read. In pricing, a larger or raised recommended plan in the middle of equal neighbors reads as the leader.
Sources: SelfMadeWebDesigner ([33 UNIQUE Website Layouts](https://www.youtube.com/watch?v=nZ2BJt9PgKE)); SelfMadeWebDesigner ([Ultimate Website Layout Guide](https://www.youtube.com/watch?v=s2DVOZ62F8w)); SatoriGraphics ([Master ADVANCED Hierarchy In Under 7 Minutes](https://www.youtube.com/watch?v=vDe1els66t8))

### Rank actions: filled, outlined, text link
One filled primary per screen. A real secondary (outlined or tonal button) beats a plain text link for the second action when it matters, for example "View ticket" filled and "Add to calendar" outlined. Tertiary is a text link. The primary should feel heavy enough, not small with lots of empty space around it. Primary is about 1.5-2x the height of standard text elements.
- Fix on mobile: primary full width in a bottom bar.
Sources: amirmoradiUX ([Figma Agent vs Claude](https://www.youtube.com/watch?v=wx2ylgMU8WM)); SatoriGraphics ([How To Master This One Important Design Principle](https://www.youtube.com/watch?v=fB4ZXJVcl6w)); TimGabe ([How Addictive Apps Are Made](https://www.youtube.com/watch?v=AnL49w4yIOw))

### Use contrast to create rhythm, then break it once
Repeat spacing, size and shapes to build a steady rhythm, then break it at one chosen spot: a featured plan, a hero image crossing the grid, a logo strip running edge to edge, a carousel that overflows right. The eye goes where the expectation breaks. Overusing breaks removes the effect. After the break, use alignment and nearby text to lead the eye to the final CTA.
Sources: SatoriGraphics ([MASTER Hierarchy For Non-Amateur Graphic Designs In 2026](https://www.youtube.com/watch?v=ZZKHTk_31ik)); DesignSpo ([$1,000,000 Design Portfolios](https://www.youtube.com/watch?v=DaeEKKSpgXU)); TimGabe ([Design Better Than 99% of UI Designers](https://www.youtube.com/watch?v=PGQnGEH7c-E)); SatoriGraphics ([5 Reasons Why Grids Are SO USEFUL](https://www.youtube.com/watch?v=vnt4pjH_O54))

### Reuse a marker to connect related parts
When two parts of a screen refer to the same thing (current period, selected item), give them the same marker, color or shape. One pulsing dot for "current period" in both chart and action area linked them instantly. Repeating an accent on CTA, active nav state, links and the key chart series works the same way.
Sources: TimGabe ([4 levels of UI/UX design](https://www.youtube.com/watch?v=86PGRyQjdzQ)); SatoriGraphics ([PERFECT LAYOUT DESIGN Step by Step](https://www.youtube.com/watch?v=eiV7E_LVlxs))

### Make the page's primary object visible by default
Linear dropped a dashboard-style project page (many equal panels that did not interact, nothing inviting work) and later regretted hiding issues behind a small toggle. Their fix: the work list stays above the fold, long summaries are collapsed with a disclosure for newcomers, and reports live in a side panel reachable from several places. Saved filter tabs above a list turned a boring list into a team "home".
- Look for: a detail page that is a grid of equal-weight cards.
- Fix: one primary working area, summaries and analytics in a right drawer, saved views as tabs.
Sources: Hatch Conference ([Adrien Griveau: How Linear designs for Planners](https://www.youtube.com/watch?v=9sJCu7BPvSw))

## Reading path and focal point

### One focal point per screen, and say what it is
Without a focal point a design is forgettable. It can be a big image, a large headline or a strongly different color. Give it extra room and keep competing elements smaller. For a creative or SaaS hero, pick one "star" tied to what the product does (for example a chart-like abstract visual behind the hero), keep it out of the text's way, and never pick it only because it looks cool.
Sources: SatoriGraphics ([Master Minimal Design](https://www.youtube.com/watch?v=CuKPfODOsnA)); SelfMadeWebDesigner ([6 EASY Tips to 10x Any Site's Design](https://www.youtube.com/watch?v=pbhLsV-Dyho)); SatoriGraphics ([6 Golden Rules Of Layout Design](https://www.youtube.com/watch?v=EFf9jBs2yfU))

### Attract, intrigue, deliver
Hook (big visual or headline), then interest (one-line subhead or curiosity line), then the message (small text, details, CTA). Apple's iPhone page: product image and name first, tagline second, paragraph third. A dashboard maps the same way: main KPI biggest, supporting charts second, filters and details third. Fewer elements of a type means more visible (one title, several chapters, many paragraphs).
Sources: SatoriGraphics ([The ONLY Video On Visual Hierarchy](https://www.youtube.com/watch?v=4QNEDhrsRLo)); SatoriGraphics ([Master 5 Design Principles](https://www.youtube.com/watch?v=FpwZTl3dCZE)); DesignSpo ([How to Make Your Website Look PROFESSIONAL](https://www.youtube.com/watch?v=jtjOJkmnzs8))

### Make gaze and shape point at the CTA
Faces and lines of sight pull the eye, and text placed where a subject looks gets read. Flip the photo so the person looks at the headline or CTA. Arrows, angled shapes and diagonals can lead toward the action. Remove decorative shapes that point away from content, since random pointers cause visual anxiety. Elements that step down in size toward the CTA also funnel the eye.
Sources: SatoriGraphics ([MASTER Hierarchy For Non-Amateur Graphic Designs In 2026](https://www.youtube.com/watch?v=ZZKHTk_31ik)); SatoriGraphics ([Master This Design Theory](https://www.youtube.com/watch?v=D4RPBIAvq5A)); SelfMadeWebDesigner ([33 UNIQUE Website Layouts](https://www.youtube.com/watch?v=nZ2BJt9PgKE))

### Balance with weight, not only symmetry
Heavy image on one side, quiet text and CTA zone on the other. Split 50/50 for calm, 60/40 for dynamic. A heavy left with an empty right feels broken, and one odd-size item breaking an aligned layout becomes the focal point. If it feels lopsided, rework the layout instead of nudging. Symmetric centered sections are the safe default for a plain landing header. Horizontal composition feels calm (settings, billing); diagonals feel like movement (launch banners). Cites Rudolf Arnheim: the natural focal point sits slightly above exact center.
Sources: SatoriGraphics ([AMATEUR VS PRO: Advanced Design Examples](https://www.youtube.com/watch?v=xzyvO71XEaA)); SatoriGraphics ([The Layout Design Workflows You Need](https://www.youtube.com/watch?v=Uz3B2u9Ug8o)); willpatersondesign ([The WORST Graphic Design MISTAKES](https://www.youtube.com/watch?v=FpqGgXiOW7c)); SatoriGraphics ([Master This Design Theory](https://www.youtube.com/watch?v=D4RPBIAvq5A))

### Use odd counts and a dominant middle for groups
Three (or five) items with one emphasized read as more harmonious than four. Pricing, feature triplets and testimonials: make the middle one larger or raised. The speaker calls it helpful, not essential. Four equal, uniform cards are fine too, and 2x2 beats 4 across when each card needs width.
Sources: SatoriGraphics ([Master LAYOUT & COMPOSITION Design](https://www.youtube.com/watch?v=N8TQfE1qKeE)); SatoriGraphics ([How To MASTER 1 Design Principle In 4 Minutes](https://www.youtube.com/watch?v=_LCEw4jCq1o)); DesignSpo ([I Redesigned YOUR Websites - Episode 2](https://www.youtube.com/watch?v=oO8MzIVyiv0))

### Scan patterns are a starting skeleton, not a law
For sparse marketing sections the Z path (logo top-left, visual or nav top-right, diagonal, CTA at the end) works. For text-heavy pages and settings, left-align and put headings and key words at the start of lines. Two sources say the F-pattern is outdated and can hide content when forced; they rely on explicit size and weight levels instead. Cites: a research paper found sites that followed left-to-right, top-to-bottom reading were rated about 20% more beautiful. Reverse for RTL.
Sources: DesignSpo ([The Beginner's Guide To Visual Hierarchy](https://www.youtube.com/watch?v=kK1TOpI948o)); SatoriGraphics ([How To MASTER 1 Design Principle In 4 Minutes](https://www.youtube.com/watch?v=_LCEw4jCq1o)); SelfMadeWebDesigner ([Give Me 7 Minutes & Your Web Design Skills Will Take Off](https://www.youtube.com/watch?v=1NTKwpAVcHg))

### Left-align text, center only on purpose
Left-aligned text looks sharper and continues the left-to-right movement; centered stacks of text look amateur. Left-align body, labels, cards and forms. Center short hero lines and empty states. Stacked text beside an icon should be left-aligned to the icon block, not centered. Startup heroes are the exception and are nearly all centered.
Sources: willpatersondesign ([5 Pro Tips For Minimal Design](https://www.youtube.com/watch?v=B-F7H1xVcec)); SatoriGraphics ([AMATEUR VS PRO GRAPHIC DESIGN! Typography Showdown](https://www.youtube.com/watch?v=Ta5hywdHPWU)); DesignSpo ([21 Website Layouts You Should Know](https://www.youtube.com/watch?v=EZGR72wgOT4))

### One idea per section, few text groups per screen
A section mixing features, plan model and testimonials overwhelms. If a screen has more than about three or four competing text groups, merge related ones into fewer proximity groups and tone down the loudest numbers. Weak designs fail because too many ideas compete and nothing is decided as the main thing.
Sources: SelfMadeWebDesigner ([33 UNIQUE Website Layouts](https://www.youtube.com/watch?v=nZ2BJt9PgKE)); SatoriGraphics ([I Improved FAMOUS Graphic Designs](https://www.youtube.com/watch?v=JiJ4EntauxE)); SatoriGraphics ([The Difference Between Amateur and Pro Designers](https://www.youtube.com/watch?v=CMv2vrpgp0w))

## Spacing system

### Pick one base unit and snap every gap to it
Base 8 with 4 as the fine step (icon next to a label, tight pairs), or a base-4 scale. Tokens like 4/8/12/16/24/32/48/64. A 51px element is a mistake. If a gap looks off, adjust the neighboring size (icon, text) before adding an odd value like 6px. Padding, margins and gaps stay on the scale. Fluid widths and content-driven heights do not (a 350.5px wide card is fine). Inconsistent spacing registers as noise and makes the eye jump.
- Look for: values like 13px, 22px, 27px in the CSS.
- Fix: grep for off-scale values and snap them. Use `gap` on flex/grid containers instead of per-child margins so repeated rows are identical.
Sources: TimGabe ([You'll Regret NOT Using The 8pt Grid in Figma](https://www.youtube.com/watch?v=ohF93_k3IMk)); DesignSpo ([The Golden Rule Of Web Design](https://www.youtube.com/watch?v=CASPWJUsHPM)); SelfMadeWebDesigner ([9 Web Design Hacks I Wish I Knew Years Ago](https://www.youtube.com/watch?v=TeMtV8BaZt0)); SatoriGraphics ([10 Quick Hacks for Better Designs in 2025](https://www.youtube.com/watch?v=cBoONiQ9u0Q))

### Space by relationship, with a ladder
Concrete ladders from the sources: icon to label 4; menu rows 8; title to subtitle 16 (or 6-12 in tight cards); unrelated components in one section 24 (same as the column gutter); between sections 32 or more. Another set: form fields 24, heading block to form 56, sibling cards 48, sections inside an outer container 64, icon to title 12. Pick a base value inside a group and double it between groups. Heading above gets about 2x the space it has below, so it clearly belongs to the block under it.
- Look for: a heading sitting equally between two blocks; equal gaps on every line of an order summary.
- Fix: `--space-base` inside a card, `--space-group: calc(var(--space-base) * 2)` between sibling groups, one `--section-gap` for sections.
Sources: DesignSpo ([20 Graphic Design Hacks You Need To Know](https://www.youtube.com/watch?v=EGPvdevwM8o)); TimGabe ([Design Better Than 99% of UI Designers](https://www.youtube.com/watch?v=PGQnGEH7c-E)); TimGabe ([6 UI Hacks I Wish I Knew As A Beginner](https://www.youtube.com/watch?v=88XxC0_zs74)); DesignSpo ([I Redesigned YOUR Websites - Episode 2](https://www.youtube.com/watch?v=oO8MzIVyiv0))

### Gutter is the unit for gaps between containers, half of it inside
With a 32px gutter, separate containers by 32px+ and elements inside a container by about 16px. Section inner padding defaults to the gutter value, stepped up for more separation, and stays identical across sections. Keep one section-gap token and check any section that deviates.
Sources: DesignSpo ([20 Graphic Design Hacks You Need To Know](https://www.youtube.com/watch?v=EGPvdevwM8o)); SatoriGraphics ([How To Use Advanced Graphic Design Principles](https://www.youtube.com/watch?v=Z2RgNy94-No)); TimGabe ([Design Better Than 99% of UI Designers](https://www.youtube.com/watch?v=PGQnGEH7c-E))

### Push the CTA slightly further from the text stack
Heading, subheading and body sit tight as one block (8-16px). The button gets more space above it (24-32px), so it belongs to the group but the layout looks designed rather than one uniform gap. Example set: 24px title to subtitle, 48px text block to buttons, 24px button to its note. A CTA also needs a clear zone of its own.
Sources: TimGabe ([9 SECRETS To Beautiful Landing Page Design Pt. 3](https://www.youtube.com/watch?v=vBuyR8uF380)); TimGabe ([Design Better Than 99% of UI Designers](https://www.youtube.com/watch?v=PGQnGEH7c-E)); SatoriGraphics ([6 Golden Rules Of Layout Design](https://www.youtube.com/watch?v=EFf9jBs2yfU))

### Starting numbers for landing pages
Text group to image at least 80-86px. Section vertical padding about 160px on desktop (see disagreements). Card inner padding 32px as baseline. Text containers no wider than about 600px. Inner content container about 960px, or 1200px for general content. Card grid gap at least 24px. 64px between stacked blocks and 80px between sections in a Figma-built site. When unsure, more space is safer.
Sources: TimGabe ([Design Better Than 99% of UI Designers](https://www.youtube.com/watch?v=PGQnGEH7c-E)); uxpeak ([UX/UI Design Tutorial in Figma - Modern Website](https://www.youtube.com/watch?v=SIoOS6tFw1Y)); SelfMadeWebDesigner ([33 UNIQUE Website Layouts](https://www.youtube.com/watch?v=nZ2BJt9PgKE))

### Control sizes on the grid
Buttons: large 64px high with 32px side padding, medium 48 with 24, small 40 with 16. Inputs and buttons both 40px when side by side, and equal height always. Use a fixed `height` with horizontal padding only, so heights stay on the grid. Icons 16/24/64/96. Card padding 32, gap 8 inside.
Sources: TimGabe ([9 SECRETS To Beautiful Landing Page Design Pt. 2](https://www.youtube.com/watch?v=cmSBbnrFGPg)); TimGabe ([Learn Framer For Beginners](https://www.youtube.com/watch?v=wgMgje60Ovw))

### Dynamic content gets fixed gaps, fixed containers distribute space
A hug-width button or chip uses a fixed gap between icon and label (`width:auto; gap:Npx`). A fixed-size container with changing content (nav, card rows, user content) distributes space (`space-between`, `grid` with equal tracks).
Sources: DesignSpo ([20 Graphic Design Hacks You Need To Know](https://www.youtube.com/watch?v=EGPvdevwM8o)); TimGabe ([Master Figma Auto Layout in 10 Minutes](https://www.youtube.com/watch?v=Kf8L3CeiWzQ))

### Group order summaries and tables by spacing, then isolate the total
Items together, fees together, the total gets its own space (extra top space, border, heavier weight). Equal gaps between every line read as one long list. Inside a card gap is smaller than between cards, which is smaller than between page sections.
Sources: amirmoradiUX ([How to Become a Product Designer in the AI Era](https://www.youtube.com/watch?v=ky_F3jdnT4Y)); SatoriGraphics ([How To INSTANTLY Make Your Graphic Design Better](https://www.youtube.com/watch?v=0SxzNcCrDxE))

### Match macro vs micro space to the surface
Cites: more macro space reads as minimal, modern and premium, and a viewer in a hurry needs more of it. More micro space with dense content reads as informative and serious. Marketing pages: large section gaps, few elements per viewport. Dense dashboards and docs: spend the effort on row spacing, line height and group gaps. Passive space (line gaps, padding) makes text legible; active space (gaps between chunks) sets reading order. Audit each gap and ask what it is for: legibility, guidance, or nothing.
Sources: SatoriGraphics ([Graphic Design Principles Are CRUCIAL](https://www.youtube.com/watch?v=UfkzHRM70sQ)); SatoriGraphics ([Graphic Design Principles Master-Class: White Space](https://www.youtube.com/watch?v=FDFD2-poyGw))

### When a page feels busy, add space before removing content
Increase section padding and group gaps first, then judge. When content is fixed and room is short, play Tetris: shrink fonts and images before cutting copy, add dividers to give long items their own zone, bold the key value. When a page is elegant but hard to read, raise body size before touching density. Do not be ultra-minimal by reflex; if a page feels empty and generic, add one strong element, not more space.
Sources: SatoriGraphics ([How To Actually Use Layout Design Properly](https://www.youtube.com/watch?v=q4_jHQru_LQ)); SelfMadeWebDesigner ([33 UNIQUE Website Layouts](https://www.youtube.com/watch?v=nZ2BJt9PgKE)); willpatersondesign ([5 Pro Tips For Minimal Design](https://www.youtube.com/watch?v=B-F7H1xVcec))

### Alternate dense and airy sections down a long page
Tight spacing feels fast; wide spacing feels like a pause. Hero hits fast, technical details sit in tight blocks, then one sparse section (a single statement or product image on open space) before the CTA. Keep spacing token values the same; vary only how many things share a viewport.
Sources: SatoriGraphics ([Graphic Design Principles Master-Class: White Space](https://www.youtube.com/watch?v=FDFD2-poyGw)); SatoriGraphics ([Full Course: 3 PROVEN Principles Of Layout Design](https://www.youtube.com/watch?v=GT-K0CrrgfU))

### Check text-in-frame padding and nearest-neighbor clearance
Text must never nearly touch a border, image or button. Badges, chips and buttons need at least one spacing unit of horizontal padding, equal on both sides. Give headings and body generous margins from edges and neighbors.
Sources: willpatersondesign ([Secret Techniques for Creating Eye-Catching Posters](https://www.youtube.com/watch?v=6at6VQD6iVQ)); SatoriGraphics ([Make BETTER Graphic Designs Using Visual Triggers](https://www.youtube.com/watch?v=V0DFvmTN4o8))

### Line height and display tightening
Body 1.5 when text looks crushed; subtitles about 1.2; display headings 0.95-1.1. A 110% line height on huge text leaves big gaps between stacked lines, and about 95% pulls two-line display text together. Slightly negative letter-spacing (about -0.03em on uppercase bold headings) helps.
Sources: TimGabe ([Learn Framer For Beginners](https://www.youtube.com/watch?v=wgMgje60Ovw)); DesignSpo ([I Redesigned YOUR Websites - Episode 2](https://www.youtube.com/watch?v=oO8MzIVyiv0))

### Derive scales from one ratio
Type and spacing from a fixed ratio so the system is derived, not invented: 1.25 or 1.333 for dense dashboards, 1.5+ for marketing, per one source. Another derives spacing from a unit in the thing itself (icon height halves and thirds as clear space). Judge the result by eye; the golden ratio is a restraint, not a goal.
Sources: willpatersondesign ([The Golden Ratio: Secret to Good Design or Just Hype](https://www.youtube.com/watch?v=UItSxy5rxB4)); willpatersondesign ([Why Pro Logos Look Perfect](https://www.youtube.com/watch?v=17cb1eqdy6I))

### Align optically, not just numerically
Round shapes overshoot a little to look equal to flat ones. Icons beside tall-ascender text drop a pixel or two to look centered. Play-triangle icons and badges nudge 1-2px after numeric centering. Round icons may need to be 1-2px larger than square ones. Trust the eye when the numbers are right and it still looks wrong.
Sources: willpatersondesign ([How To Design A Professional Modern Logo #3](https://www.youtube.com/watch?v=rR-ZeWO6PIM)); willpatersondesign ([Subscriber Logo Critique Season 2 Ep 1](https://www.youtube.com/watch?v=ECemKdwkxPw)); willpatersondesign ([Why Pro Logos Look Perfect](https://www.youtube.com/watch?v=17cb1eqdy6I))

## Grid, containers and alignment

### Build every page from boxes: full-bleed section, max-width constrainer, content
Section full-bleed, inner `max-width` container with `margin-inline:auto`, then groups. Use 1200 for general content and about 960 for text-heavy heroes. Pad the wrapper at least the gutter so text never touches the container edge on phones. Use as few boxes as you can.
Sources: TimGabe ([Learn Framer For Beginners](https://www.youtube.com/watch?v=wgMgje60Ovw)); DesignSpo ([How To Build A Website From Start To Finish](https://www.youtube.com/watch?v=b2TP7K9ZFWk)); SelfMadeWebDesigner ([Master Website Layouts in Under 10 Minutes](https://www.youtube.com/watch?v=EF_ucfA3CJs))

### 12 columns, whole spans, content on fewer
12 divides by 2, 3, 4, 6. Worked math: 12 x 72 + 11 x 24 = 1128px container. Gutter at or below 50% of column width; 24 is the common default. Use whole-column spans only (a 5.5-column box is a bug), such as text 6 and image 5 with a 1-column gap. Real content spans 1-6 columns, so prose and cards rarely run full width. Avoid odd grids (5 or 9 columns) and odd widths (45, 125). On a 6-column grid, an important item spanning 2 columns instead of 1 becomes dominant.
- Fix: `grid-template-columns: repeat(12,1fr)` with `grid-column: span N`. Equal `fr` columns in one container class keep sections aligned as items are added or removed.
Sources: DesignSpo ([The Golden Rule Of Web Design](https://www.youtube.com/watch?v=CASPWJUsHPM)); TimGabe ([Master Responsive Grids in Figma](https://www.youtube.com/watch?v=sybtdc4dYzE)); SatoriGraphics ([5 Reasons Why Grids Are SO USEFUL](https://www.youtube.com/watch?v=vnt4pjH_O54)); TimGabe ([Design Better Than 99% of UI Designers](https://www.youtube.com/watch?v=PGQnGEH7c-E))

### Check shared left edges in devtools
Left edges of headings, body, buttons, cards and nav items should land on a few shared x positions. In a 3-up feature row, icons, headings and descriptions of each column share the same left edge. A "made by" line off-center from the text above is the typical miss. Nav centering: `grid-template-columns: 1fr auto 1fr`, not flex `space-between` with unequal sides.
Sources: SatoriGraphics ([Master LAYOUT & COMPOSITION Design](https://www.youtube.com/watch?v=N8TQfE1qKeE)); ShantanuKumar ([How to Design Amazing Landing pages w/ Readymag](https://www.youtube.com/watch?v=dro9e5_VT2U)); TimGabe ([9 SECRETS To Beautiful Landing Page Design Pt. 3](https://www.youtube.com/watch?v=vBuyR8uF380))

### Break the grid once, on purpose
Keep content on grid lines, then let one element violate it: a hero image bleeding over a column edge, a badge overlapping a section boundary, an organic blob behind gridded content. One or two per screen, marked as intentional. Keep dashboards strict; save overlaps and off-grid art for marketing hero art.
Sources: SatoriGraphics ([How to BREAK Graphic Design Rules](https://www.youtube.com/watch?v=pEENvfgCEF0)); SatoriGraphics ([The ONLY Way To Break Graphic Design Principles](https://www.youtube.com/watch?v=aeI4pFCPgs8)); TimGabe ([9 SECRETS To Beautiful Landing Page Design Pt. 3](https://www.youtube.com/watch?v=vBuyR8uF380)); willpatersondesign ([Watch Me Design a Typographic Poster](https://www.youtube.com/watch?v=RvykWGAUTiw))

### Share one grid and one section rhythm across marketing, app and docs
The same container widths, gutters and section spacing across marketing page, app shell, emails and docs keep identity cohesive. Design the homepage first, lock its tokens and section components, then build inner pages from existing components.
Sources: SatoriGraphics ([How To Use Advanced Graphic Design Principles](https://www.youtube.com/watch?v=Z2RgNy94-No)); SelfMadeWebDesigner ([The Easiest Way to Build Killer Websites](https://www.youtube.com/watch?v=O7MaPnRy5Us))

### Use modular grids with inner buffers for card layouts
Pick a module shape and count, put big items in big modules, and keep inner padding so text never touches a module edge. You do not need to fill every module; empty modules are negative space. Use one aspect ratio for similar images (for example 3:2) via `aspect-ratio`.
Sources: SatoriGraphics ([The Layout Design Workflows You Need](https://www.youtube.com/watch?v=Uz3B2u9Ug8o)); SatoriGraphics ([How To Master This One Important Design Principle](https://www.youtube.com/watch?v=fB4ZXJVcl6w))

## Page and section layouts

### Hero recipes from one formula
Standard SaaS hero: nav with logo left and menu right, last nav item styled as a button, optional badge (news or award) above, 2-line benefit headline, supporting text, primary and secondary CTA, then a visual or demo. Variants change only alignment, size and gap: centered (mega headline, large gap, about 40px between heading, body, CTA); left-aligned (headline one size down, gap 32, smaller CTA, asset right); grid of four (smaller everything). Keep the same gap between heading, body and CTA in each variant. Narrow center column (about 640px on 12 columns) reads modern and focused, with the CTA also in the header.
- Look for: product screenshot taking about 60% of the hero so text feels cramped.
- Fix: headline is the center, product visual partly cropped at the bottom so the next section is hinted. For complex products, use a two-column hero with a bigger button and a GIF or loop on the right; avoid video in a side column because people expect video centered.
Sources: DesignSpo ([21 Website Layouts You Should Know](https://www.youtube.com/watch?v=EZGR72wgOT4)); TimGabe ([4 Easy Tips For Stunning Landing Pages](https://www.youtube.com/watch?v=cocnZubvfFE)); DesignSpo ([PRO Vs AMATEUR Website Design](https://www.youtube.com/watch?v=x8Vp8k3jXaA)); TimGabe ([Steal This Landing Page Hero Workflow](https://www.youtube.com/watch?v=m3NjcBDqFnA))

### Write the hero's message, action, and asset before you design it
Order: write heading, body and visual; pick the one desired user action; collect references with room for your heading, body, CTA and visual; then design. If any is missing, stop. Cites: about 3 seconds to convince a visitor the click was worth it; about 20% of people scroll past the fold. Check the hero at 1440x900 and 390x844 without scrolling: it says what it is and shows one CTA. Do not shrink images and padding to cram more above the fold; the first view has to sell one thing well.
Sources: TimGabe ([Steal This Landing Page Hero Workflow](https://www.youtube.com/watch?v=m3NjcBDqFnA)); SelfMadeWebDesigner ([The Easiest Way to Build Killer Websites](https://www.youtube.com/watch?v=O7MaPnRy5Us)); SelfMadeWebDesigner ([50 Web Design Tips & Tricks](https://www.youtube.com/watch?v=rRFD6tENX2U)); uxpeak ([$42K vs $297K UX/UI Design](https://www.youtube.com/watch?v=U7jTCgIWS4w))

### Show real output big when the product's value is its output
Midjourney redesign: dense grid of real output images in the hero, nav reduced to sign in plus one filled join button, a short scroll story (hero, mock prompt input, final CTA). For a tool whose value is what it makes, lead with the output, not the team.
Sources: TimGabe ([I Redesigned Midjourney's Landing Page in 19 Minutes](https://www.youtube.com/watch?v=_n39rxieClg))

### Pick the benefit layout by how the benefits relate
Benefits are about 60-80% of a homepage. Point-by-point benefits: accordion or tabs with a changing visual. Many loosely related features: bento. A story (build, launch, grow): step tabs. One outcome by many ways: one big featured benefit plus 3 small. A visual product: floating graphics around a headline. Do not use a plain 3-icon row for everything.
Sources: DesignSpo ([21 Website Layouts You Should Know](https://www.youtube.com/watch?v=EZGR72wgOT4)); DesignSpo ([The Perfect Website Layout For Startups](https://www.youtube.com/watch?v=Z7r5RNo-hN0))

### Column count by content type
3 columns: features, testimonials, plans. 4: blog posts, portfolio, products (crowded on small screens); 2x2 beats 4 across when cards need width and the section should fit one viewport. 5+: footers and link directories only, titled and aligned. Rarely past 6. A grid does not need filling; leave an empty slot as a mental pause.
Sources: SelfMadeWebDesigner ([33 UNIQUE Website Layouts](https://www.youtube.com/watch?v=nZ2BJt9PgKE)); DesignSpo ([I Redesigned YOUR Websites - Episode 2](https://www.youtube.com/watch?v=oO8MzIVyiv0))

### One repeatable container for rhythm
Design one container (title, benefit line, description, divider, image) and repeat it for each service or feature. Repetition removes clutter. Keep equal card heights, identical text-to-button gap and identical card gaps; uneven gaps are a visible flaw. Replace four identical per-card buttons with one section button or a clickable card. Remove duplicated logos (nav only).
Sources: DesignSpo ([I redesigned YOUR websites](https://www.youtube.com/watch?v=-F1F4YISY4E)); DesignSpo ([I Redesigned YOUR Websites - Episode 2](https://www.youtube.com/watch?v=oO8MzIVyiv0)); DesignSpo ([PRO Vs AMATEUR Website Design](https://www.youtube.com/watch?v=x8Vp8k3jXaA))

### Vary section structure with purpose
Start familiar, then take a turn: identical repeated blocks signal "I have seen the end". Alternate single column, two column, cards, image side and background every one or two sections, matching the story rather than random. Do not lean on the 50/50 image-left/text-right split; tweak it (stagger image heights, vary proportions, one overlap). Single column for focus (hero, CTA); second column for features with icons or testimonials with photos.
Sources: SelfMadeWebDesigner ([Ultimate Website Layout Guide](https://www.youtube.com/watch?v=s2DVOZ62F8w)); SelfMadeWebDesigner ([Master Website Layouts in Under 10 Minutes](https://www.youtube.com/watch?v=EF_ucfA3CJs)); SelfMadeWebDesigner ([50 Web Design Tips & Tricks](https://www.youtube.com/watch?v=rRFD6tENX2U))

### Standard landing order
Hero, a short "what is this" section tied to the visitor's goal or pain, features, proof, call to action, footer. Each section: a headline naming a pain or outcome, a subline with a new angle, a product visual with context, trust proof, one CTA. Non-sales links (careers, docs, help center, status) go in the footer; marketing nav stays at 3-5 items plus one CTA button.
Sources: TimGabe ([9 SECRETS to BEAUTIFUL Landing Page Design Pt. 1](https://www.youtube.com/watch?v=RdHXcv1k_Dg)); DesignSpo ([The Perfect Website Layout For Startups](https://www.youtube.com/watch?v=Z7r5RNo-hN0))

### Dense optional text: dividers, numerals, accordions, bullets with icons
Numbers draw the eye in process sections (large numerals on steps). Convert any paragraph with 3+ parallel ideas into a short list with small icons. Add row dividers and consistent icons to long lists (changelogs, FAQs) so each item reads as a unit. Accordion: most important item open by default, horizontal labels. Cites: a Nielsen Norman study found users skim past big blocks of text; break up paragraphs every two or three sentences.
Sources: SelfMadeWebDesigner ([9 Web Design Hacks I Wish I Knew Years Ago](https://www.youtube.com/watch?v=TeMtV8BaZt0)); SelfMadeWebDesigner ([33 UNIQUE Website Layouts](https://www.youtube.com/watch?v=nZ2BJt9PgKE)); SelfMadeWebDesigner ([Ultimate Website Layout Guide](https://www.youtube.com/watch?v=s2DVOZ62F8w))

### Options as selectable cards, and let users choose list vs card view
Plan, role and onboarding pickers: radio cards (border plus check state) with label, icon or image instead of plain radio lists, with an "Other" escape that allows typing. On browse pages, offer a card/list toggle and remember it: big photo cards help desire, compact lists help comparing.
Sources: uxpeak ([Top 5 UX/UI Design Tips, Part 2](https://www.youtube.com/watch?v=gG4urkinFQI)); uxpeak ([$42K vs $297K UX/UI Design](https://www.youtube.com/watch?v=U7jTCgIWS4w))

### Expose content instead of a banner that leads to content
A banner saying "Discover 100+ recipes" costs a tap before any value. Show the top 10 directly. Count taps to first value. Related trust data goes beside its anchor (rating next to the product title, not far below).
Sources: uxpeak ([Top 5 UX/UI Design Tips, Part 2](https://www.youtube.com/watch?v=gG4urkinFQI)); uxpeak ([This UI/UX Redesign Will Teach You More Than 100 Tutorials](https://www.youtube.com/watch?v=GGg61sdEjeI))

### Keep key actions in the same place across screens
Primary button position, nav order and search location stay identical across pages so users build muscle memory. Flag any screen where the primary action moves. Optimize the most common task first and reveal rare actions only on demand.
Sources: TimGabe ([What Founders Can Learn From Apple's Design Domination](https://www.youtube.com/watch?v=doiaMtD80p8))

## Imagery placement

### Keep text off faces and subjects
The eye goes to faces, so text over a face is hard to read and a heavy black overlay washes the photo out. Never put logo, badge or text over a face. Move the logo to the nav only. Let the image run full height and place text on the empty side or in the lower area.
- Look for: a hero photo with a text shadow or oversized logo trying to compensate.
- Fix: text anchored bottom or on the empty side, over the flattest part of the image, contrast checked on the lightest area.
Sources: DesignSpo ([I redesigned YOUR websites](https://www.youtube.com/watch?v=-F1F4YISY4E)); DesignSpo ([PRO Vs AMATEUR Website Design](https://www.youtube.com/watch?v=x8Vp8k3jXaA)); SelfMadeWebDesigner ([Ultimate Website Layout Guide](https://www.youtube.com/watch?v=s2DVOZ62F8w))

### For user-uploaded images, put text below the image, not on it
Uber Eats-style cards: name and numbers sit under the photo so the card looks the same whatever the vendor uploads. If you must overlay, use a scrim. Overlay or video backgrounds are fine only if the text block stays fully legible.
Sources: uxpeak ([$42K vs $297K UX/UI Design](https://www.youtube.com/watch?v=U7jTCgIWS4w)); DesignSpo ([PRO Vs AMATEUR Website Design](https://www.youtube.com/watch?v=x8Vp8k3jXaA))

### Size product imagery to sell, not to identify
Cites a junior design with 56px food photos: you see a bowl but are not tempted. The intermediate fix made photos about 3x wider and the largest element on the card; seniors went full width. If imagery is why people click (product, template, recipe, listing), give it at least card width. Small thumbs are for identification only.
Sources: uxpeak ([$42K vs $297K UX/UI Design](https://www.youtube.com/watch?v=U7jTCgIWS4w))

### Every image must support the message
Three mistakes: wrong emphasis (a prominent image unrelated to the main message), clashing style, irrelevant imagery that misleads. Delete stock filler; swap for product screenshots or real people. Supporting background imagery sits at low opacity so the headline stays the primary read. Watermarks, logo patterns and background repeats stay lower in contrast than the hero content. When a lot of colorful visuals sit inside long text, use a few vivid ones that mirror the copy, not many tiny tightly packed thumbnails.
Sources: SatoriGraphics ([How To Actually Use Layout Design Properly](https://www.youtube.com/watch?v=q4_jHQru_LQ)); SelfMadeWebDesigner ([11 years of web design knowledge in 7 minutes](https://www.youtube.com/watch?v=ityZtG3FMgw)); willpatersondesign ([5 MIND BLOWING Poster Design Tips](https://www.youtube.com/watch?v=jo36w2_payY)); SatoriGraphics ([Making FAMOUS Graphic Designs Better](https://www.youtube.com/watch?v=INMuAYZDums))

### Pin decorative images to the content wrapper, not the page
Floating hero images positioned relative to the same max-width wrapper as the text stay near it. Pinned to the full-width section they drift to the screen edges on wide monitors and wander during resize. Use `position:relative` on the wrapper and absolute children with only the edges needed. At 320-375px check that decoration does not overlap copy; move or crop it.
Sources: TimGabe ([Learn Framer For Beginners](https://www.youtube.com/watch?v=wgMgje60Ovw))

### Use icons only when relevant, one style
A relevant icon next to an address, email or key feature speeds scanning (map pin beside the address). It must be obviously relevant (camera for photography), not filler. Cliche themed bullets look amateur; use plain bullets or checks.
Sources: SatoriGraphics ([The ONLY Video You Need To Improve Your Graphic Designs](https://www.youtube.com/watch?v=VA5QmkoQqz0)); SatoriGraphics ([Making FAMOUS Graphic Designs Better](https://www.youtube.com/watch?v=INMuAYZDums))

### Size the logo to its real proportion, ship lockup variants
Do not inflate the logo to feel branded: about 24-32px high in a header, with the icon-to-wordmark ratio kept the same everywhere. Ship at least a horizontal lockup (nav, email header), a stacked or square version (avatar, app icon), and an icon-only favicon. Check each in its real slot at nav size, and check the mobile header at 360px. Until the brand is known, keep the wordmark next to a bare icon.
Sources: willpatersondesign ([Reviewing Your Logos - Brutally Honest](https://www.youtube.com/watch?v=ZjTNqPZqFEw)); willpatersondesign ([Subscriber LOGO CRITIQUE Ep 22](https://www.youtube.com/watch?v=gR1rJj45RGY)); willpatersondesign ([Pro Logo Designer VS Fiverr Designers](https://www.youtube.com/watch?v=TKdsKBd7Eo8)); Will Paterson Design ([The NEW Subscriber Logo Critique](https://www.youtube.com/watch?v=uRzEZ_tl5SA))

## Mobile and responsive layout

### Reflow per breakpoint, do not shrink the desktop
Column counts: 12 desktop, 8 tablet, 4 mobile (Material), or 12, 6, 1 in another source. Shrink margins and gutters with the screen, for example gutter 20, 16, 12 and mobile page margin about 12. Rebalance for small screens: pin images to the top, remove decorative animations, check hover-only effects. Preview the stacked vertical order before publishing.
- Look for: a desktop grid scaled down, with 4-column rows on a phone.
Sources: TimGabe ([Master Responsive Grids in Figma](https://www.youtube.com/watch?v=sybtdc4dYzE)); DesignSpo ([20 Graphic Design Hacks You Need To Know](https://www.youtube.com/watch?v=EGPvdevwM8o)); SelfMadeWebDesigner ([Master Website Layouts in Under 10 Minutes](https://www.youtube.com/watch?v=EF_ucfA3CJs)); ShantanuKumar ([How to design a simple website](https://www.youtube.com/watch?v=o8S9qJbvpkU))

### Step components down together at each breakpoint
Example per tier: CTA height 88, 72, 64; radius 20, 16, 12; decoration 240, 184, 120; side padding 64, 32, 12. Section padding 40 on tablet and 24 on mobile, a smaller logo variant, hamburger with an open state. On tablet, hide nav links and cut header height to about 96px.
Sources: TimGabe ([Learn Framer For Beginners](https://www.youtube.com/watch?v=wgMgje60Ovw)); TimGabe ([Complete Website in Framer](https://www.youtube.com/watch?v=PYskozIWh-E))

### Make layouts adapt with wrap, fill and fractions
`flex-wrap: wrap` lets cards drop to a new row. Children sized by `1fr` or `flex:1` share space. A single fixed-width child among fill children squashes or overflows on small screens. Text blocks fill; they are not fixed.
- Look for: fixed `width: Npx` on a text container that overflows at 320-375px.
- Fix: the cards pattern, `display:grid; gap:24px; grid-template-columns: repeat(3,1fr)` dropping to 2 then 1; a feature card gets `grid-column: span 2`; grid height auto.
Sources: TimGabe ([Learn Framer For Beginners](https://www.youtube.com/watch?v=wgMgje60Ovw)); TimGabe ([Card Layouts in Framer](https://www.youtube.com/watch?v=udTGvssp-h8))

### Card rows: swipe or stack
3-5 card rows can become a horizontal scroll row on mobile to limit vertical scrolling (`overflow-x:auto` with scroll-snap), or stack when each card carries essential content. Decide by how much work the user needs to reach the next section. Four-plus columns on a phone rarely make sense, except text on one side with minor images.
Sources: SelfMadeWebDesigner ([33 UNIQUE Website Layouts](https://www.youtube.com/watch?v=nZ2BJt9PgKE))

### Put primary actions where the thumb rests
Bottom and center, not the top corners: primary CTA in a bottom sticky bar, 44-48px tall, full width, no tiny icon-only primary. Bottom bars leave room for the home indicator (about 34px) and use `padding-bottom: env(safe-area-inset-bottom)`. Test on a real phone at 360, 390 and 430 widths; a desktop preview misleads.
Sources: uxpeak ([Top 5 UX/UI Design Tips, Part 2](https://www.youtube.com/watch?v=gG4urkinFQI)); uxpeak ([How to Design a Great Bottom Mobile Navigation Bar](https://www.youtube.com/watch?v=wLJ40GV2XEc)); TimGabe ([How Top 1% Apps Keep You Hooked](https://www.youtube.com/watch?v=D9SXaj6qQIQ))

### Hero height: test a short phone
A hero at `100vh` on a 700px-tall phone fills the screen and can cut content. Use `min-height` (100svh or dvh) with height fitting content plus about 64px bottom padding. Without a min-height a big screen shows the next section under the hero. Check at 700px height and 360px width. Components should scale with text: `.btn{padding:.5em 1em}`; viewport units only for big sections, because they make buttons microscopic on small screens.
Sources: TimGabe ([From Figma to Framer](https://www.youtube.com/watch?v=XLWXztyA80Q)); TimGabe ([Learn Framer For Beginners](https://www.youtube.com/watch?v=wgMgje60Ovw)); DesignSpo ([24 Web Design Concepts You Need To Know](https://www.youtube.com/watch?v=a_6s4AKQ2VI))

### Responsive scales, adaptive changes layout
Responsive: the same layout scales (card is 33% width). Adaptive: layout changes at a breakpoint (three cards in a row become three rows). Use percent/fr widths for scaling plus breakpoints for layout changes where the layout looks bad small. Keep 2-3 queries; resize continuously from 320 to 1440 and fix what breaks rather than adding in-between breakpoints.
Sources: DesignSpo ([24 Web Design Concepts You Need To Know](https://www.youtube.com/watch?v=a_6s4AKQ2VI)); TimGabe ([Learn Framer For Beginners](https://www.youtube.com/watch?v=wgMgje60Ovw))

### Design mobile beside desktop, and check the real device split
Review each section at 390px next to desktop before moving on, keeping alignment and button sizing consistent. Format shapes flow: tall narrow screens push one descending path with the CTA at the end; wide screens allow side-by-side groups. Stack media and copy only on narrow viewports.
Sources: SelfMadeWebDesigner ([The Easiest Way to Build Killer Websites](https://www.youtube.com/watch?v=O7MaPnRy5Us)); SatoriGraphics ([The Graphic Design Course To MASTER Layout Design](https://www.youtube.com/watch?v=yUvGHNzqG7M)); SatoriGraphics ([Making FAMOUS Graphic Designs Better](https://www.youtube.com/watch?v=Tm25IxJQPWM))

## Where designers disagree

### Text over photos: gradient scrim vs frontend-design's no-gradient ban
frontend-design bans gradients of any kind. Several designers use a bottom-only gradient (about the lower 25%, for example `linear-gradient(to top, rgba(0,0,0,.7), transparent 25%)`), a directional gradient on the text side, or a blurred dark panel behind the text column to keep text legible over busy imagery. Another says to avoid text over images entirely, or use a dark overlay or lowered image opacity. Safe reconciliation: prefer text outside the image; if over it, use a flat low-opacity overlay and check contrast on the lightest part.
Sources: DesignSpo ([I redesigned YOUR websites](https://www.youtube.com/watch?v=-F1F4YISY4E)); TimGabe ([I Made The Biggest Movie Ever Into A Website](https://www.youtube.com/watch?v=R33gaV3EV1I)); SelfMadeWebDesigner ([Ultimate Website Layout Guide](https://www.youtube.com/watch?v=s2DVOZ62F8w))

### Eyebrow above the headline
Several designers recommend a small uppercase or accent-colored label above a huge headline (even demoting a tagline to a superscript at 128px headline size). frontend-design lists ALL-CAPS eyebrows as template chrome. Use sentence case and low emphasis if you need one, and never both eyebrow and brand strip.
Sources: DesignSpo ([PRO Vs AMATEUR Website Design](https://www.youtube.com/watch?v=x8Vp8k3jXaA)); DesignSpo ([The Perfect Website Layout For Startups](https://www.youtube.com/watch?v=Z7r5RNo-hN0))

### Section padding size
frontend-design says py-24 to py-32 (96-128px). One source gives about 160px top and bottom on desktop; others use 64-80px between sections, 64-96px for calming a busy layout, or 96px vertical. The sources agree on consistent, not on a single number. Take the frontend-design default for marketing and 64-80 for denser product pages, then keep it identical across sections.
Sources: TimGabe ([Design Better Than 99% of UI Designers](https://www.youtube.com/watch?v=PGQnGEH7c-E)); uxpeak ([UX/UI Design Tutorial in Figma](https://www.youtube.com/watch?v=SIoOS6tFw1Y)); SatoriGraphics ([Graphic Design Principles Master-Class: White Space](https://www.youtube.com/watch?v=FDFD2-poyGw))

### Mobile-first vs per-size design
One group says start from the most constrained size and scale up, and build desktop and mobile together. Another says the "90% mobile" stat is often about apps, so check analytics for the product's real device split and solve each size on its own rather than only shrinking one version. frontend-design verifies all four widths, which satisfies both. Also: one source says use 12/8/4 grid steps at three breakpoints; frontend-design says breakpoints come from content.
Sources: SatoriGraphics ([I Wish I Knew These Graphic Design Rules SOONER](https://www.youtube.com/watch?v=05EKAJPRrGw)); SelfMadeWebDesigner ([11 Years of Brutally Honest Web Design Advice](https://www.youtube.com/watch?v=WxZHUe8mvhU)); TimGabe ([Learn Framer For Beginners](https://www.youtube.com/watch?v=wgMgje60Ovw))

### Base unit: 4 or 8, and golden ratio
Some say everything divisible by 4; others use 8 with a 4 exception; one says 6 or 8 give too few options. Golden ratio and thirds: some use them as restraint, others call them overrated and say to judge by eye. Rules like 60/30/10 are starting points only.
Sources: DesignSpo ([The Golden Rule Of Web Design](https://www.youtube.com/watch?v=CASPWJUsHPM)); TimGabe ([You'll Regret NOT Using The 8pt Grid in Figma](https://www.youtube.com/watch?v=ohF93_k3IMk)); SatoriGraphics ([Using Grids For NEXT-LEVEL Logo Designs](https://www.youtube.com/watch?v=BC-0TkWP2Js))

### Gradient as hero art
One designer recommends an abstract gradient of vertical bars behind the hero as the page "star". frontend-design bans hero washes. Keep the star idea (one visual tied to the product story, kept behind and out of the text's way) and build it from flat shapes or real product output.
Sources: SelfMadeWebDesigner ([6 EASY Tips to 10x Any Site's Design](https://www.youtube.com/watch?v=pbhLsV-Dyho))
