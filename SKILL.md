---
name: design-wisdom
description: Design tactics and audit moves distilled from about 800 talks by working designers (Tim Gabe, DesignSpo, uxpeak, Hatch Conference, Satori Graphics, Will Paterson, Amir Moradi, Shantanu Kumar, Self-Made Web Designer). Use when reviewing or polishing a web app's UX, designing a landing, pricing, onboarding or billing flow, auditing an AI-built UI that looks generic, designing loading, empty, error and limit states, or building a brand identity. Complements frontend-design, which sets the taste rules; this skill supplies the moves that find what is wrong and the patterns that fix it.
---

# Design Wisdom

Designers rarely fix a product by knowing more rules. They fix it by running specific moves on the real screens: blur it, break it, compare screen 1 with screen 80, hand it to a stranger for five seconds. This skill is a library of those moves, plus the patterns they lead to.

## How it fits with frontend-design

- frontend-design owns the hard rules: tokens, type sizes, motion timings, hard bans. When a note here conflicts with it (gradients, Inter, ALL-CAPS eyebrows, one accented headline word), frontend-design wins unless the user says otherwise.
- Each reference ends with `Where designers disagree`. Read those as context for a deliberate choice, never as permission to break a ban.
- This skill adds what frontend-design lacks: audit tactics, state and flow design, conversion, premium feel, psychology and brand.

## When building

1. **Brief first.** Before styling, write five lines: who it is for, the one job of this screen, three values or tone words, the 1-2-3 rank of what the user must see, and what the screen must not look like (the category cliche). Every later choice should trace back to a line.
2. **State table before screens.** List every state the flow can reach (empty, loading, slow, partial, error, offline, limit reached, success, undo window) and design each one. AI-built products skip exactly these, and they are where premium is earned.
3. **Wireframe with real content** in gray boxes, rank 1-2-3, then add color.
4. **Spend boldness in one place.** Keep conventions for finding things (nav, forms, settings) and put the product's one signature move where users spend the most time.
5. **Run the core review moves below** before calling it done.

## When reviewing

Run moves from the playbook on the rendered product, not the code. For each finding, record the move that found it, the evidence (a screenshot or exact copy), and the fix. Use frontend-design's severity scale. Fix papercuts in batches; stop at good enough once no HIGH remains.

## Core moves (run these every time)

| Move | How an agent runs it | What it catches |
|---|---|---|
| **Blur, grayscale, thumbnail** | Screenshot with `filter: blur(6px)`, then `grayscale(1)`, then view at 25% size | Whether the H1 and primary CTA are the top two blobs; color carrying hierarchy that value should carry |
| **Rank 1-2-3** | Write the intended order, then compare it with what wins the blur test | Competing loud elements, a buried CTA |
| **Break it on purpose** | Go offline mid-flow, force a 500 and a hang, fail the payment, empty every list, hit every limit | Silent failures, false "Saved", dead ends with no next step |
| **Ugly content** | 60-char names, 80-char strings with no spaces, missing images, 0 and 10,000 items | Overflow, broken truncation, layouts that only work with demo data |
| **Screen 1 vs screen 80** | Screenshot every route, put them side by side, list where buttons, spacing, copy and patterns differ | The product no longer feeling like one product |
| **Landing vs app** | Compare the marketing page with the logged-in app at the same zoom | A billboard promise the product does not keep |
| **Five-second cold read** | Give a fresh subagent only the screenshot, no brief: "what is this, who is it for, what do I do next?" | Unclear value, wrong audience signal |
| **Read only the headings** | Extract the H1 and H2s of the page and read them alone | A story that does not sell or explain |
| **Swap the logo** | Put the page next to 3 to 5 competitor pages with logos hidden | A generic look with no decision of its own |
| **Remove one element** | Delete each element in turn; if nothing breaks, it goes | Clutter, decoration without a job |
| **Three objections** | Write the three objections the user has at this step, check each is answered on screen | Missing proof, price or risk answers |
| **Walk to the first win** | Sign up as a new user and count clicks and seconds to first value | Onboarding that asks before it gives |

## Patterns these moves usually lead to

- Every action answers within 400ms: say what happened, offer a way back, and say what to do next.
- Errors name the cause and the fix and keep the user's input, with Retry or Contact support right there.
- Limits use one component everywhere: "2 of 2 used", plus the exact reset date and the upgrade path.
- Long work narrates named steps and offers Cancel. A spinner alone is never enough past a few seconds.
- Empty states give a starter kit or sensible defaults, not just a sentence.
- Onboarding reaches the first win within about 60 seconds; ask only for what the product needs now.
- Pricing shows one exact price, the charge date, the trial timeline and how to cancel, near the button.
- The landing hero states the outcome for a named audience, shows the real product, and puts proof beside the one filled CTA.
- Premium is evidence of care, more than looks: handled states, undo, consistency, and a well-handled failure.

## References

Open the file that matches the task. Each entry has the move, what to look for, the fix, and video sources.

| File | Open when |
|---|---|
| [audit-playbook.md](references/audit-playbook.md) | Reviewing any product: perception passes, first-time-user simulation, break-it passes, journey walks, cross-screen comparison, critique and iteration loops, auditing AI-generated screens |
| [states-and-flows.md](references/states-and-flows.md) | Designing onboarding, empty, loading, error and limit states, AI output states, forms, filters, navigation |
| [conversion-and-copy.md](references/conversion-and-copy.md) | Landing pages, hero, CTAs, section order, social proof, pricing and paywalls, microcopy |
| [premium-and-not-generic.md](references/premium-and-not-generic.md) | A product that looks generic or AI-built, consistency across screens, polish passes, motion, perceived performance |
| [hierarchy-and-spacing.md](references/hierarchy-and-spacing.md) | Layout feels off: hierarchy, focal point, spacing system, grids, imagery, responsive reflow |
| [type-and-color.md](references/type-and-color.md) | Choosing or auditing type and palette, contrast matrices, dark mode, accessibility past the floor |
| [psychology.md](references/psychology.md) | Explaining or deciding why a design works: attention, memory limits, trust, peak-end, habits, ethics of engagement |
| [branding.md](references/branding.md) | Brand brief and voice, logo design and testing, differentiating from the category, carrying the brand into the product |

## Running the moves as an agent

- Use any browser automation for screenshots. Blur, grayscale and flip are one injected style: `document.documentElement.style.filter = 'blur(6px)'`.
- Simulate failure with request interception or devtools network conditions: offline, 500, a request that never returns.
- Stand in for a stranger with a fresh subagent that sees only the screenshot. Never give it the brief, because knowing the intent hides the problem.
- Cited studies in the references are as the speakers quoted them. Use them for direction, and check the original before putting a number in user-facing copy.
