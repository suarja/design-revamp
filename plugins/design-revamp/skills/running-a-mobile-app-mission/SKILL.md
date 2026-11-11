---
name: "running-a-mobile-app-mission"
description: "Entry point for any work on a mobile app, ours or a client's. Pick the mission (understand the app, find what brings users back, redo one screen, revamp the whole app, position it on the store, store visuals, release, prove it works, promote it), then chain the existing skills in order with their inputs, deliverables and owner gates. Holds the phase map from discovery to launch, the Air France effect checks and the known gaps. Use when someone asks to revamp, redesign, position, ship or make an app addictive, when a client app arrives, or when you do not know which design, product or release skill to start with."
---

# Running a mobile app mission

This skill is a map. It adds no method of its own: every step below belongs to a skill
that already exists. Start from the mission that was asked, not from phase 0. Most
requests are one mission ("just redo these screens"); a full engagement chains them.

## 1. Pick the mission

| Mission | Skills, in order | Needs as input | Delivers | Usually next |
| --- | --- | --- | --- | --- |
| Understand the app before touching it | `diagnosing-product-stage`, `championing-an-epic` steps 1-2, `running-discovery-interviews` when users are reachable | The app running, its store page, its reviews | Hypothesis cards, the user's problem in their words, one KPI and one guardrail, the scope with what is refused | Find what brings users back |
| Find what brings users back | `finding-gesture-primitives`, `design-bank` | The scope | The core gesture, its trace, the chosen Air France moments, named references | Revamp |
| Redo one screen | `revamping-a-screen` (calls `design-bank`, `canvas-generation`) | The current capture, the sentence the screen must make understood | An accepted canvas, then the coded screen compared with it | Prove it works |
| Revamp the whole app | `revamping-an-app` (calls the three above, `explainer-mascot-poses`, `codex`) | Captures of every screen, navigation read from the code, the copy from the locale files | Direction, one board per screen group, states board, copy board, icon, merged lots | Prove it works, then store visuals |
| Position it on the store | `positioning-an-app-on-the-store` | The owner's words for the category and the message order | Promise, measured keywords with date, fields split, refusals recorded | Store visuals |
| Store visuals | `store-screenshot-art-direction`, `app-showcase-pipeline`, `app-store-preview-video` | The shipped design, the positioning | Screenshot pack per locale, App Preview video | Release |
| Release | `releasing-mobile-apps` | An integrated branch | Build in the store, OTA on the right runtime, release record | Measure |
| Prove it works | `mobile-visual-validation`, `expo-metro-tunneling`, `expo-shared-workstation-runs` | A build | iPhone and iPad captures at 100 %, PASS, FAIL, NOT RUN or BLOCKED per check | The owner's walk on a real phone |
| Promote it | `choosing-a-short-format`, `designing-motion-promo-shorts`, `explainer-video-pipeline`, `writing-build-in-public-posts` | Real captures, before and after | Shorts, a build-in-public post, a before/after case | Measure |
| Measure | `championing-an-epic` steps 6-7, PostHog skills (`instrument-product-analytics`, `modeling-activation-metrics`, `creating-surveys`) | The KPI of the first mission | J+7 and J+30 checkpoints, a proof card | The next mission |

If the request fits none of these rows, say so and ask; do not stretch a row.

## 2. A full engagement

Chain the missions in this order. Each phase ends on a gate the owner (or the client)
passes before the next starts.

| # | Phase | Mission row | Gate |
| --- | --- | --- | --- |
| 0 | Audit | Understand the app (the reading part) | The "before" captures, store page, ratings and baseline numbers are written down |
| 1 | Discovery and scope | Understand the app (the deciding part) | Scope signed, with what is refused, in black and white |
| 2 | Positioning | Position it on the store | The owner picks the promise among two or three measured options |
| 3 | The loop | Find what brings users back | The owner picks the gesture and the moments |
| 4 | Design | Redo one screen or Revamp the whole app | Every board accepted before any code |
| 5 | Build | Revamp the whole app, delegation part | Each lot reviewed against its board before the next |
| 6 | Validation | Prove it works | The owner walks the app on a real phone; the Air France checks below |
| 7 | Launch | Store visuals, Release, Promote it | The owner's go before any submission or publication |
| 8 | Measure and case study | Measure | Before/after and numbers ready to show |

Scope fixed to the millimetre is what frees time for polish. Refuse scope that does not
serve the KPI and park it; that saved effort goes into phases 4 to 6.

## 3. The Air France effect

The owner's words: looking forward to booking a flight just to use the Air France app.
The whole trip is followed, with Live Activities, micro-animations and "aha" moments,
and the loop brings people back. Provisional checks, to confirm with the owner after the
first client case:

1. **Anticipation.** The user looks forward to one precise moment of the app.
2. **Presence outside the app.** Live Activity, widget or notification at the right time.
3. **An answer to every gesture.** Motion or haptic feedback, never a frozen screen.
4. **A trace that grows.** The owner's question: "What does this build?"
5. **Return without chasing.** People come back without being prompted.

Mark each check PASS, FAIL or NOT RUN in phase 6. A guess stays NOT RUN.

## 4. Rules

- Read the app as it is before proposing anything: real screens on a simulator,
  navigation from the code, copy from the locale files.
- A departure from the current product is a proposal, written as such, decided by the
  owner. Never present your taste as the owner's decision.
- Store submission, publication, outreach and any paid tool need the owner's go.
- For a client app, keep the client's repository, brand and data in the client's
  project. Nothing from a client goes into this marketplace except anonymised lessons.
- After each mission, write the lesson into the skill that owns that step (`omni-lessons`),
  then update this map only if a row changed.

## 5. Known gaps

Say a gap out loud when a mission hits it; do not improvise a method silently.

| Gap | Where it hurts | Current workaround |
| --- | --- | --- |
| No skill for delight moments and the retention loop (Live Activities, widgets, haptics, motion) | Phases 3 to 5 | `finding-gesture-primitives` for the loop, Expo skills (`expo-animation`, `expo-native-ui`) for the build |
| Boards are static | Phase 4 | Describe motion in the board legend, prototype it in code in one lot |
| No keyword-ranking tracking script, no rule for asking ratings | Phase 2, after launch | Re-measure by hand after two to four weeks; ask for a rating after the first real success |
| No consumer audit grid (store reviews, funnel, retention) | Phase 0 | `diagnosing-product-stage` plus reading the reviews by hand |
| No test with real users after the build | Phase 6 | The owner's walk, three to five people from the network |
| `releasing-mobile-apps` assumes Expo, EAS and Convex | Phase 7 for another stack | Follow its order, adapt the commands to the client's stack |
| No case-study format, no outreach to store developers | Phase 8 | `writing-build-in-public-posts` for the before/after; outreach by hand |
