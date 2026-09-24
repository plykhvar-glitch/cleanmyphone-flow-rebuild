# CleanMy®Phone: onboarding + paywall rebuild

**Live prototype: https://plykhvar-glitch.github.io/cleanmyphone-flow-rebuild/**

A clickable prototype of CleanMy®Phone's onboarding and paywall with the sequence re-ordered for conversion. The art direction is CleanMy®Phone's own: the indigo-to-violet gradient, the light centred headlines, the frosted violet buttons, the cyan primary button, the bubble scan screen, the "Your clutter" list and the three-card plan picker. Only the order and a few additions changed.

Every screen has a side panel with the rationale, what was kept from the app and where the screen sat in the shipping flow. The **Before → After** tab holds the ranked list of changes. Chips under the phone jump to any stage with answers already filled in, including the offer paywall.

## What was kept

- The splash and the welcome screen, with the legal text word for word
- All four feature tour screens, in their original order, with their copy and button labels ("I See", "Alright", "Got It", "Let's Start")
- The scanning screen with the bubbles and the glowing orb, and the "Your clutter" result list
- The paywall layout: Premium Plan header, four icon rows, Monthly / Annual / Lifetime cards with the 3-day trial tab, the cyan button, Restore Purchase · Terms · Privacy
- Both system prompts (notifications and tracking), word for word

## Ranked changes

| # | Priority | Change | What changed | Expected impact |
| :-- | :-- | :-- | :-- | :-- |
| 1 | Fix first | The scan runs before the price | Your app already scans the library and shows "Your clutter", but onboarding never shows it before the price. Photo access and the scan now come first, so the paywall follows a real number of gigabytes. | CR +10–20% |
| 2 | Fix first | System prompts moved after the paywall | The notification and tracking prompts popped up on the welcome screen, before anyone saw the app. They now appear after the paywall. | CR +10–15% |
| 3 | High | Paywall names what was found | The headline said "Try it for free" to everyone. It now says how much space the scan found in the category they picked. | CR +15–20% |
| 4 | High | Second screen when the paywall closes | Closing the paywall ended the flow. It now opens a screen that lays out the 3-day trial date by date, with the $7.99 monthly plan as the alternative. | ARPU +10–15% |
| 5 | High | One question: what to clear first | The flow asked nothing. One tap now picks a category, and the scan, the result list, the paywall and the trial screen all lead with it. | CR +10–15% |
| 6 | High | Rating and awards next to the plans | The 4.6 from 23K ratings, App of the Day and Red Dot appear nowhere in the flow. They now sit above the plan cards. | CR +10–15% · ARPU +2–5% |
| 7 | High | Yearly saving made visible | The Annual card showed $36.99 with nothing to compare it to. It now shows $3.08 a month and SAVE 61% against Monthly. | CR +5–15% · ARPU +10–15% |
| 8 | Medium | Privacy promise before photo access | Photo access is now asked before the paywall. The app's own on-device and no-upload promises sit right above the button. | CR +5–10% |
| 9 | Medium | Real reviews during the scan | Four reviews from macpaw.com now rotate while the scan runs. It is the one moment everyone waits. | CR +5–10% |
| 10 | Medium | Billing line above the button | The trial terms were only in the small grey line inside the button. "Nothing charged today · $36.99/year after 3 days" now sits above it. | CR +3–8% |
| 11 | Low | Button follows the plan | The button said "Start 3-Days Free Trial" whichever card was picked. It now matches Monthly and Lifetime too. | CR +3–8% |
| 12 | Low | Progress dots on the tour | The four feature screens gave no sense of how many were left. Four dots now sit above the button. | CR +5–15% |

## Grounding

Every price, rating, review and award comes from CleanMy®Phone's own published material: the App Store listing (In-App Purchases: Yearly $36.99, Monthly $7.99; 4.6 from 23K ratings; the 3-day trial terms), macpaw.com/cleanmyphone (7M downloads, App of the Day, Red Dot 2024–2025, UX Design Awards, four named reviews, the sample "Your clutter" library) and the app's own screens (Lifetime $89.99). The scan numbers are MacPaw's published demo library; in the app they are the user's own. The full list, including figures deliberately left out, is in **Sources & grounding** inside the prototype.

*Impact ranges are Adapty's expected effect from teardowns and A/B tests across subscription apps — not measured lift for CleanMy®Phone.*

## Run locally

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.
